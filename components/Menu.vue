<template>
  <mdb-navbar dark color="secondary-color-dark" position="top">
    <mdb-navbar-toggler>
      <mdb-navbar-nav>
        <mdb-nav-item to="/" active>Inicio</mdb-nav-item>
        <mdb-nav-item to="/familia">Familia</mdb-nav-item>
        <mdb-nav-item to="/acciones">Acciones</mdb-nav-item>
        <mdb-nav-item to="/nosotros">Nosotros</mdb-nav-item>
        <mdb-nav-item to="/comite">Comite</mdb-nav-item>
        <mdb-nav-item to="/grupos">Grupos</mdb-nav-item>
        <mdb-nav-item to="/biblioteca">Biblioteca</mdb-nav-item>
        <mdb-nav-item to="/calendario">Calendario</mdb-nav-item>
        <mdb-nav-item to="/insumos">Insumos</mdb-nav-item>
      </mdb-navbar-nav>
      <!--
      <mdb-navbar-nav right class="d-inline">
        <a href="https://www.facebook.com/zona9scoutsargentina" class="text-white p-2">
          <mdb-icon fab icon="facebook" />
        </a>
        <a href="https://github.com/caseroft/zona9.org.ar" class="text-white p-2">
          <mdb-icon fab icon="github" />
        </a>
        <a href="https://www.instagram.com/zona9saac/" class="text-white p-2">
          <mdb-icon fab icon="instagram" />
        </a>
      </mdb-navbar-nav>-->
    </mdb-navbar-toggler>

    <ul class="navbar-nav ml-auto nav-flex-icons">
      <li class="nav-item">
        <a
          class="nav-link"
          target="_blank"
          href="https://www.facebook.com/distrito5zona9saac/"
        >
          <i class="fab fa-lg fa-facebook-f"></i>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          target="_blank"
          href="https://github.com/caseroft/distrito5zona9.ar"
        >
          <i class="fab fa-lg fa-github"></i>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          target="_blank"
          href="https://www.instagram.com/distrito5zona9/"
        >
          <i class="fab fa-lg fa-instagram"></i>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          target="_blank"
          href="https://web.whatsapp.com/send?phone=5491154208465"
        >
          <i class="fab fa-lg fa-whatsapp"></i>
        </a>
      </li>
    </ul>
  </mdb-navbar>
</template>

<script>
import {
  mdbNavbar,
  mdbNavItem,
  mdbNavbarNav,
  mdbNavbarToggler,
  mdbDropdown,
  mdbDropdownItem,
  mdbDropdownMenu,
  mdbDropdownToggle,
  mdbInput,
  mdbBtn,
  mdbNavbarBrand
} from "mdbvue";
export default {
  name: "NavigationPage",
  components: {
    mdbNavbar,
    mdbNavItem,
    mdbNavbarNav,
    mdbNavbarToggler,
    mdbDropdown,
    mdbDropdownItem,
    mdbDropdownMenu,
    mdbDropdownToggle,
    mdbInput,
    mdbBtn,
    mdbNavbarBrand
  }
};
</script>
