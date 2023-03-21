<template>
    <div>
      <ul v-for="post in posts" v-bind:key="post.id">
        <li>{{ post.title.rendered }}</li>
        <p>{{ post.content.rendered }}</p>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        posts: [],
      };
    },
    methods: {
      async getData() {
        try {
          let response = await 
          fetch("https://wordpress-878924-3326173.cloudwaysapps.com/wp-json/wp/v2/posts");
          this.posts = await response.json();
        } catch (error) {
          console.log(error);
        }
      },
    },
    created() {
      this.getData();
    },
  };
  </script>