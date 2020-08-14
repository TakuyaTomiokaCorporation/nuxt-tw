<template>
  <div>
    <div class="bg-black"></div>
    <header class="pc-menu header_menu">
      <ul>
        <li>
          <a href="/"><img src="@/assets/img/header/logo_w.png" alt="AVIOT" /></a>
        </li>
        <li>
          <a href="/products">PRODUCTS</a>
        </li>
        <li>
          <a href="/artist">ARTIST VOICE</a>
        </li>
        <li>
          <a href="/news">NEWS</a>
        </li>
        <li>
          <a href="/review">REVIEW</a>
        </li>
        <li>
          <a href="/media">MEDIA</a>
        </li>
        <li>
          <a href="/locations">STORE</a>
        </li>
        <li>
          <a href="/registration">WARRANTY</a>
        </li>
        <li>
          <a href="/support">SUPPORT</a>
        </li>
      </ul>
    </header>
  </div>
</template>

<style lang="scss">
  .bg-black {
  width: 100%;
  height:90px;
  background-color: #000;
}

header {
  background-color: rgba(0, 0, 0, 0.25);
  position: fixed;
  z-index: 100;
  width: 100%;
  height: 90px;
  top: 0;
  ul{
    letter-spacing: -0.4em;
    max-width: 1080px;
    margin: 27px auto;
    padding: 0;
    li{
      letter-spacing: normal;
      display: inline-block;
      list-style: none;
      margin: 0;
      padding: 0;
      vertical-align: middle;
      width: auto;
      margin-right: 20px;
      &:nth-child(n+2):hover{
        border-bottom: 1.5px solid #ffffff;
      }
    }
  }
}
// header ul {
//   letter-spacing: -0.4em;
//     max-width: 1080px;
//     margin: 27px auto;
//     padding: 0;
// }
// header ul li {
//   letter-spacing: normal;
//   display: inline-block;
//   list-style: none;
//   margin: 0;
//   padding: 0;
//   vertical-align: middle;
//   width: auto;
//   margin-right: 20px;
// }

// header ul li:nth-child(n+2):hover {
//   border-bottom: 1.5px solid #ffffff;
// }
header ul li:nth-child(1) {
  width: 250px;
}

header ul li a {
  display: block;
  font-size: 13px;
  line-height: 26px;
  text-decoration: none;
  color: #fff;
}
header ul li:nth-child(1) img {
  width: calc(100% - 100px);
}
header ul li:nth-child(n+2) a {
  font-family: 'Timmana', sans-serif;
  display: block;
  font-weight: bold;
  padding: 0 10px;
  margin-bottom: 2px;
}

@media screen and (max-width:960px) {
  .pc-menu ul {
    margin: 25px 10px;
  }
  .pc-menu li:nth-child(n+2) {
    display: none;
  }

}
</style>