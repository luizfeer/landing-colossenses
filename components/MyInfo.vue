<template>
    <div class="flex flex-col items-center justify-center">
        <h1 class="font-sans font-normal text-2xl md:text-3xl text-zinc-900 dark:text-zinc-50/90">{{ name }}</h1>
        <h2 class="font-sans font-light text-xl md:text-xl text-zinc-800/90 dark:text-zinc-50/70">{{ title }}</h2>
        <p class="font-sans  text-lg md:text-lg text-zinc-800/60 dark:text-zinc-400 my-10 bg-yellow-900 bg-opacity-30 bg-blend-color-burn p-4 rounded-md">
            A Colossensess é uma página cristã reformada que tem por objetivo expandir o Reino de Deus e glorificar o nome dEle. A página é administrada por Tainá Oliveira e Mariana Sivieri, duas jovens cristãs reformadas. O conteúdo é fiel às Escrituras, o nosso propósito é ensinar, instruir, exortar e cumprir o chamado do Senhor, de pregar o seu Evangelho.
        </p>
    </div>
</template>

<script setup>
const app = useAppConfig();
const { data: { name, title, bio } } = app
</script>
