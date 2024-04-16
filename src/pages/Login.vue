<template>
  <div>
    <q-form @submit="enviarForm" class="q-pa-xl">
      <q-input v-model="usuario" placeholder="ingresa tu usuario" type="text" />
      <q-input v-model="password" placeholder="ingresa tu password" type="text" />
      <p class="text-pink-9">Test ...</p>
    </q-form>
  </div>
</template>

<script>
export default {
  data(){
    return{
      usuario: '',
      password: ''
    }
  },
  methods:{
    enviarForm(){

    }
  }
};
</script>

<style lang="scss" scoped></style>
