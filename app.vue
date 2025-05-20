<script setup>
const event = {
  name: "Fire Trail Nesselwang"
};

useSeoMeta({
  ogImage: "https://allgaeu-competition.vercel.app/og.jpg",
  ogTitle: event.name,
});

useHead({
  titleTemplate: (pageTitle) => [pageTitle, event.name].filter(Boolean).join(" | "),
  viewport: "width=device-width, initial-scale=1, maximum-scale=1",
  charset: "utf-8",
  meta: [
    { property: "og:type", content: "website" },
    { name: "twitter:card", content: "summary_large_image" },
    { name: "apple-mobile-web-app-title", content: event.name },
    { "http-equiv": "refresh", content: "10; url=https://nesselwang-competition.vercel.app" }
  ],
  script: [
    {
      src: "https://plausible.io/js/script.js",
      "data-domain": "nesselwang-competition.vercel.app",
      defer: true,
    }
  ],
  link: [
    {
      rel: "icon",
      type: "image/png",
      href: "/favicon-96x96.png",
      sizes: "96x96",
    },
    {
      rel: "icon",
      type: "image/svg+xml",
      href: "/favicon.svg",
    },
    {
      rel: "shortcut icon",
      href: "/favicon.ico",
    },
    {
      rel: "apple-touch-icon",
      sizes: "180x180",
      href: "/apple-touch-icon.png",
    },
    {
      rel: "manifest",
      href: "/site.webmanifest",
    },
  ],
});
</script>

<template>
  <div>
    <section class="section">
      <div class="container">

        <div class="notification">
            <p class="title">Die Allgäu Competition hat einen neuen Namen!</p>
            <p>Wir freuen uns, dich am Samstag, den 18. Oktober 2025 zum
            <strong>Fire Trail Nesselwang</strong> begrüßen zu dürfen!</p>
        </div>

        <p class="pl-5">
          <a href="//nesselwang-competition.vercel.app" class="has-text-grey-lighter">
            Wir leiten dich weiter .. wenn du nicht so lange warten möchtest: klicke hier.
          </a>
        </p>

      </div>
    </section>
  </div>
</template>

<style>
@import url("bulma");
</style>
