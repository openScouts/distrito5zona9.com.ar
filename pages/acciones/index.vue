<template>
  <mdb-container>
    <h1 class="h1-responsive">Acciones</h1>
    <hr />

    <blockquote class="blockquote bq-primary">
      <p>
        En este espacio vas a poder encontrar las acciones que se hicieron y que
        están haciendo los/as scouts de nuestro distrito. En este espacio vas a
        poder encontrar las acciones que se hicieron y que se están haciendo
        los/as scouts de nuestro distrito. Animate e inspirá a otros scouts,
        registra tu acción.
      </p>
    </blockquote>
    <nuxt-link
      to="/acciones/enviar"
      class="stretched-link btn white-text success-color"
    >
      Registrar Nueva Accion
    </nuxt-link>
    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        class="embed-responsive-item"
        src="https://drive.google.com/embeddedfolderview?id=1_psj3ROTuBl1dJfmn9__hhz5K8Nuv4yi#list"
        allowfullscreen
      ></iframe>
    </div>
    <nuxt-link
      to="/acciones/enviar"
      class="stretched-link btn white-text success-color"
    >
      Registrar Nueva Accion
    </nuxt-link>
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
      title: "Acciones"
    };
  }
};
</script>
