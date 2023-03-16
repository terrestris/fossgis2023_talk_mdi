<template>
  <header
    v-if="$slidev.nav.currentPage === 1"
    >
    <img src="/mdide_logo_white.png">
    <img src="/terrestris_logo_invers.svg"
    >
  </header>
    <div
    class="header2"
    v-if="$slidev.nav.currentPage != 1 && $slidev.nav.currentPage != 4 && $slidev.nav.currentPage != 7"
    >
    <img src="/mdide_logo.png">
    <img src="/terrestris-logo-normal.svg">
  </div>
</template>

<style>
header {
  position: fixed;
  top: 0;
  width: 100%;
  height: 5vh;
  flex-direction: row;
  color: white;
  display: flex;
  background: #1b355a;
  justify-content: space-between;
}
.header2 {
  position: fixed;
  top: 0;
  width: 100%;
  height: 5vh;
  flex-direction: row;
  color: white;
  display: flex;
  background: white;
  justify-content: space-between;
}

</style>