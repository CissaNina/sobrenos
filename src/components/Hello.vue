<template>
  
  <section>
    <h1>Sobre nós</h1>
    <p>O ReciclAção propõe estimular e mobilizar a comunidade a
        descartar adequadamente seus materiais recicláveis,
        retirando-os do meio ambiente e dando origem a um ciclo fértil
        e produtivo que retorna em forma de recursos locais, com
        ênfase na educação e na cooperação</p>
    <p>O Projeto reciclação começou 3 anos após o desabamento do
        campinho, na Rua Gomes Lopes em 2010, provocado pelo
        temporal e acúmulo de lixo nas encostas.36 pessoas morreram
        e 7 mil ficaram desabrigadas. A partir disso o grupo PROA,
        junto com a Cris dos Prazeres e sua equipe de trabalho, criaram
        o projeto ReciclAção para promover ações de conservação e
        conscientização ambiental no morro dos Prazeres,
        concentradas no bem-estar das pessoas através do combate de
        doenças como dengue, zica e chikungunya e outras doenças
        causadas por acúmulo de lixo.</p>
        <h3><a href="">Saiba mais >></a></h3>
        <img src="../assets/01.jpg">
  </section>
</template>

<script>
import axios from 'axios';

export default {
  name: 'hello',
  data () {
    return {
      respostas: [],
    }
  },
  created() {
    axios.get(`http://jsonplaceholder.typicode.com/users`)
    .then(response => {
      this.respostas = response.data
    })
  }
}
</script>

<style>
      h1{ 
          display: flex;
          justify-content: flex-start;
          align-items: flex-end;
          font-family: 'Roboto Slab, Bold';
          color: #00923F;
          width: 195px;
          height: 55px;
          size: 42px;
          text-align: left;
          padding-left: 21.32px;
          margin: 0;
          font-size: 180%;
        }
      p{
        font-family:'Roboto Slab, Regular';
        color: #000000;
        width:330px;
        size: 11px;
        opacity: 100%;
        text-align: left;
        padding-left: 21.32px;
        font-size: 80%;


      }
      h3{ font-family: 'Roboto Slab, Bold';
          color: #E67816;
          width: 116px ;
          height:24px ;
          size:18px;
          text-align: left;
          padding-left: 21.32px;
          font-size: 100%;



      }

      a:link, a:visited {
      text-decoration: none;
  }

    

      img{width: 360px;
          height:225.21px;  }
</style>
