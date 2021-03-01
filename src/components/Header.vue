<template>
  <v-card>
    <v-app-bar app>
      <v-app-bar-title class="headline text-uppercase mr-4">
        <span>Stock</span>
        <span class="font-weight-light">Trader</span>
      </v-app-bar-title>
      <v-app-bar-items>
        <v-btn text to="/">Início</v-btn>
        <v-btn text to="/portfolio">Portfólio</v-btn>
        <v-btn text to="/stocks">Ações</v-btn>
      </v-app-bar-items>

      <v-spacer></v-spacer>

      <v-app-bar-items>
        <v-btn text>Finalizar o Dia</v-btn>
        <v-menu offset-y>
          <template v-slot:activator="{ on, attrs }">
            <v-btn text v-bind="attrs" v-on="on"> Salvar & Carregar </v-btn>
          </template>
          <v-list>
            <v-list-item>
              <v-list-item-title>Salvar Dados</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title>Carregar Dados</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </v-app-bar-items>
    </v-app-bar>
  </v-card>
</template>

<script>
export default {};
</script>

<style>
</style>