<template>
  <div class="token" :style="tokenStyle">
    <div class="box">
      <img :src="require(`@/static/images/icon-${this.tokenName}.svg`)" :alt="this.tokenName"/>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '../assets/scss/main';

.token {
  width: 130px;
  height: 130px;
  border: 17px solid blueviolet;
  box-sizing: border-box;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: white;
  box-shadow: 0 5px 0 blueviolet;
  cursor: pointer;
  transition: all 500ms ease-in-out;

  &:active {
    transform: scale(.9)
  }

  .box {
    box-shadow: 0 -5px 0 #bcc1d5;
    display: flex;
    justify-content: center;
    align-items: center;
    flex: 1;
    align-self: stretch;
    border-radius: 50%
  }
}
</style>

<script>
export default {
  name: 'PxToken',
  props: {
    tokenName: String
  },

  data: () => ({
    color: {
      paper: {
        base: '#516ef4',
        border: '#2543c3'
      },

      rock: {
        base: '#de3a5a',
        border: '#980e31'
      },

      scissors: {
        base: '#ecaB1e',
        border: '#c76c14'
      }
    }
  }),

  computed: {
    tokenStyle () {
      if (this.tokenName === 'rock') {
        return `border: 17px solid ${this.color.rock.base};
                  box-shadow: 0 5px 0 ${this.color.rock.border};`
      } else if (this.tokenName === 'paper') {
        return `border: 17px solid ${this.color.paper.base};
                  box-shadow: 0 5px 0 ${this.color.paper.border};`
      } else {
        return `border: 17px solid ${this.color.scissors.base};
                  box-shadow: 0 5px 0 ${this.color.scissors.border};`
      }
    }
  }
}
</script>
