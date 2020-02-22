<template>
  <mdb-container>
    <section class="text-center">
      <h1 class="h1-responsive font-weight-bold my-5">
        Comite Ejecutivo Distrital
      </h1>

      <p class="note note-warning">
        Recuerden que el medio oficial de comunicación en nuestro distrito es
        mediante correo electrónico, y en el caso de que la normativa asociativa
        lo requiera (teniendo en cuenta lo acordado por el comité y el consejo
        de distrito), y que en algunas oportunidades será necesario que se
        presente documentación en soporte papel.
      </p>

      <mdb-row>
        <template v-for="integrante in comite">
          <mdb-col lg="3" md="6" class="mb-lg-0 mb-5" :key="integrante.codigo">
            <mdb-view hover cascade>
              <img
                class="img-fluid pt-2"
                :src="'/imagenes/comite/' + integrante.codigo + '.jpg'"
                :alt="integrante.nombre"
              />
            </mdb-view>
            <h5 class="font-weight-bold mt-4 mb-3">{{ integrante.nombre }}</h5>
            <p class="text-uppercase blue-text">{{ integrante.funcion }}</p>
            <p class="grey-text">{{ integrante.descripcion }}.</p>
            <p class="grey-text">
              <a :href="'mailto://' + integrante.correo">Contactar</a>
            </p>

            <hr />
          </mdb-col>
        </template>
      </mdb-row>
    </section>
  </mdb-container>
</template>

<script>
import comite from "../../config/comite.json";

import { mdbContainer, mdbRow, mdbCol, mdbView, mdbIcon } from "mdbvue";

export default {
  components: {
    mdbContainer,
    mdbRow,
    mdbCol,
    mdbView,
    mdbIcon
  },
  head() {
    return {
      title: "Comite Ejecutivo Distrital"
    };
  },
  data() {
    return {
      comite: comite.comite
    };
  }
};
</script>

<style scoped>
.rounded-circle {
  max-width: 150px;
}
</style>
