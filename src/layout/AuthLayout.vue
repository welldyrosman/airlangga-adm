<template>
  <div class="main-content bg-default">
    <!-- Navbar -->
    <!-- Header -->
    <div
      style="background: linear-gradient(87deg, #1a6fff 0, #171a4d 100%) !important"
      class="header bg-gradient-green py-lg-2"
    >
      <div class="container">
        <div class="header-body text-center mb-7">
          <div class="row justify-content-center">
            <div class="col-lg-5 col-md-6">
              <img
                style="max-height: 170px; margin-bottom: 50px; margin-top: 50px"
                :src="logo"
                class="navbar-brand-img"
                alt="..."
              />
            </div>
          </div>
        </div>
      </div>
      <div class="separator separator-bottom separator-skew zindex-100">
        <svg
          x="0"
          y="0"
          viewBox="0 0 2560 100"
          preserveAspectRatio="none"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
        >
          <polygon class="fill-default" points="2560 0 2560 100 0 100"></polygon>
        </svg>
      </div>
    </div>
    <!-- Page content -->
    <div class="container mt--8 pb-5">
      <router-view></router-view>
    </div>
    <footer class="py-8"></footer>
  </div>
</template>
<script>
export default {
  name: "auth-layout",
  props: {
    logo: {
      type: String,
      default: "img/brand/travel.png",
      description: "Sidebar app logo",
    },
  },
  data() {
    return {
      year: new Date().getFullYear(),
      showMenu: false,
    };
  },
};
</script>
<style></style>
