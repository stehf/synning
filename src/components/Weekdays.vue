<template>
  <div class="weekday">
    <h3>{{todayName}}</h3>
  </div>
</template>
<script>
  import days from "./json/color-map.json"

  // get today's hex code
  const date = new Date();
  const today = date.getDay();
  const todayColor = days[today].hexCode || "#000";
  const todayName = days[today].name || "Happy Birthday!";

  export default {
    name: 'Weekdays',
    data() {
      return {
        todayColor: todayColor,
        todayName: todayName
      }
    }
  }
</script>
<style>
  h3 {
    color:  white;
    font-size: 10em;
    margin:  0;
    text-shadow: 2px 2px 4px #000000;
  }
  .weekday {
    background-color: v-bind(todayColor);
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>