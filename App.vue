<template>
  <div id="app">
    <h1>Chuck Norris Jokes</h1>
    <ul>
      <li v-for="(joke, index) in chuck" :key="index">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chuck: [
        { value: "Chuck Norris can skydive into outer space." },
        { value: "The chief export of Chuck Norris is pain." },
        { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  text-align: center;
  margin: 20px;
}

h1 {
  color: #2c3e50;
  margin-bottom: 20px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  background-color: #f4f4f9;
  border: 1px solid #ccc;
  border-radius: 8px;
  margin: 10px 0;
  padding: 10px;
  text-align: left;
  font-size: 18px;
  color: #333;
  transition: background-color 0.3s ease;
}

li:hover {
  background-color: #e0f7fa;
}
</style>
