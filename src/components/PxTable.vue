<template>
  <main class='PxTable'>
    <PxToken tokenName="rock" />
    <PxToken tokenName="paper" />
    <PxToken tokenName="scissors" />
  </main>
</template>

<style lang="scss">
@import '../assets/scss/main';

.PxTable {
  display: flex;
  flex-wrap: wrap;
}
</style>

<script>
import PxToken from '@/components/PxToken'

export default {
  name: 'PxTable',
  components: { PxToken }
}
</script>
