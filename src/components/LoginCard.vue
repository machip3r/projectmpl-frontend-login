<template>
  <v-card class="login-card">
    <v-card-title>Login</v-card-title>
    <v-card-text>
      <v-form>
        <v-text-field
          v-model="email"
          :rules="emailRules"
          solo
          label="Correo Electrónico"
          type="email"
          clearable
          required
        ></v-text-field>
        <v-text-field
          v-model="rules"
          solo
          label="Contraseña"
          type="password"
          clearable
          required
        ></v-text-field>
      </v-form>
    </v-card-text>
    <v-card-action>
      <v-row justify="end">
        <v-btn>Cancel</v-btn>
        <v-btn color="primary" plain>Entrar</v-btn>
      </v-row>
    </v-card-action>
  </v-card>
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({});
</script>

<style>
.login-card {
  width: 50%;
  height: 30vw;
  margin: 0 auto;
  padding: 30px;
}
</style>
