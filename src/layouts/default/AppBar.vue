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
      <v-responsive>
      <v-dialog
        transition="dialog-top-transition"
        width="800px"
        
      >
        <template v-slot:activator="{ props }">
          <v-btn
          style="color: aliceblue;"
            v-bind="props"
          >Contactenos</v-btn>
        </template>

        <template v-slot:default="{ isActive }">

          <v-card >
            <!--
            <v-toolbar style="background:#950c15;" class="v-toolbar-title"
              title="Contactenos"
            ></v-toolbar>
            -->
            
            <v-row>
              <v-col cols="12" sm="6" md="4">
                <v-img class="mx-auto my-auto" width="300" height="300"  src="@/assets/logoPyF.png"></v-img>
              </v-col>
              
              <v-divider :thickness="5" class="border-opacity-0" vertical></v-divider>
              <v-col>
          <v-card-text>
              
          <form @submit.prevent="submitForm">
            <!-- Formulario Dialogo Contacenos PyF -->
            
            <v-row>
              <v-col>
                <v-text-field class="prepend-icon"
                  clearable
                  label="Nombre"
                  v-model="formData.name"
                  prepend-icon="mdi-account"
                  variant="solo-filled"
                ></v-text-field>

                <v-text-field class="prepend-icon"
                  clearable
                  label="Telefono"
                  v-model="formData.telefono"
                  prepend-icon="mdi-cellphone"
                  variant="solo-filled"
                ></v-text-field>
              </v-col>
            
            
            
              <v-col>
                <v-text-field class="prepend-icon"
                  clearable
                  label="Correo"
                  v-model="formData.correo"
                  prepend-icon="mdi-email"
                  variant="solo-filled"
                ></v-text-field>

                <v-text-field class="prepend-icon"
                  clearable
                  label="Asunto"
                  v-model="formData.asunto"
                  prepend-icon="mdi-card-account-mail"
                  variant="solo-filled"
                  ></v-text-field>
                </v-col>
            </v-row>
            
                <v-textarea class="prepend-icon"
                  clearable
                  label="Label"
                  prepend-icon="mdi-message"
                  variant="solo-filled"
                ></v-textarea>
                
            <!-- Otros campos del formulario -->

            <v-btn type="submit">Enviar</v-btn>
          </form>
        </v-card-text>
      </v-col>
      </v-row>
        <v-card-actions class="justify-end">
              <v-btn
                variant="text"
                @click="isActive.value = false"
              >Close</v-btn>
            </v-card-actions>
          
          </v-card>
        </template>
      </v-dialog>  
      </v-responsive>    

      <!--<v-btn text style="color: aliceblue;">Contactenos</v-btn>-->
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
import { ref } from 'vue';

const formData = ref({
  name: '',
  email: '',
  // Agrega otros campos según tus necesidades
});

const submitForm = () => {
  // Lógica para manejar el envío del formulario
  console.log('Formulario enviado:', formData.value);
  // Puedes agregar lógica adicional, como enviar los datos al servidor, etc.
};
</script>
<style>
  .v-toolbar-title{
    color: rgb(255, 255, 255);
    text-align: center;
    font-size: 20px;
    
  }
  .prepend-icon{
    color: rgb(249, 50, 50);
  }
</style>