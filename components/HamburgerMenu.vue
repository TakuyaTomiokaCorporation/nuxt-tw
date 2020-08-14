<template>
  <div>
    <div class="cp_offcm01 smt">
    <input type="checkbox" id="cp_toggle01">
    <label for="cp_toggle01"><span></span></label>
      <div class="cp_menu">
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
      </div>
    </div>
  </div>
</template>

<style>

#cp_toggle01 {
  display: none;
}
.cp_offcm01 {
	position: absolute;
	top: 20px;
	right: 20px;
	display: inline-block;
	z-index: 101;
	display: none;
}

.cp_offcm01 .cp_menu {
	position: fixed;
	top: 0;
	right: -100vw;
	width:100%;
	height: 100%;
	cursor: pointer;
	-webkit-transition: 0.53s transform;
	        transition: 0.53s transform;
	-webkit-transition-timing-function: cubic-bezier(.38,.52,.23,.99);
	        transition-timing-function: cubic-bezier(.38,.52,.23,.99);
	background-color: #000000;
	opacity: 0.8;
}
.cp_offcm01 .cp_menu ul {
	margin: 80px 0 0 0;
	padding: 0;
}
.cp_offcm01 .cp_menu li {
	list-style: none;
}

.cp_offcm01 .cp_menu li a {
	display: block;
	padding: 10px 20px;
	text-decoration: none;
	color: #ffffff;
}
.cp_menu ul li:nth-child(1) {
  margin-bottom: 20px;
}
.cp_menu ul li:nth-child(1) img {
  width: 150px;
}
.cp_offcm01 #cp_toggle01 {
	position: absolute;
	display: none;
	opacity: 0;
}
.cp_offcm01 #cp_toggle01:checked ~ .cp_menu {
	width:100%;
	-webkit-transform: translateX(-100vw);
	        transform: translateX(-100vw);
}


  
@media screen and (max-width:960px) {
  .cp_logo {
    display: block;
    position: absolute;
    top: 10px;
  }
  .cp_offcm01 {
    display: block;
    position: absolute;
    top: 0;
  }
  .cp_offcm01 #cp_toggle01 ~ label {
    display: block;
    margin-top: 20px;
    padding: 0;
    cursor: pointer;
    -webkit-transition: 0.5s transform;
    transition: 0.5s transform;
    -webkit-transition-timing-function: cubic-bezier(.61,-0.38,.37,1.27);
    transition-timing-function: cubic-bezier(.61,-0.38,.37,1.27);
    text-align: center;
    color: #333333;
    z-index: 1;
    position: fixed;
    right: 20px;
  }
  .cp_offcm01 #cp_toggle01 ~ label::before {
    font-family: 'FontAwesome';
    content: '\f0c9';
    font-size: 2em;
    color: #fff;
  }
  .cp_offcm01 #cp_toggle01:checked ~ label::before {
    content: '\f00d';
  } 
}
  
</style>