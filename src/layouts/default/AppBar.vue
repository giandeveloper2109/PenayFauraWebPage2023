<!-- Navbar.vue -->

<template>
  <v-responsive>
  <v-app-bar app class=" text-center d-flex flex-column" style="background:#950c15;">
    <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
    
    <div>
      <v-img class="mr-3" src="@/assets/logoPyF.png" height="60px" width="60px"></v-img>
    </div>
    <div>
      <v-toolbar-title style="color: aliceblue;" >Peña & Faura</v-toolbar-title>
    </div>
    <v-spacer></v-spacer>
    <div>
      <v-btn text style="color: aliceblue;">Quienes Somos</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: aliceblue;">Socios</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: aliceblue;">Servicios</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: aliceblue;">Contactenos</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-img class="mr-3" src="@/assets/Idiomas/espana.png" height="20px" width="20px"></v-img>
    </div>
    <div>
      <v-img class="mr-3" src="@/assets/Idiomas/ingles.png" height="20px" width="20px"></v-img>
    </div>
  </v-app-bar>
</v-responsive>
</template>

<script setup>
  //
</script>