<template>
  <div id="app">
    <nav
      class="navbar navbar-expand-lg navbar-light bg-light"
      style="background-color: #e3f2fd;"
    >
      <div class="container-fluid">
        <a class="navbar-brand" href="#">VacunaChain</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" href="#">Registrar Vacunación</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Consultar Registro</a>
            </li>
          </ul>
          <form class="d-flex">
            <input
              class="form-control me-2"
              type="search"
              placeholder="Search"
              aria-label="Search"
            />
            <button class="btn btn-outline-success" type="submit">
              Search
            </button>
          </form>
        </div>
      </div>
    </nav>

    <RegisterVaccine title="Registra un nuevo paciente" />
  </div>
</template>

<script>
import RegisterVaccine from "./components/RegisterVaccine.vue";
// import ListVaccine from "./components/ListVaccine.vue";

export default {
  name: "App",
  components: {
    RegisterVaccine,
    // ListVaccine
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
