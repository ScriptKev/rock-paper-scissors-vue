<template>
  <div class="home">
    <PxHeader />
    <PxTable />
  </div>
</template>

<style lang="scss" scoped>
@import '../assets/scss/main';

.home {
  height: 100%;
  width: 100%;
  padding: 20px 0;
  font-family: 'Barlow Semi Condensed', sans-serif;
  color: hsl(229, 25%, 31%);
  background: radial-gradient(circle, hsl(214, 47%, 23%) 0%, hsl(237, 49%, 15%) 100%);
}
</style>

<script>
import PxHeader from '@/components/PxHeader'
import PxTable from '@/components/PxTable'

export default {
  name: 'Home',
  components: { PxHeader, PxTable }
}
</script>
