<template>
  <div>
    <div class="flex flex-col my-12 space-y-2 md:space-y-4">
      <h1 class="text-center font-bold pb-4 text-lg sm:text-2xl xl:text-3xl 2xl:text-5xl">Escolha uma página</h1>
      <p><nuxt-link to="/photogrid">PhotoGrid</nuxt-link></p>
      <p><nuxt-link to="/login">Formulário de login</nuxt-link></p>
      <p><nuxt-link to="/endereco">Formulário de endereço</nuxt-link></p>
      <p><nuxt-link to="/api">API</nuxt-link></p>
    </div>
  </div>
</template>

<style scoped>
p{
  padding: 1rem 2rem;
  border: 1px solid #333;
  border-radius: 1rem;
  background-color: #bee6d6;
  text-align: center;
  font-size: 1rem;
}

p:hover, p:focus{
  cursor: pointer;
  background-color: #c1bee6;
}

@media(min-width: 640px){
  p{
    padding: 1rem 3rem;
    font-size: 1.2rem;
  }
}

@media(min-width: 768px){
  p{
    font-size: 1.3rem;
  }
}

@media(min-width: 1024px){
  p{
    font-size: 1.5rem;
  }
}

@media(min-width: 1280px){
  p{
    font-size: 1.7rem;
  }
}

@media(min-width: 1536px){
  p{
    font-size: 2rem;
  }
}
</style>