<template>
  <div class="home">

  </div>
</template>

<script >


export default {
    components: { },
    methods: {
      teste() {
        var listas = [true,false,true];
        var pessoa = {
          nome: 'Alek',
          idade: 18
        };

        JSON.stringify(pessoa);
        console.log();

      },
    },
  beforeCreate() {
    this.teste();
    },
}


</script>

<style lang="scss" scoped>

</style>
