<template>
    <div class="contact-page">
        <h1>Contactez-nous</h1>
        <form class="contact-form">
            <div class="form-group">
                <label for="name">Nom:</label>
                <input type="text" id="name" name="name" required />
                <label for="prenom">Prénom:</label>
                <input type="text" id="prenom" name="prenom" required />
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required />
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
                <button type="submit">Envoyer</button>
            </div>
        </form>
      
    </div>
</template>


<style scoped>
.contact-page {
    max-width: 600px;
    margin: 40px auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 8px;
    background-color: #f9f9f9;
}
.contact-page h1 {
    text-align: center;
    color: rebeccapurple;
}
.contact-form {
    display: flex;
    flex-direction: column;
}
.form-group {
    display: flex;
    flex-direction: column;
    gap: 12px;
    margin-bottom: 16px;
}

.form-group label {
    font-weight: bold;
    color: #333;
}
.form-group input,
.form-group textarea {
    padding: 8px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 16px;
}

.form-group button {
    padding: 10px;
    background-color: rebeccapurple;
    color: white;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    cursor: pointer;
    transition: background-color 0.3s;
}
.form-group button:hover {
    background-color: #5e35b1;
}
.form-group button:active {
    background-color: #4a2c91;
}
.form-group button:focus {
    outline: none;
    box-shadow: 0 0 0 3px rgba(103, 58, 183, 0.5);
}
.form-group input:focus,
.form-group textarea:focus {
    outline: none;
    border-color: rebeccapurple;
    box-shadow: 0 0 0 3px rgba(103, 58, 183, 0.2);
}
@media (max-width: 600px) {
    .contact-page {
        margin: 20px;
        padding: 15px;
    }
    .form-group input,
    .form-group textarea {
        font-size: 14px;
    }
    .form-group button {
        font-size: 14px;
        padding: 8px;
    }
}

</style>