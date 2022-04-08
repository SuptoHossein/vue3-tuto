<template>
  <div>
    <h1>For Loop</h1>
    <ul>
      <li v-for="item in technology" v-bind:key="item">
        {{ item }}
      </li>
    </ul>
    <br /><br />
    <ul>
      <li v-for="user in users" v-bind:key="user.name">
        Name is: {{ user.name }} and email is: {{ user.email }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ForLoop",
  data() {
    return {
      technology: ["java", "javascript", "php", "golang"],
      users: [
        { name: "supto", email: "supto.hossein@gmail.com" },
        { name: "sam", email: "sam.hossein@gmail.com" },
        { name: "bruce", email: "bruse.hossein@gmail.com" },
        { name: "tony", email: "tony.hossein@gmail.com" },
      ],
    };
  },
};
</script>

<style>
</style>