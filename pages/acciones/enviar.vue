<template>
  <mdb-container>
    <h1 class="h1-responsive font-weight-bold text-center my-5">
      Envio de Acciones realizadas por los diferentes ramas del distrito
    </h1>

    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        src="https://docs.google.com/forms/d/e/1FAIpQLScn9VqrtPD4TIuBlmz1y49IV4LPkKKvweDgUkNVRSriprkkrg/viewform?embedded=true"
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
      title: "Envio de Acciones"
    };
  }
};
</script>
