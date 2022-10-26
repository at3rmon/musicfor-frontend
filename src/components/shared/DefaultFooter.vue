<script setup>
import Copywrites from "@/components/Copywrites.vue";
import { library } from "@fortawesome/fontawesome-svg-core";
/* import font awesome icon component */
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
/* import specific icons */
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
  <footer class="footer items-center p-4 bg-neutral text-neutral-content">
    <div class="items-center grid-flow-col">
      <Copywrites />
    </div>
    <div class="grid-flow-col gap-4 md:place-self-center md:justify-self-end">
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
    </div>
  </footer>
</template>
