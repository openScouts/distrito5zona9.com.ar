<template>
  <!-- Footer -->
  <mdb-footer color="unique-color-dark" class="page-footer font-small pt-0">
    <div class="secondary-color-dark">
      <mdb-container class="text-left">
        <mdb-row class="py-4 d-flex align-items-center">
          <mdb-col md="6" lg="5" class="text-center text-md-left mb-4 mb-md-0">
            <h6 class="mb-0 white-text">
              ¡Conéctate con nosotros en las redes sociales!
            </h6>
          </mdb-col>
          <mdb-col md="6" lg="7" class="text-center text-md-right">
            <a
              class="fb-ic ml-0"
              href="https://www.facebook.com/distritocinco.zonanueve/"
            >
              <i class="fab fa-facebook fa-2x white-text mr-lg-4"></i>
            </a>
            <a class="ins-ic" href="https://www.instagram.com/distrito5zona9/">
              <i class="fab fa-instagram fa-2x white-text mr-lg-4"></i>
            </a>
            <a
              class="ins-ic"
              href="https://web.whatsapp.com/send?phone=5491154208465"
            >
              <i class="fab fa-whatsapp fa-2x white-text mr-lg-4"></i>
            </a>
            <a
              class="ins-ic"
              href="https://github.com/openscouts/distrito5zona9.com.ar"
            >
              <i class="fab fa-github fa-2x white-text mr-lg-4"></i>
            </a>
          </mdb-col>
        </mdb-row>
      </mdb-container>
    </div>
    <mdb-container class="mt-5 mb-4 text-center text-md-left">
      <mdb-row class="mt-3">
        <mdb-col md="4" lg="4" xl="4" class="mb-4">
          <h6 class="text-uppercase font-weight-bold">
            <strong>Nosotros</strong>
          </h6>
          <hr
            class="deep-purple accent-2 mb-4 mt-0 d-inline-block mx-auto"
            style="width: 60px"
          />
          <p>
            Formamos parte de un Movimiento Mundial de jóvenes, niños y adultos.
            Nuestro medio es la educación no formal, educación alternativa que
            potencie las capacidades de las personas, que no se agota en un
            tiempo o en un lugar específico y que se brinda en forma permanente.
          </p>
        </mdb-col>
        <mdb-col md="4" lg="4" xl="4" class="mb-4">
          <h6 class="text-uppercase font-weight-bold">
            <strong>Links Externos</strong>
          </h6>
          <hr
            class="deep-purple accent-2 mb-4 mt-0 d-inline-block mx-auto"
            style="width: 60px"
          />
          <p>
            <a href="https://www.scouts.org.ar/">Scouts de Argentina</a>
          </p>
          <p>
            <a href="https://www.scout.org/es"
              >Organización Mundial del Movimiento Scout</a
            >
          </p>
        </mdb-col>
        <mdb-col md="4" lg="4" xl="4" class="mb-4">
          <h6 class="text-uppercase font-weight-bold">
            <strong>Contacto</strong>
          </h6>
          <hr
            class="deep-purple accent-2 mb-4 mt-0 d-inline-block mx-auto"
            style="width: 60px"
          />
          <p>
            <i class="fas fa-home mr-3"></i> Nuestra Señora De La Merced 4624,
            Caseros, Buenos Aires, Sabados de 14:30 a 19:00 hs
          </p>
          <p>
            <i class="fas fa-envelope mr-3"></i> z9d5.director@scouts.org.ar
          </p>
        </mdb-col>
      </mdb-row>
    </mdb-container>
    <div class="footer-copyright text-center py-3">
      <mdb-container fluid>
        &copy; 2019 Copyright:
        <a href="https://caseroft.com.ar"
          >Desarrollador por Andres Lacquaniti</a
        >
      </mdb-container>
    </div>
  </mdb-footer>
  <!-- Footer -->
</template>
<script>
import { mdbFooter, mdbContainer, mdbRow, mdbCol } from "mdbvue";
export default {
  name: "FooterPage",
  components: {
    mdbFooter,
    mdbContainer,
    mdbRow,
    mdbCol
  }
};
</script>
