<template>
  <footer
    v-if="$slidev.nav.currentPage !== 4">
    <div>
    J. Melles (BSH), H. Blitza (terrestris) | FOSSGIS | 16.03.2023
    </div>
    <div
      class="absolute bottom-0 -left-40px progress"
      :style="`width: ${Math.floor(
        100 * ($slidev.nav.currentPage / $slidev.nav.total)
      )}%;`"
    />
    <SlideCurrentNo
      v-if="$slidev.nav.currentPage !== 1"
      className="pageNumber"
    />
  </footer>
</template>

<style scoped>
footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 4vh;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  color: white;
  display: flex;
  background: #1b355a;
}

.progress {
  mix-blend-mode: soft-light;
  height: 0.5vh;
  background: white;
  transition: width 1s;
}

.pageNumber {
  position: absolute;
  padding: 10px;
  right: 0;
}
</style>