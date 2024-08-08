<script setup>

import { ref, reactive } from 'vue'
  const title = 'VALORANT'
  let price = ref(9.99)
  function increment() {
    price.value += 1
    instructor.age += 1
    instructor.sns.follower += 1
  }

  const instructor = reactive({
    name : 'ken',
    age : 20,
    sns : {
      twitter : '@@',
      instagram : 'tyotyo',
      follower : 20
    }
  })

  const sectionInfo = {
    sections : ref(10),
    kind : ref('japanese')
  }
</script>

<template>
  <h1>Title: {{ title }}</h1>
  <h2>Price: {{ price }}</h2>
  <h2>Instructor Name: {{ instructor.name }}</h2>
  <h2>Instructor Age: {{ instructor.age }}</h2>
  <h2>Instructor Sns: {{ instructor.sns.twitter }}</h2>
  <h2>Instructor Sns: {{ instructor.sns.instagram }}</h2>
  <h2>Instructor Sns Follower : {{ instructor.sns.follower }}</h2>
  <h2>Section Info: {{ sectionInfo.sections.value }}</h2>
  <button @click="increment">button</button>
</template>
<style>

</style>


