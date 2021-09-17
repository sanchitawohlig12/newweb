<template>
  <v-tabs class="d-flex justify-end">
    <v-btn v-for="social in socials" :key="social" icon :href="social.href">
      <v-icon :color="social.color">
        {{ social.icon }}
      </v-icon>
    </v-btn>
  </v-tabs>
</template>

<script>
export default {
  data() {
    return {
      socials: [
        {
          name: "facebook",
          icon: "mdi-facebook",
          color: "blue darken-1",
          href: "https://www.facebook.com",
        },
        {
          name: "instagram",
          icon: "mdi-instagram",
          color: "pink lighten-2",
          href: "https://www.instagram.com",
        },
        {
          name: "pinterest",
          icon: "mdi-pinterest",
          color: "red lighten-1",
          href: "https://www.pinterest.com",
        },
        {
          name: "twitter",
          icon: "mdi-twitter",
          color: "blue lighten-1",
          href: "https://www.twitter.com",
        },
        {
          name: "youtube",
          icon: "mdi-youtube",
          color: "red",
          href: "https://www.youtube.com",
        },
      ],
    };
  },
};
</script>

<style>
</style>
