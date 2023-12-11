<template>
    <v-footer
    style="background:#950c15;" class=" text-center d-flex flex-column" 
    >
      <div>
        <v-btn style="color:#ffffff;"
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          :icon="icon"
          variant="text"
        ></v-btn>
      </div>
  
      <div class="pt-0" style="color:#ffffff;">
        Descripcion del estudio Peña&Faura
      </div>
  
      <v-divider></v-divider>
  
      <div style="color:#ffffff;">
        {{ new Date().getFullYear() }} — <strong>Peña & Faura</strong>
      </div>
      <div>
        <section style="color:#ffffff;" class="w-full text-center mt-16">
			Diseñado por Remain Computers &copy; 2023
	    </section>        
      </div>

    </v-footer>
  </template>
  <script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>