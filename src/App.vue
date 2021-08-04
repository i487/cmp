<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style-type: none;
  font-family: 'Work Sans', sans-serif;
}

.container {
  padding: 0 15px;
  max-width: 1200px;
  margin: 0 auto;
}
.btn {
  font-weight: bold;
  font-size: 16px;
  line-height: 26px;
  color: #F07566;
  padding: 10px 28px;
  border: 1px solid rgba(240, 117, 102, 0.236809);
  border-radius: 6px;
  background: transparent;
  cursor: pointer;
  &_color_white {
    color: white;
    background: #F07566;
  }
}
</style>
