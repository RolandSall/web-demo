<template>
  <v-app>
    <v-container >
      <Navbar />
      <div v-for="item  in 3 " :key="item">
        <Post/>
      </div>
    </v-container>
  </v-app>
</template>

<script>

import SubmitButton from "./components/Buttons/SubmitButton";
import Navbar from "./components/Navbar";
import Post from "./components/Post";

export default {
  name: 'App',
  components: {
    Navbar,
    SubmitButton,
    Post,
  },
  data() {
    return {
      //
    }
  }
}
</script>
