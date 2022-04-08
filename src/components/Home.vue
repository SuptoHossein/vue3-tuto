<template>
  <h1>Vuejs 3 Tutorial</h1>

  <!-- <InterpolationAndData /> -->
  <!-- <MethodsWithParams /> -->
  <!-- <EventsComponent /> -->
  <!-- <TwoWayBinding /> -->
  <!-- <GetInputFieldValue /> -->
  <!-- <GetCheckboxRadioButtonValue /> -->
  <!-- <IfElse /> -->
  <!-- <ForLoop /> -->
  <!-- <PassDataParentToChild name="supto" :usrDetails="user" :usrData="getData" /> -->

  <ul>
    <li v-for="user in users" :key="user.name">
      <ReuseComponent :usersData="user" :getAlert="getAlert" />
    </li>
  </ul>
</template>

<script>
// import InterpolationAndData from "./InterpolationAndData.vue";
// import MethodsWithParams from "./MethodsWithParams.vue";
// import EventsComponent from "./Events.vue";
// import TwoWayBinding from "./TwoWayBinding.vue";
// import GetInputFieldValue from "./GetInputFieldValue.vue";
// import GetCheckboxRadioButtonValue from "./GetCheckbox&RadioButtonValue.vue";
// import IfElse from "./IfElse.vue";
// import ForLoop from "./ForLoop.vue";
// import PassDataParentToChild from "./PassDataParentToChild.vue";
import ReuseComponent from "./ReuseComponent.vue";

export default {
  name: "Home-component",
  components: {
    // InterpolationAndData,
    // MethodsWithParams,
    // EventsComponent,
    // TwoWayBinding,
    // GetInputFieldValue,
    // GetCheckboxRadioButtonValue,
    // IfElse,
    // ForLoop,
    // PassDataParentToChild,
    ReuseComponent,
  },
  data() {
    return {
      user: { name: "Peter", email: "peter@test.com" },
      users: [
        {
          name: "supto",
          email: "supto@test.com",
        },
        {
          name: "peter",
          email: "peter@test.com",
        },
        {
          name: "sam",
          email: "sam@test.com",
        },
        {
          name: "tony",
          email: "tony@test.com",
        },
      ],
    };
  },
  methods: {
    getData() {
      console.log("parent function called");
    },
    getAlert(name) {
      alert(name);
    },
  },
};
</script>

<style scoped>
h1 {
  color: orange;
}
</style>