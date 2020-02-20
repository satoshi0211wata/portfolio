<template>
  <div>
    <h2>{{ title | lowerCase | upperCase }}</h2>
    <p>{{ subTitle | upperCase | lowerCase }}</p>
    <P>{{ number }}</P>
    <button @click="number++">+1</button>
  </div>

</template>

<script>
import { tokyoNumber } from "@/tokyoNumber";

export default {
  mixins: [tokyoNumber],
  created() {
    console.log("created in component");
  }
};
</script>