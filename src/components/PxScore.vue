<template>
  <section class="PxScore">
    <small>Score</small>
    <p>12</p>
  </section>
</template>

<style lang="scss" scoped>
@import '../assets/scss/main';

.PxScore{
  background: white;
  text-align: center;
  padding: 10px 0;
  border-radius: 8px;
  width: 80px;

  small {
    letter-spacing: 1.5px;
    color: #2A45C2;
    text-transform: upperCase;
    font-size: 10px;
    font-weight: bold;
  }

  p {
    color: #565468;
    font-size: 40px;
    margin: 0;
    font-weight: 700;
  }
}
</style>

<script>
export default {
  name: 'PxScore'
}
</script>
