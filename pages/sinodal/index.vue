<template>
  <mdb-container>
    <h1 class="h1-responsive">Sinodal</h1>
    <hr />

    <blockquote class="blockquote bq-primary">
      Ser Sinodal:
      <p>
        Nuestras actividades y acciones son posible con la ayuda de otros/as.
        Por eso podes registrarte como sinodal y te puedan contactar los grupos
        scouts de nuestro distrito.
      </p>
    </blockquote>

    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        src="https://docs.google.com/forms/d/e/1FAIpQLSc5_Y-PnoQdgxU0Y8OyFwvmjdBjhOjME0sSCzCnnWdT13fbcA/viewform?embedded=true"
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

  head() {
    return {
      title: "Quienes Somos"
    };
  }
};
</script>
