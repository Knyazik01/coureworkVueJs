<template>
  <footer class="footer">
    <div class="footer_left">
      <FooterLink :link-content="'github.png'" link-url="https://github.com/Knyazik01" link-type="img" link-label="Knyazik01" new-tab/>
    </div>

    <div class="footer_right">
      <FooterLink :link-content="'\u00A9 Viktor Kniahnitskyi'"/>
    </div>
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

<style lang="scss" scoped>

.footer {
  margin: 10px 15px 0 15px;
  padding: 10px;
  border-top: 2px dashed white;
  display: flex;
  flex-direction: row;
  font-size: 1.2em;
  justify-content: space-between;
  align-items: center;
}

</style>