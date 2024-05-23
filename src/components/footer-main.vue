<template>
  <footer>
    <p>Seu Nome</p>
    <p>Contato: seuemail@exemplo.com</p>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#objetivos">Objetivos</a></li>
        <li><a href="#reciclagem">Reciclagem</a></li>
        <li><a href="#coletivismo">Coletivismo</a></li>
        <li><a href="#conscientizacao">Conscientização</a></li>
      </ul>
    </nav>
  </footer>
</template>

<script>
export default {
};
</script>

<style>
footer {
  background: #2e7d32;
  color: white;
  padding: 1rem;
  text-align: center;
}

footer nav ul {
  list-style: none;
  padding: 0;
}

footer nav ul li {
  display: inline;
  margin: 0 0.5rem;
}

footer nav ul li a {
  color: white;
  text-decoration: none;
}

@media (max-width: 768px) {
  footer nav ul {
    flex-direction: column;
  }

  footer nav ul li {
    display: block;
    margin: 0.5rem 0;
  }
}
</style>
