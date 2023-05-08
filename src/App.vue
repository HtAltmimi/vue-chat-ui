<script setup>
import ChatList from "@/components/ChatList.vue";
import { ref } from "vue";
const conversations = ref([]);
conversations.value.push({
  title: "Chat with Ahmed",
  messages: [
    {
      outgoing: true,
      text: "Hi , Ahmed ",
      username: "ahmed1998",
    },
    {
      outgoing: false,
      text: "Hello, Ali!",
      username: "hhh",
    },
  ],
});
conversations.value.push({
  title: "Chat with Krar",
  messages: [
    {
      outgoing: true,
      text: "Hi, Krar",
      username: "hdrm147",
    },
    {
      outgoing: false,
      text: "Hello, Ali!",
      username: "azeez",
    },
  ],
});
</script>
<template>
  <div class="container flex justify-center">
    <chat-list :conversations="conversations"></chat-list>
  </div>
</template>
