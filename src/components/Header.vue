<template>
  <v-card>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase mr-4">
        <span>Stock</span>
        <span class="font-weight-light">Trader</span>
      </v-toolbar-title>
      <v-toolbar-items>
        <v-btn flat to="/">Início</v-btn>
        <v-btn flat to="/portfolio">Portfólio</v-btn>
        <v-btn flat to="/stocks">Ações</v-btn>
      </v-toolbar-items>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn flat>Finalizar o Dia</v-btn>
        <v-menu offset-y>
          <template v-slot:activator="{ on, attrs }">
            <v-btn flat v-bind="attrs" v-on="on"> Salvar & Carregar </v-btn>
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
      </v-toolbar-items>
    </v-toolbar>
  </v-card>
</template>

<script>
export default {};
</script>

<style>
</style>