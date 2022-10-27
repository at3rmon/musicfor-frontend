<script setup>
import Copywrites from "@/components/Copywrites.vue";
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import {
  faTwitter,
  faYoutube,
  faFacebookF,
  faPinterest,
  faFoursquare,
} from "@fortawesome/free-brands-svg-icons";
library.add(faTwitter, faYoutube, faFacebookF, faPinterest, faFoursquare);
</script>

<template>
  <footer class="bg-neutral text-neutral-content">
    <section
      class="h-96 bg-cover bg-no-repeat bg-fixed flex justify-center items-center bg-blend-multiply bg-neutral"
      style="background-image: url(../src/assets/images/musicfor-live.jpg)"
    >
      <p class="max-w-lg text-center italic text-2xl">
        <span class="divider text-sm">Quote</span>
        "...everyone on that train can be going the same direction but have
        different destinations..."
        <span class="divider"></span>
      </p>
    </section>
    <section
      class="flex flex-col gap-2 md:flex-row justify-between items-center p-4"
    >
      <Copywrites />
      <section class="flex gap-2">
        <a
          href="https://twitter.com/musicforedu"
          target="_blank"
          class="hover:text-accent hover:scale-110 transition duration-150 text-3xl"
        >
          <font-awesome-icon icon="fa-brands fa-twitter" />
        </a>
        <a
          href="https://www.facebook.com/musicforEdu"
          target="_blank"
          class="hover:text-accent hover:scale-110 transition duration-150 text-3xl"
        >
          <font-awesome-icon icon="fa-brands fa-facebook-f" />
        </a>
        <a
          href="https://www.pinterest.com/musicforedu/"
          target="_blank"
          class="hover:text-accent hover:scale-110 transition duration-150 text-3xl"
        >
          <font-awesome-icon icon="fa-brands fa-pinterest" />
        </a>
        <a
          href="http://4sq.com/1CNGu0B"
          target="_blank"
          class="hover:text-accent hover:scale-110 transition duration-150 text-3xl"
        >
          <font-awesome-icon icon="fa-brands fa-foursquare" />
        </a>
        <a
          href="https://www.youtube.com/channel/UCAmIGNdNLlak8NQzZnpuQ1g"
          target="_blank"
          class="hover:text-accent hover:scale-110 transition duration-150 text-3xl"
        >
          <font-awesome-icon icon="fa-brands fa-youtube" />
        </a>
      </section>
    </section>
  </footer>
</template>
