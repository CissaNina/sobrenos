<template>
  
  <section>
    <h1>Resultados</h1>
 
  
  	<ul>
  		<li>
  			<img src="../assets/1.svg">
  				<h3>18 toneladas de resíduos coletados em dois anos</h3> <p>7,460T de Garrafas Pet; 1,322T de alumínio; 3,688T de plástico duro; 3,851T de papelão; 1,789T de Longa Vida; 1320l de óleo usado</p>
		</li>
		<li><img src="../assets/2.svg">
			<p>Revitalização de espaços que costumavam servir como depósito de lixo irregular</p>
		</li>
		<li><img src="../assets/3.svg">
			<p>Melhor relação entre profissionais da Comlurb e moradores</p>
		</li>
		<li><img src="../assets/4.svg">
			<p>Valorização dos profissionais de limpeza Aumento do rendimento e produtividade	</p>
		</li>
		<li><img src="../assets/5.png">
			<p>Comunidade mais limpa</p>
		</li>
		<li><img src="../assets/6.svg">
			<p>Caçambas de lixo cheias Maior conscientização ambiental</p>
		</li>
		<li>
			<img src="../assets/7.svg">
			<p>Moradores com atitudes socio-ambientais</p>
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
		height: 667px;
		background: #7AC49F;
	}

	h1{
		display: flex;
        justify-content: flex-start;
        align-items: flex-end;	
		width: 221px;
		height: 55px;
		size: 42px;
		color: #FFFFFF;
		text-align: left;
        padding-left: 25%;
        margin: 0;
        font-size: 225%;

	}


	ul {
		display:flex;
		flex-direction: row;
		flex-wrap:wrap;
		justify-content: center;
		line-height: 0.7em;
 		width:100%;
 		height:84%;
     	list-style-type:none;
     	padding-left:10px;


 }

 	li{		
 		width: 30%;
 		height: 20%;


 	}

	img{
		size: 3px;
		width: 82.90px;
		height: 82.90px;	
  		margin: 0 .8%;
	}

	p{
		font-family: 'Roboto Slab, Regular';
		width: 95.7px;
		height: 65.01px;
		font-size:8px;
		color: #FFFFFF;
		text-align: center;
	}

	h3{
		font-family: 'Roboto Slab, Regular';
		width: 95.7px;
		height: 15.01px;
		font-size:8px;
		color: #FFFFFF;
		text-align: center;
	}
</style>