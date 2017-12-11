<template>  
  <section>
    <div class="sobre-txt">
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
        </div>
        <div class="sobre-img">
            <img src="../assets/01.jpg">
        </div>      
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
body{
  margin: 0 auto;
  padding: 0 auto;
}
    div{
          display: flex;
          justify-content: flex-start;
          flex-direction: column;
          width: 100%;
          margin: 0;
          padding: 0;
    } 
      h1{ 
          
          font-family: 'Roboto Slab, Bold';
          color: #00923F;
          size: 42px;
          text-align: left;
          padding-left: 21.32px;
          margin: 0;
          font-size: 1.5em;
        }
      p{
        font-family:'Roboto Slab, Regular';
        color: #000000;
        width:70%;
        opacity: 100%;
        padding-left: 21.32px;
        font-size: 0.75em;


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

    

      img{width: 305px;
          height:225.21px;  }


            @media (min-width: 1024px) {

              
              section{
                display: flex;
              }

              h1{
                width: 413px;
                height: 50px;
                size: 89px;
              }

              p{
                width: 65%;
                size: 22px;
                margin-left: 20px; 
              }

              h3{ 
                  width: 282px;
                  height: 23px;
                  size:44px;
                  font-size: 20px;
                  }

              img{
                width: 30%;
                height: 30%;
                background:url(../assets/desabamento3.jpg) center center;;
                background-repeat: no-repeat;
                } 


            }
      
</style>
