<template>
  
  <section>
    <h1>Resultados</h1>
 
  
  	<ul>
  		<li>
  			<img src="../assets/1.svg">
	  			<p>18 toneladas <br> <span class="nivel2">de resíduos coletados em dois anos</span> <br> <span class="nivel3">7,460T de Garrafas Pet; 1,322T de alumínio; 3,688T de plástico duro; 3,851T de papelão; 1,789T de Longa Vida; 1320l de óleo usado</span></p>
		</li>
		<li>
			<img src="../assets/2.svg">
			<p>Revitalização <br>de espaços </br><span class="nivel2">que costumavam servir como depósito de lixo irregular</span></p>
		</li>
		<li>
			<img src="../assets/3.svg">
			<p>Melhor relação <br><span class="nivel2">entre profissionais da <br>Comlurb <br>e moradores</br></span></p>
		</li>
		<li>
			<img src="../assets/4.svg">
			<p>Valorização dos profissionais <span class="nivel2"><br>de limpeza </br></span><span class="nivel3">Aumento do rendimento e produtividade</span></p>
		</li>
		<li>
			<img src="../assets/5.svg">
			<p>Comunidade <br>mais limpa</br></p>
		</li>
		<li>
			<img src="../assets/6.svg">
			<p>Caçambas de <br>lixo cheias <br><span class="nivel3">Maior <br>conscientização</br> ambiental</span></br></p>
		</li>
		<li>
			<img src="../assets/7.svg">
			<p>Moradores com atitudes <br><span class="nivel2">socio-ambientais</span></br></p>
		</li>

  	</ul>
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
		box-sizing: border-box;
		margin:  auto;
		padding:  auto;
	}
	section{
		width: 100%;
		min-height: 70vh;
		background: #7AC49F;
		display: flex;
		justify-content: center;
		align-items: flex-start;
		flex-flow: row wrap;
	}

	h1{	
		width: 80%;
		height: 55px;
		color: #FFFFFF;
		text-align: center;
        margin: 0;
        font-size: 225%;

	}


	ul {
		display:flex;
		flex-direction: row;
		flex-wrap:wrap;
		justify-content: center;
		align-items: flex-start;
		line-height: 0.7em;
 		width:100%;
 		height:84%;
     	list-style-type:none;
     	padding-left:0px;

 }

 	li{		
 		width: 13%;
 		min-width: 100px;
 		min-height: 20%;
 		margin:5px;	

 	}

	img{
		width: 100%;
		/*height: 82.90px;	*/
  		margin: 0 .8%;
	}

	p{
		font-family: 'Roboto Slab, Regular';
		/*width: 95.7px;
		height: 65.01px;*/
		font-size:15px;
		line-height:12px;
		color: #FFFFFF;
		text-align: center;

	}
	.nivel2{
		font-size: 12px
	}
	.nivel3{
		font-size: 10px
	}


				@media (min-width: 768px) {
					p{
						font-size: 18px;
						line-height:14px;
					}
					.nivel2{
						font-size: 12px;
					}
					.nivel3{
						font-size: 10px;
					}
				}

	
</style>