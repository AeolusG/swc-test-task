<template>
  <nav class="sidenav">
    <h1 class="title">Demo Test</h1>
    <button type="button">
      <img src="../assets/images/user.svg" alt="profile" />
      <span class="visibility">Profile</span>
    </button>

    <button type="button" class="active">
      <img src="../assets/images/rim.svg" alt="vehicles" />
      <span class="visibility">Vehicles</span>
    </button>
    <button type="button">
      <img src="../assets/images/settings.svg" alt="vehicles" />
      <span class="visibility">Setting</span>
    </button>
  </nav>
</template>

<style lang="scss" scoped>
@import '../assets/fonts/fonts.css';
.title {
  color: #f1f1f1;
  font-family: 'DMSans', sans-serif;
  font-weight: 700;
  font-size: 24px;
  margin: 0;
  text-align: center;
  margin-bottom: 80px;
}
.sidenav {
  height: 100%;
  width: 260px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #282828;
  overflow-x: hidden;
  padding-top: 20px;
  background-image: url('../assets/images/waves.svg');
  background-repeat: no-repeat;
  background-position-y: bottom;
  img {
    padding-right: 10px;
  }
  button {
    padding: 12px 8px;
    font-size: 16px;
    color: rgba(255, 255, 255, 0.4);
    display: flex;
    font-family: 'DMSans', sans-serif;
    font-weight: 500;
    margin-bottom: 20px;
    border-right: none;
    border-top: none;
    border-bottom: none;
    border-left: 2px solid rgba(255, 255, 255, 0);
    background-color: rgba(255, 255, 255, 0);
    min-width: 260px;
  }
  button:hover {
    color: #f1f1f1;
    background-color: rgba(255, 255, 255, 0.2);
    border-right: none;
    border-top: none;
    border-bottom: none;
    border-left: solid 2px rgba(217, 14, 50, 1);
  }
  .active {
    color: #f1f1f1;
    background-color: rgba(255, 255, 255, 0.2);
    border-left: solid 2px rgba(217, 14, 50, 1);
  }
}

.visibility {
  display: inline;
}
@media (min-width: 768px) and (max-width: 991px) {
  .sidenav {
    height: 100%;
    width: 100px;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;
    background-color: #282828;
    overflow-x: hidden;
    padding-top: 20px;
  }
  img {
    padding-left: 30px;
  }
  .visibility {
    opacity: 0;
  }
  a:hover {
    img {
      display: none;
    }
    .visibility {
      display: block;
      opacity: 1;
      transition: 2s;
      margin: auto;
    }
  }
}
@media (max-width: 768px) {
  .sidenav {
    height: 100%;
    width: 100px;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;
    background-color: #282828;
    overflow-x: hidden;
    padding-top: 20px;
  }
  img {
    padding-left: 30px;
  }
  .visibility {
    opacity: 0;
  }
  a:hover {
    img {
      display: none;
    }
    .visibility {
      display: block;
      opacity: 1;
      transition: 2s;
      margin: auto;
    }
  }
}
</style>
