<template>
  <div>
    <q-form @submit="enviarData">
      <q-input filled v-model="date" mask="date" :rules="['date']">
        <template v-slot:append>
          <q-icon name="event" class="cursor-pointer">
            <q-popup-proxy
              cover
              transition-show="scale"
              transition-hide="scale"
            >
              <q-date v-model="date">
                <div class="row items-center justify-end">
                  <q-btn v-close-popup label="Close" color="primary" flat />
                </div>
              </q-date>
            </q-popup-proxy>
          </q-icon>
        </template>
      </q-input>
      <q-btn color="secondary" type="submit">Envio de info</q-btn>
    </q-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      date: "2030/02/01",
    };
  },

  methods:{
    enviarData(){
      const numero = 2;
      console.log(this.date)
      console.log(numero)
      console.log('enviando data....')
    }
  },
};
</script>

<style lang="scss" scoped>
.rojo {
}
</style>
