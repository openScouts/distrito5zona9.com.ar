<template>
  <mdb-container>
    <h1 class="h1-responsive font-weight-bold text-center my-5">
      Gestion de Insumos Distritales
    </h1>
    <nuxt-link
      to="/insumos/solicitar"
      class="stretched-link btn white-text success-color"
    >
      Solicitar Insumo
    </nuxt-link>
    <div class="row">
      <div class="col-lg-3">
        <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
          <img
            class="img-fluid"
            src="https://media.aws.alkosto.com/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/x/1/x1123h-1_1.jpg"
            alt="acta Distrito"
          />
          <a>
            <div class="mask rgba-white-slight"></div>
          </a>
        </div>
      </div>
      <div class="col-lg-9">
        <p>
          Como saben el Distrito posee un Proyector para favorecer las
          presentaciones, por ejemplo, para con los padres, eventos y para
          mejorar las actividades con los beneficiarios.
        </p>
        <p>
          Para organizar el uso del mismo, el consejo de distrito en 2012 acepto
          la propuesta de registrar en el calendario distrital los pedidos y es
          ahí donde se puede ver la disponibilidad del mismo.
        </p>
        <p>
          Por favor enviar un mail a comunicaciones@distrito5zona9.com.ar con
          copia a tu jefe/a de grupo Indicando el motivo del uso (Que rama lo
          usaría?, horarios? tipo de actividad?) para reservarlo y si en la
          fecha que lo precisan estuviese reservado por otro grupo veremos de
          forma más ágil la forma de tratar de coordinar entre quienes lo
          precisan para que todos puedan aprovechar los recursos.
        </p>
        <p>
          Lamentablemente esto no es siempre posible por lo cual ni bien tengan
          planificada la actividad avisen!
        </p>
        <h3>Dentro de la caja van a encontrar:</h3>
        * El proyector. <br />* El cable VGA. <br />* Una pantalla de 2 mtrs x
        1,80mtrs <br />* Un alargue con una zapatilla de 5 mtrs. para facilitar
        el uso.
        <br />
      </div>
      <nuxt-link
        to="/insumos/solicitar"
        class="stretched-link btn white-text success-color"
      >
        Solicitar Insumo
      </nuxt-link>
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
