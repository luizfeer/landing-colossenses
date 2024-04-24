<template>
    <div class="p-4 rounded-2xl">
        <iframe class="rounded-2xl" src="https://open.spotify.com/embed/playlist/7g5SuefIr2F8zGcWntm4sw?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

    </div>
    <UContainer>
        
        <footer class="flex items-center justify-evenly py-12 relative z-20">
            <NuxtLink :to="`mailto:${email}`"
                class="text-sm text-zinc-700 hover:text-zinc-950 dark:text-zinc-50/80 hover:dark:text-zinc-50">
                {{ email }}
            </NuxtLink>
            <!-- <NuxtLink to="https://github.com/cesswhite/hato-minimal-template" target="_blank"
                class="text-sm text-zinc-700 hover:text-zinc-950 dark:text-zinc-50/80 hover:dark:text-zinc-50">
                Donwload Hato | Free Template
            </NuxtLink>
            <NuxtLink :to="`tel:${phone}`"
                class="text-sm text-zinc-700 hover:text-zinc-950 dark:text-zinc-50/80 hover:dark:text-zinc-50">
                {{ phone }}
            </NuxtLink> -->
        </footer>
    </UContainer>
</template>


<script setup>
const app = useAppConfig();
const { data: { email, phone } } = app
</script>
