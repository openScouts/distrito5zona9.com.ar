<template>
  <mdb-container>
    <h1 class="h1-responsive font-weight-bold text-center my-5">
      Gestion de Insumos Distritales
    </h1>
    <blockquote class="blockquote bq-primary ">
      <p>
        Como saben el Distrito, tiene algunos materiales que son para uso de
        todos.
        <br />
        Para organizar el uso de los mismos, el consejo de distrito en 2012
        acepto la propuesta de registrar en el calendario distrital los pedidos
        y es ahí donde se puede ver la disponibilidad de dichos elementos.
        <br />
        <strong>
          ¡Lamentablemente esto no es siempre posible por lo cual, ni bien
          tengan planificada la actividad avisen!
        </strong>
      </p>
    </blockquote>
    <h3 class="text-info">
      !Favor tener a bien pensar que ademas de ir a retirar los materiales hay
      que devolverlos!
    </h3>
    <hr />

    <nuxt-link
      to="/insumos/solicitar"
      class="stretched-link btn white-text success-color"
    >
      Solicitar Insumo
    </nuxt-link>

    <hr />
    <h4 class="">
      Insumos Disponibles
    </h4>
    <div class="row">
      <div class="col-lg-3">
        <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
          <img class="img-fluid" src="/imagenes/insumos/proyector.jpg" />
          <a>
            <div class="mask rgba-white-slight"></div>
          </a>
        </div>
      </div>
      <div class="col-lg-9">
        <p>
          Contamos con un proyector con conexion VGA y una Pantalla de pie de
          2x1,5 para facilitar las presentaciones realizadas en los grupos.
        </p>
      </div>
    </div>
    <hr />
    <div class="row">
      <div class="col-lg-3">
        <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
          <img class="img-fluid" src="/imagenes/insumos/gacebo.webp" />
        </div>
      </div>
      <div class="col-lg-9">
        <p>
          Contamos con un gazebo de 3 x 3 con paredes de mosquiteros.
        </p>
        <br />
      </div>
    </div>
    <hr />
    <div class="row">
      <div class="col-lg-3">
        <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
          <img class="img-fluid" src="/imagenes/insumos/iglu.jpg" />
        </div>
      </div>
      <div class="col-lg-9">
        <p>
          Contamos con una Carpa Iglu de 4 personas, para facilitar tus
          actividades en contacto con la naturaleza.
        </p>
        <br />
      </div>
    </div>
    <hr />
    <div class="row">
      <div class="col-lg-3">
        <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
          <img class="img-fluid" src="/imagenes/insumos/antiparras.jpg" />
        </div>
      </div>
      <div class="col-lg-9">
        <p>
          Contamos con 45 pares de lentes de seguridad para realizar actividades
          tomando los recaudos necesarios para que nuestras actividades
          contemplen el cuidado fisico de quienes las desarrollan.
        </p>
        <br />
      </div>
    </div>
    <hr />

    <nuxt-link
      to="/insumos/solicitar"
      class="stretched-link btn white-text success-color"
    >
      Solicitar Insumo
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
      title: "Quienes Somos"
    };
  }
};
</script>
