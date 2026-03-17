<template>
  <div class="d-flex justify-center align-center" 
    style="height: 100vh"> 
      <v-card width="400" class="text-center" elevation="12">
        <!-- LOGO -->
         <v-icon size="80" color="pink" class="mt-10">mdi-apple</v-icon>
        <v-card-text class="py-10"  >
          <!-- Username TextField -->
          <v-text-field  variant="outlined" v-model="username" flat label="Username" prepend-inner-icon="mdi-account" clearable> </v-text-field>
          <!-- Password TextField -->
          <v-text-field variant="outlined" v-model="password" flat label="Password" prepend-inner-icon="mdi-lock" type="password" clearable> </v-text-field>
          <!-- Signin Button -->
          <v-btn color="primary" @click="login" block >Signin</v-btn>
        </v-card-text>
      </v-card>
  </div>
</template>

<script setup>
definePageMeta({
    layout: 'auth',
});
const defaultUsername = ref ("Admin");
const defaultPassword = ref ("Admin123");
const username = ref ("");
const password = ref ("");
  
// Regular Function
function login(){

// alert("Login function called");
if (username.value === defaultUsername.value )
if (username.value === defaultPassword.value )
}
</script>