<template>
  <mdb-container>
    <h1 class="h1-responsive">Grupos del Distrito 5</h1>
    <hr />

    <template v-for="grupo in grupos">
      <div :key="grupo.id">
        <mdb-row>
          <mdb-col lg="5" xl="4">
            <mdb-view class="mb-lg-0 mb-4">
              <img
                class="img-fluid"
                :src="'/imagenes/panuelos/' + grupo.id + '.svg'"
                alt="Sample image"
              />
              <a>
                <mdb-mask overlay="white-slight" waves />
              </a>
            </mdb-view>
          </mdb-col>
          <mdb-col lg="7" xl="8">
            <h3 class="font-weight-bold mb-3 p-0">
              <strong>{{ grupo.nombre }} -- Nro {{ grupo.id }}</strong>
            </h3>
            <!--
          <p class="dark-grey-text">
            Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere
            possimus, omnis voluptas assumenda est, omnis dolor repellendus et aut officiis debitis cum soluta nobis est eligendi
            placeat facere aut rerum.
            </p>-->
            <ul class="list-group list-group-flush">
              <li class="list-group-item" v-if="grupo.fundacion">
                Fundado el {{ grupo.fundacion }}
              </li>
              <li class="list-group-item">
                Direccion {{ grupo.direccion }}

                <a
                  class="btn btn-info btn-sm"
                  target="_blank"
                  :href="
                    'https://www.google.com.ar/maps/dir/' +
                      grupo.Latitud +
                      ',' +
                      grupo.Longitud
                  "
                >
                  Ir
                </a>
              </li>
              <li class="list-group-item">
                localidad de {{ grupo.localidad }}
              </li>
              <li class="list-group-item">Partido de {{ grupo.partido }}</li>
              <li class="list-group-item">
                <a :href="'mailto://grupo' + grupo.id + '@scouts.org.ar'">
                  Contactar
                </a>
              </li>
              <!--
              <li class="list-group-item" v-if="grupo.distrito != 0 ">Distrito {{grupo.distrito}}</li>
            --></ul>
          </mdb-col>
        </mdb-row>
        <hr class="my-5" />
      </div>
    </template>
  </mdb-container>
</template>

<script>
import Grupos from "../../config/grupos.json";
import {
  mdbContainer,
  mdbRow,
  mdbCol,
  mdbCard,
  mdbCardBody,
  mdbMask,
  mdbIcon,
  mdbView,
  mdbBtn
} from "mdbvue";
export default {
  components: {
    mdbContainer,
    mdbRow,
    mdbCol,
    mdbCard,
    mdbCardBody,
    mdbMask,
    mdbIcon,
    mdbView,
    mdbBtn
  },

  head() {
    return {
      title: "Grupos del Distrito 5"
    };
  },
  data() {
    return {
      grupos: Grupos
    };
  },
  methods: {}
};
</script>
