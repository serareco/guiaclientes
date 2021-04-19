<template>
  <div id="app">
    <Nav />
    <div class="container-fluid my-md-4">
      <aside></aside>
      <main>
        <div id="content">          
          <div class="row" >
            <div class="col-md-4 col-sm-4" v-for="task in tasks" :key="task.id">
              <Task :datos="task" />
            </div>
          </div>
        </div>
      </main>
    </div>
    <Footer />
  </div>
</template>

<script>
import Nav from "./components/Nav";
import Task from "./components/Task";
import Footer from "./components/Footer";

export default {
  name: "App",
  data() {
    return {
      tasks: [
        {
          id: 1,
          description: "comprar pan",
          responsable: "Sergio",
          detail: "Ir al kiosco de enfrente a comprar pan",
        },
        {
          id: 2,
          description: "comprar leche",
          responsable: "Yanet",
          detail: "Ir al kiosco de enfrente a comprar leche",
        },
        {
          id: 3,
          description: "pasear el perro",
          responsable: "Sergio",
          detail: "sacar el perro a pasear.",
        },
      ],
    };
  },
  components: {
    Nav,
    Task,
    Footer,
  },
};
</script>

<style>
</style>
