<template>
  <header class="header">
    <h1>Rock <br/> Paper <br/> Scissors</h1>
    <px-score />
  </header>
</template>

<style lang="scss" scoped>
@import '../assets/scss/main';

.header {
  width: 80%;
  max-width: 1024px;
  margin: auto;
  padding: 12px 12px 12px 23px;
  border: 3px solid rgba(255,255,255, .29);
  border-radius: .5em;
  display: flex;
  justify-content: space-between;
  align-items: center;

  h1 {
    color: white;
    font-size: 18px;
    line-height: 16px;
    font-weight: 700;
    text-transform: uppercase;
  }
}
</style>

<script>
import PxScore from '@/components/PxScore'

export default {
  name: 'PxHeader',
  components: { PxScore }
}
</script>
