<template>
  <div id="app">
    <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav> -->
    <router-view/>
  </div>
</template>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Quantico&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap');

  * {
    margin: 0px;
    padding: 0px;
    font-family: 'Poppins', sans-serif;

    text-decoration: none;
  }

  button:hover {
      cursor: pointer;
  }

  body {
    background-image: url("./assets/img/triangles.png");
    background-size: cover;
    background-attachment: fixed;
    background-repeat: no-repeat;

    display: flex;
    flex-direction: column;
    align-items: center;
  }

  header {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    margin: 8vh 0px 3vh 0px;
}

  nav {
    display: flex;
    justify-content: space-between;
    width: 280px;

    margin-top: 3vh;
}

  .title {
    text-align: center;
  }
 
  .title > h1 {
    font-size: 1.9rem;
    color: #000;
  }

  .title > h3 {
    font-size: 1.2rem;
    color: #000;
  }

  /* estilo padrão link: */
  .link {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #D2D2D2;
    transition: all .3s ease-in;
    font-size: .8rem;
  }

  .link > svg {
    transition: all .3s ease-in;
  }

  .fridge_icon,
  .star_icon,
  .clock_icon {
    fill: #D2D2D2;
    height: 24px;
  }

  /* estilo ao passar o mouse em cima (hover): */
  .link:hover {
    color: #00726E;
  }

  .link:hover > .fridge_icon,
  .link:hover > .star_icon,
  .link:hover > .clock_icon {
      fill: #00726E;
  }

  /* estilo específico (ilusão de estado)  */
  .link_active {
      color: #00726E;
  }

  .link_active > .fridge_icon,
  .link_active > .star_icon,
  .link_active > .clock_icon {
      fill: #00726E;
  }

  .items{
    border: 0px;
    border-radius: 50px 50px 0px 0px;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    background-color: #fff;
    display: flex;
    flex-direction: column;
    width: 90%;
    bottom: 0px;
    top: 40vh;
    min-height: 60vh;
    position: absolute;
  }

  .items_title {
    display: flex;
    align-self: center;
    margin: 12px 10vw 0px 10vw;
    align-items: center;
  }

  .items_title > h3 {
    margin: 0px 2vh;
    font-size: .9rem;
  }

  .items_title > span {
    width: 24px;
    height: 3px;
    background-color: #f1f1f1;
  }

  .green_button{
    border: 0px;
    border-radius: 10px;
    padding: 12px 27px 12px 16px;
    color: #fff;
    background-color: #33AFAA;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    top: -20px;
    position: relative;
    align-self: center;
  }

  .gray_button{
    border: 0px;
    border-radius: 10px;
    padding: 10px 12px;
    color: #00726E;
    background-color: #EAF3F1;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    align-self: center;
  }

  .gray_button > svg {
    fill: #00726E;
  }

  ::-webkit-scrollbar {
    width: 16px;
  }

  ::-webkit-scrollbar-track {
    background-color: transparent;
    margin-top: 18px;
  }

  ::-webkit-scrollbar-thumb {
    background-color: #d6dee1;
    border-radius: 20px;
    border: 6px solid transparent;
    background-clip: content-box;
  }

  ::-webkit-scrollbar-thumb:hover {
    background-color: #a8bbbf;
  }

  @media (min-width: 460px) {
    .items {
      width: 420px;
    }
    .list_transactions {
      padding: 0px 3vw 0px 4vw !important;
    }
    .items_title {
      margin: 32px 4vw 16px 4vw !important;
    }
  }
</style>

