<template>
  <div class="w-full relative min-h-screen h-full pt-12 bg-zinc-50 dark:bg-zinc-950">
    <div class="relative z-20">
      <LazySwitchMode />
      <UContainer>
        <div v-motion-fade class="flex flex-col gap-2 items-center justify-center">
          <LazyPhotoProfile />
          <LazyMyInfo />
          <LazySocialNetwork />
          <LazyGallery />
        </div>
      </UContainer>
    </div>
    <Footer />
    <img v-motion-fade-visible src="/shadow.png"
      class="object-cover object-center fixed w-full h-full left-0 top-0 z-10 dark:mix-blend-soft-light"
      alt="shadow-background" loading="lazy">
  </div>
</template>

<script setup>
const img = useImage()
useSeoMeta({
  title: 'COLOssensess',
  ogTitle: 'COLOssensess - Site Oficial',
  description:
    'Cultivando uma vida com intencionalidade e propósito.',
  ogDescription:
    'Cultivando uma vida com intencionalidade e propósito.',
  ogImage: "https://colossensess.com/og.jpg",
  ogImageSecureUrl: 'https://colossensess.com/og.jpg',
  ogUrl: 'https://colossensess.com/og.jpg',
  twitterImage: "https://colossensess.com/og.jpg",
  twitterCard: "summary_large_image",
  twitterTitle: 'COLOssensess - Site Oficial',
  twitterDescription: 'Cultivando uma vida com intencionalidade e propósito.',
  ogImageWidth: 1200,
  ogImageHeight: 630,
});

useHead({
  htmlAttrs: {
    lang: 'pt-BR'
  },
  link: [
    {
      rel: 'icon',
      type: 'image/svg',
      href: '/favicon.ico'
    }
  ]
})
</script>
