<template>
  <mdb-container>
    <h1 class="h1-responsive">Biblioteca Distrital</h1>
    <hr />
    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        class="embed-responsive-item"
        src="https://drive.google.com/embeddedfolderview?id=1C3RzQ9XMmme1gWKQyBT7equTfAl-ZCQ_#list"
        allowfullscreen
      >
        Cargando datos ....
      </iframe>
    </div>
  </mdb-container>
</template>

<script>
import { mdbContainer } from "mdbvue";
export default {
  components: {
    mdbContainer
  },

  head() {
    return {
      title: "Biblioteca Distrital"
    };
  }
};
</script>
