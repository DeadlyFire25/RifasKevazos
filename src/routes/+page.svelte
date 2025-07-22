<script>
  import Header from '../components/Header.svelte';
</script>


<Header></Header>
<main class="bg-main text-white h-screen">
  <div class="relative w-full h-auto">
    <img
      src="home/rifa2.jpg"
      alt="Sorteo"
      class="w-full h-[600px] object-center object-cover rounded-lg"
    />
    <div class="absolute inset-0 bg-opacity flex flex-col items-center justify-center text-center text-white px-4">
      <h2 class="text-2xl md:text-4xl font-bold mb-2">PARTICIPA Y GANA</h2>
      <p class="text-lg md:text-2xl font-bold mb-2">SORTEOS ENTRE AMIGOS EN BASE A LA LOTERIA NACIONAL</p>
      <p class="text-md md:text-xl mb-4">¡ARRIESGA POCO Y GANA MUCHO!</p>
      <a class="bg-secondary px-8 py-1 my-8 rounded-2xl text-lg" href="/">Ver boletos</a>
      <a class="bg-secondary px-8 py-1 rounded-2xl text-lg" href="/home">Ver sorteos valorant</a>
    </div>
  </div>
</main>