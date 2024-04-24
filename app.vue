<template>
  <div id="app">
    <div class="header">
      <div class="inner-header flex">
        <div class="wifi">
          <div class="qrcode">
            <NuxtImg src="/wifi.png" />
          </div>
        </div>
      </div>
      <Waves />
    </div>

    <div class="content flex">
      <p>pretty fly for a wifi</p>
    </div>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400&display=swap');

body {
  margin: 0;
}

h1 {
  font-family: 'Lato', sans-serif;
  font-weight: 300;
  letter-spacing: 2px;
  font-size: 48px;
}

p {
  font-family: 'Lato', sans-serif;
  letter-spacing: 1px;
  font-size: 14px;
  color: #333333;
}

.header {
  position: relative;
  text-align: center;
  background: linear-gradient(60deg, rgba(84, 58, 183, 1) 0%, rgba(0, 172, 193, 1) 100%);
  color: white;
}

.inner-header {
  height: 65vh;
  width: 100%;
  margin: 0;
  padding: 0;
}

.flex {
  /*Flexbox for containers*/
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.content {
  position: relative;
  height: 20vh;
  text-align: center;
  background-color: white;
}

.wifi {
  background-color: #6067f0;
  width: 350px;
  height: 350px;
  border-radius: 13px;
  box-shadow: 2px 4px 20px -3px #555555a8;
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
  box-sizing: border-box;
}

.qrcode {
  margin: auto;
  margin-top: 40px;
  margin-bottom: 70px;
  background: #fff;
  width: 250px;
  padding: 7px;
  border-radius: 7px;
  box-shadow: 0 4px 10px 0px #55555596;
}

.qrcode > img {
  opacity: 0.8;
  width: 250px;
}

/*Shrinking for mobile*/
@media (max-width: 768px) {
  .content {
    height: 30vh;
  }
}
</style>
