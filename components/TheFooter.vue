<template>
  <div>
    <footer>
      <FooterSns />
      <p>&copy;AVIOT</p>
    </footer>
  </div>
</template>

<script>
import FooterSns from "@/components/FooterSns";
export default {
  components:{
    FooterSns,
  }
}
</script>

<style lang="scss">
footer{
  background-color: black;
  color: white;
  text-align: center;
}
</style>