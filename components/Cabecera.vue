<template>
  <div class="jumbotron jumbotron-fluid card card-image secondary-color-dark p-0">
    <img src="/imagenes/principal.svg" class="img-fluid" alt />

    <!--
    <div class="container">
      <h2 class="display-4">Fluid jumbotron</h2>
      <p
        class="lead"
      >This is a modified jumbotron that occupies the entire horizontal space of its parent.</p>
    </div>-->
  </div>
</template>


<style scoped>
.jumbotron {
  margin-top: 54px;
}
</style>


<script>
import { mdbCard, mdbBtn } from "mdbvue";
export default {
  name: "JumbotronPage",
  components: {
    mdbCard,
    mdbBtn
  }
};
</script>