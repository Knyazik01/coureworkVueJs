<template>
  <footer>
    <FooterLink link-content="Knyazik01" link-url="#"/>
    <FooterLink :link-content="'github.png'" link-url="#" link-type="img"/>
    <FooterLink :link-content="'\u00A9 Viktor Kniahnitskyi'"/>
  </footer>
</template>

<script>
import FooterLink from "@/components/footer/FooterLink";

export default {
  name: "Footer",
  components: {
    FooterLink,
  }
}
</script>

<style scoped>

</style>