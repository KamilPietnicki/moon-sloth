<template>
  <div class="header">
    <div class="logo">
      <img src="~/assets/sloth-small.png" />
    </div>

    <div class="menu">
      <a href="http://">Telegram</a>
      <a href="http://">Twitter</a>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss">
.header {
  display: block;
  position: relative;

  width: 100%;
  height: 180px;
  margin-bottom: 160px;
  padding-top: 80px;

  .logo {
    display: block;
    position: absolute;

    left: 0;
    top: 50%;
    transform: translateY(-50%);

    img {
      width: auto;
      height: 100px;
    }
  }

  .menu {
    display: block;
    position: absolute;

    right: 0;
    top: 50%;
    transform: translateY(-50%);

    a {
      text-transform: uppercase;
      font-size: 16px;

      color: #526488;
      text-decoration: none;
      margin-left: 20px;

      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>