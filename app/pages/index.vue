<template>
  <div>
    <NuxtRouteAnnouncer />
    <Information />
    <Stack />
    <Project />
    <Experience />
    <Formation />
    <Contact />
  </div>
</template>
<script setup>

import Stack from '~/components/Stack.vue';
import Information from '~/components/Information.vue';
import Project from '~/components/Project.vue';
import Experience from '~/components/Experience.vue';
import Formation from '~/components/Formation.vue';
import Contact from '~/components/Contact.vue';

</script>