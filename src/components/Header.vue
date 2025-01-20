<template>
  <div class="header">
    <div class="header__logo">
      <img src="https://i.imgur.com/Fm7jYRr.png" alt="">
    </div>
  </div>
</template>
<script>

export default {
  name: 'Header',
  props: {
    type: {
      type: String,
      default: 'text'
    },
    text: {
      type: String,
      default: 'Ingresar'
    }
  },

  methods: {
    click() {
      this.$emit('click')
    }
  }
}
</script>

<style>
.header {
  padding: 0px 30px;
  background-color: #00adb3;
  box-shadow: 0px 0px 20px 6px rgba(0, 0, 0, 0.05);
  width: 100vw;
  height: 40vh;
  z-index: 3;
  display: flex;
  justify-content: center;
}

.header__logo {
  margin: 7px 0 0 20px;
  width: 250px;
  object-fit: cover;
  display: flex;
  justify-content: center;
}

img {
  width: 100%;
}

.header__title {
  margin-left: .75rem;
  font-size: 25px;
  font-weight: bold;
  color: #ff8f00;
  display: flex;
  align-items: center;
  padding-top: 0.1rem
}
</style>
