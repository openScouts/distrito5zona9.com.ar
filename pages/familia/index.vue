<template>
  <mdb-container>
    <h1 class="h1-responsive">Familia</h1>
    <hr />

    <blockquote class="blockquote bq-primary">
      <p>
        Todas las preguntas que ustedes como familia tengan merecen ser respondidas, veamos antes si no es una de las preguntas que alguien ha tenido antes. Sino no dudes en consultarnos.
        Preguntas frecuentes
        Dejamos los documentos que pueden ser de utilidad para los familiares de los jóvenes que ya se encuentran afiliados a Scouts de Argentina y realizan actividad en un grupo scout
      </p>
    </blockquote>

    <div class="embed-responsive embed-responsive-16by9">
      <iframe
        class="embed-responsive-item"
        src="https://drive.google.com/embeddedfolderview?authuser=0&id=1srRXIqeRsWNf407NsgP4F8XNm4pS7eG7#list"
        allowfullscreen
      ></iframe>
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