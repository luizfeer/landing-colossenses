<template>
    <UAvatar class='dark:block hidden' src="/logo-dark.png" size="3xl" alt="my-profile-photo" height="200" />
    <UAvatar class="dark:hidden block" :src="photo" size="3xl" alt="my-profile-photo" height="200" />
</template>

<script setup>
const app = useAppConfig();
const { data: { photo } } = app
</script>
