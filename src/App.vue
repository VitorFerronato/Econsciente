<template>
  <div id="app">
    <Header-main />
    <section id="home" class="hero">
      <div class="hero-content">
        <h1>Econsciente</h1>
        <p>Pequena descrição sobre o site.</p>
      </div>
    </section>
    <main>
      <section id="objetivos">
        <Objectives-section />
      </section>
      <section id="reciclagem">
        <Recyclin-section />
      </section>
      <section id="coletivismo">
        <Coletivism-section />
      </section>
      <section id="conscientizacao">
        <Consientization-section />
      </section>
    </main>
    <Footer-main />
  </div>
</template>
<script>
import HeaderMain from "./components/header-main.vue";
import ObjectivesSection from "./components/objectives-section.vue";
import RecyclinSection from "./components/recyclin-section.vue";
import ColetivismSection from "./components/coletivism-section.vue";
import ConsientizationSection from "./components/consientization-section.vue";
import FooterMain from "./components/footer-main.vue";

export default {
  name: "App",
  components: {
    HeaderMain,
    ObjectivesSection,
    RecyclinSection,
    ColetivismSection,
    ConsientizationSection,
    FooterMain,
  },
};
</script>

<style>
body,
html {
  margin: 0;
  padding: 0;
  font-family: "Roboto", sans-serif;
  background-color: #f5f5f5;
  color: #333;
  scroll-behavior: smooth;
}

#app {
  text-align: center;
}

.hero {
  background-image: url("https://images.unsplash.com/photo-1701637342541-6734100cb333?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D");
  background-size: cover;
  background-position: center;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

.hero-content h1 {
  font-size: 4rem;
  margin: 0;
}

.hero-content p {
  font-size: 1.5rem;
  margin: 0;
}

main {
  padding: 2rem;
}

section {
  margin: 2rem 0;
  padding: 2rem;
  background: white;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

h2 {
  color: #2e7d32; /* Verde ambiental */
}

/* Estilos responsivos */
@media (max-width: 768px) {
  .hero-content h1 {
    font-size: 2.5rem;
  }

  .hero-content p {
    font-size: 1rem;
  }

  section {
    margin: 1rem 0;
    padding: 1rem;
  }
}

@media (max-width: 480px) {
  nav ul {
    flex-direction: column;
  }

  nav ul li {
    margin: 0.5rem 0;
  }

  .hero-content h1 {
    font-size: 2rem;
  }

  .hero-content p {
    font-size: 0.875rem;
  }

  section {
    margin: 1rem 0;
    padding: 1rem;
  }
}
</style>
