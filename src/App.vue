<script setup>
  import Emojis from './components/Emojis.vue';
</script>

<template>
  <header>
    <div>
      <h1>emojis-web-jct</h1>
    </div>
  </header>
  <nav>
    <ul>
      <ol><a href="http://">🌸 Inicio</a></ol>
      <ol><a href="http://">🔥 Favoritos</a></ol>
      <ol><a href="http://">📱 Por categorías</a></ol>
      <ol><a href="http://">✨ Combinaciones</a></ol>
      <ol><a href="http://">🆕 Nuevos</a></ol>
    </ul>
  </nav>
  <main>
    <section>
      <hr>
      <h2>🌸 Inicio</h2>
      <br>
      <p>Bienvenido a mi colección personal de emojis ✨ Aquí guardo todos mis favoritos, desde los más
        <br>
        cute hasta los más útiles. Mi rincón emoji donde encuentro el perfecto para cada momento jajaja.
      </p>
    </section>
    <hr>
    <section>
      <h2>🔥 Favoritos</h2>
      <br>
      <p>
        Mis emojis de siempre, los que nunca fallan y siempre uso en mis mensajes. Mi selección premium
        <br> de los más expresivos y que me representan jajaja.
      </p>
      <br>
      <div class="div-emoji">
        <div class="dv-emoji">
          <Emojis/> 
        </div>
      </div>
    </section>
    <hr>
    <section>
      <h2>📱 Por categorías</h2>
      <br>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores nulla deleniti nisi quisquam sed
        <br> eos perspiciatis beatae vitae explicabo odit, voluptates quam, repellat iste consequatur harum
        <br> ad vel. Odio, voluptates.
      </p>
    </section>
    <section>
      <h2>✨ Combinaciones</h2>
      <br>
      <p>
        Todos mis emojis organizaditos por temas para encontrar exactamente lo que necesitas. Desde
        <br> caritas hasta objetos, todo súper clasificado y fácil de navegar.
      </p>
    </section>
    <section>
      <h2>🆕 Nuevos</h2>
      <br>
      <p>Aquí están mis combos favoritos de emojis que quedan perfectos juntos. Esas mezclas que le dan
        <br> más personalidad y flow a cualquier mensaje jajaja.
      </p>
    </section>
  </main>
  <footer>
    <small>Footer</small>
  </footer>
  <Index />
</template>

<style scoped></style>
