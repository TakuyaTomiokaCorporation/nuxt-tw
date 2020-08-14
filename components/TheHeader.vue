<template>
  <div>
    <HamburgerMenu />
    <HeaderNav />
  </div>  
</template>

<script>
import HeaderNav from "@/components/HeaderNav";
import HamburgerMenu from "@/components/HamburgerMenu";

export default {
  components: {
    HeaderNav,
    HamburgerMenu,
  }
}
</script>