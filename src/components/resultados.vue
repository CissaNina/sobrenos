<template>
  
  <section>
    <h1>Resultados</h1>
 
  
  	<ul>
  		<li>
  			<img src="../assets/1.png">
  			<p>18 toneladas de resíduos coletados em dois anos 7,460T de Garrafas Pet; 1,322T de alumínio; 3,688T de plástico duro; 3,851T de papelão; 1,789T de Longa Vida; 1320l de óleo usado</p>
		</li>
		<li><img src="../assets/2.png">
			<p>Revitalização de espaços que costumavam servir como depósito de lixo irregular</p>
		</li>
		<li><img src="../assets/3.png">
			<p>Melhor relação entre profissionais da Comlurb e moradores</p>
		</li>
		<li><img src="../assets/4.png">
			<p>Valorização dos profissionais de limpeza Aumento do rendimento e produtividade	</p>
		</li>
		<li><img src="../assets/5.png">
			<p>Comunidade mais limpa</p>
		</li>
		<li><img src="../assets/7.png">
			<p>Caçambas de lixo cheias Maior conscientização ambiental</p>
		</li>
		<li>
			<img src="../assets/8.png">
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
	
	section{
		width: 375px;
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
        padding-left: 21.32px;
        margin: 0;
        font-size: 225%;
	}
	ul {
     	list-style-type:none;

 }

 	li{
 		

 	}

	img{
		width: 82.9px;
		height: 82.9px;
	}

	p{
		font-family: 'Roboto Slab, Regular';
		width: 95.7px;
		height: 65.01px;
		size: 8px;

	}
</style>