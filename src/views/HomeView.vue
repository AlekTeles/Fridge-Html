<template>
  <div class="home">

    <body>
    <header>
        <a class="title" href="./fridge">
            <h3>Minha</h3>
            <h1>Geladeira</h1>
        </a>
    </header>

    <section> 
        <img class="green_fridge" src="../assets/img/fridge-green.png" alt="gela">
        <div class="subtitle">
            <h4>Monitore suas comidas</h4>
            <p>Saiba sempre o que há na sua geladeira</p>
        </div>
        <a href="./fridge">
            <button class="gray_button">Pular</button>
        </a>
    </section>
</body>
  
  </div>
</template>

<script >


export default {
  name: "HomeView",
  components: {},
  methods: {},
}


</script>

<style lang="scss" scoped>

.home {
  display: flex;

  justify-content: center;

  section{
    text-align: center;
    line-break: strict;
  }

  .green_fridge{
    height: 50vh;

  }

  .subtitle {
    margin-top: 23px;
    margin-bottom: 24px;
    display: flex;
    flex-direction:  column;
    justify-content: center;
  }

  .gray_button {
    margin-bottom: 48px;
    padding: 10px 24px;
    box-shadow: none;
    background-color: #e1ece952;
    color: #00726ead;

  transition: all .3s ease-in;

    &:hover {
      background-color: #EAF3F1;
      color: #00726E;
    }

  }



  .subtitle > h4 {
    font-size: 16px;
  }

  .subtitle > p {
    font-size: 14px;
    color: #8D8D8D;
    height: 45px;
    width: 272px;
    padding-inline-start: 43px;
  }
}
  .title {
   margin-top: 50px; 
  
  }

</style>  
