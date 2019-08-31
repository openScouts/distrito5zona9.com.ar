<template>
  <mdb-container>
    <h1 class="h1-responsive font-weight-bold text-center my-5">Solicitud de Insumos Distritales</h1>
    <div class="row">
      <div class="col-lg-9">
        <mdb-row>
            <mdb-col>
              <mdb-input label="Your name" v-model="fields.name" required />
            </mdb-col>
            <mdb-col>
              <mdb-input type="email" label="Your email" v-model="fields.email" required />
            </mdb-col>
          </mdb-row>
          <mdb-row>
            <mdb-col>
              <mdb-input label="Subject" v-model="fields.subject" required />
            </mdb-col>
          </mdb-row>
          <mdb-row>
            <mdb-col>
              <mdb-input
                type="textarea"
                label="Your message"
                v-model="fields.message"
                required
              />
            </mdb-col>
          </mdb-row>
        </mdb-col>
        <mdb-btn color="primary" type="submit" class="float-left">Solicitar</mdb-btn>
      </div>
    </div>
  </mdb-container>
</template>



<script>
  import {
    mdbContainer,
    mdbInput,
    mdbCard,
    mdbCardHeader,
    mdbCardTitle,
    mdbCardText,
    mdbCardBody,
    mdbIcon,
    mdbBtn,
    mdbRow,
    mdbCol
  } from "mdbvue";

  export default {
    components: {
      mdbContainer,
      mdbInput,
      mdbCard,
      mdbCardHeader,
      mdbCardTitle,
      mdbCardBody,
      mdbCardText,
      mdbIcon,
      mdbBtn,
      mdbRow,
      mdbCol
    },
    data() {
      return {
        fields: {
          name: "",
          email: "",
          subject: "",
          message: ""
        }
      };
    },
      head() {
        return {
          title: "Quienes Somos"
        };
      }
  };
</script>
