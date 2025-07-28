<script>
  import Header from '../components/Header.svelte';
  import { AccordionItem, Accordion } from "flowbite-svelte";

</script>


<Header/>

<main class="bg-main text-white h-screen flex flex-col">
  <div class="relative w-full h-auto">
    <img
      src="home/honda.jpg"
      alt="Sorteo"
      class="w-full h-64 md:h-[550px] object-cover"
    />
    <div class="absolute inset-0 bg-opacity flex flex-col items-center justify-center text-center text-white px-4">
      <h2 class="text-2xl md:text-4xl font-bold mb-2">PARTICIPA Y GANA</h2>
      <p class="text-lg md:text-2xl font-bold mb-2">SORTEOS ENTRE AMIGOS EN BASE A LA LOTERIA NACIONAL</p>
      <p class="text-md md:text-xl mb-4">¡ARRIESGA POCO Y GANA MUCHO!</p>
      <a class="bg-secondary px-8 py-1 my-8 rounded-2xl text-lg" href="/">Ver boletos</a>
      <a class="bg-secondary px-8 py-1 rounded-2xl text-lg" href="/home">Ver sorteos valorant</a>
    </div>
  </div>

  
  <div class="flex justify-center items-center flex-col mt-8">
    <div class="w-1/2">
<Accordion class="bg-main" activeClass="bg-gray-700" inactiveClass
="bg-gray-600" transitionType="slide" transitionDuration={300}>
  <AccordionItem open class="text-2xl secondary-color">
    {#snippet header()}¿CÓMO SE ELIGE A LOS GANADORES?{/snippet}
    <p class="mb-2 text-gray-500 dark:text-gray-400">Todos nuestros sorteos se realizan en base a la Lotería Nacional para la Asistencia Pública mexicana.​</p>
  </AccordionItem>
  <AccordionItem class="text-2xl secondary-color">
    {#snippet header()}¿QUÉ SUCEDE CUANDO EL NÚMERO GANADOR ES UN BOLETO NO VENDIDO?{/snippet}
    <p class="mb-2 text-gray-500 dark:text-gray-400">Se elige un nuevo ganador realizando la misma dinámica en otra fecha cercana (se anunciará la nueva fecha).</p>
    <p class="mb-2 text-gray-500 dark:text-gray-400">Esto significa que, ¡Tendrías el doble de oportunidades de ganar con tu mismo boleto!</p>
  </AccordionItem>
  <AccordionItem class="text-2xl secondary-color">
    {#snippet header()}¿DÓNDE SE PUBLICA A LOS GANADORES?{/snippet}
    <p class="mb-2 text-gray-500 dark:text-gray-400">En nuestra página oficial de Facebook RIFAS EL GUERO puedes encontrar todos y cada uno de nuestros sorteos anteriores, así como las transmisiones en vivo con Lotería Nacional y las entregas de premios a los ganadores!</p>
  </AccordionItem>
</Accordion>


  </div>
</div>

</main>


<style>
  p
  {
    font-size: 1.4rem;
    color: #fff;
  }
</style>