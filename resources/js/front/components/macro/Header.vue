<template>
  <header class="d-flex justify-content-between align-items-center">
      <a href="/" >
        <div class="logo d-flex align-items-center">
            <img src="/storage/uploads/logo-deliveroo.png" alt="logo deliveroo">
            <span class="header_title">deliveboo</span>
        </div>
      </a>

    <a href="/admin/home">
      <button class="btn btn-main">
        Area riservata
      </button>
    </a>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang='scss' scoped>

header {

  height: 80px;
  background-color: var(--white);
  padding: 15px;
  box-shadow: rgba(60, 64, 67, 0.1) 0px 1px 6px 0px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 99;

  .logo{
    height: 30px;
    cursor: pointer;

    img {
      height: 100%;
    }

    .header_title {
      font-size: 1.15rem;
      font-weight: bold;
      font-family: 'Poppins', sans-serif;
      color: var(--main-color);
      margin-left: 5px;
    }
  }
}

@media screen and (min-width: 576px) {
  .btn-main {
    font-size: 1rem;
    padding: 10px 15px;
  };
}

@media screen and (min-width: 1400px) {
  header {
    padding: 15px 50px;
  }
}
</style>