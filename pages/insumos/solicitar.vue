<template>
  <mdb-container>
    <h1 class="h1-responsive font-weight-bold text-center my-5">
      Solicitud de Insumos Distritales
    </h1>
    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        src="https://docs.google.com/forms/d/e/1FAIpQLSdRRC6XcQTBzr0jQ5hwJpR40t_E7CU0Pd8vRB8E2qthSZhihA/viewform?embedded=true"
        allowfullscreen
      >
        Cargando…
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
  data() {
    return {};
  },
  head() {
    return {
      title: "Quienes Somos"
    };
  }
};
</script>
