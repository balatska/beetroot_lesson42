<template>
  <div>
    <!-- <h1 v-once>{{ title }}</h1>
    <p>
      {{ getTitle() }}
    </p>
    <h1>{{ title }}</h1>

    <a v-bind:href="url">Google</a><br>

    {{ link }}
    <p v-html="link"></p> -->

    <counter />
    <counter />
  </div>
</template>

<script>
import Counter from "@/components/Counter";

export default {
  name: 'app',
  components: {
    'counter': Counter,
  },
  data() {
    return {
      title: 'Some title',
      url: 'https://google.com',
      link: "<a href=\"https://google.com\">Google</a>",
    }
  },
  methods: {
    getTitle() {
      this.title = 'Some other title';

      return this.title;
    }
  },
}
</script>


