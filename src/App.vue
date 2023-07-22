<script setup>
import { reactive } from 'vue';

  const nome = 'Tarcio Teles';
  const meuObj = {
    nome: 'Teles',
    filmeFavorito: 'O matemático'
  }
  function dizOla () {
    const nome = 'Tarcio Teles';
    return `Olá ${nome}`
  }


  const ImagemDoFilmeOMatematico = 'data:image/jpeg;base64,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';

  const imagemFilmeOppehaimer = 'https://proxy.olhardigital.com.br/wp-content/uploads/2023/07/Destaque-Poster-de-Oppenheimer.jpg';

  const botaoEstaDesabilitado = false;

  const gostaDoOmatematico = false;
  const gostaDoOppehaimer = false;
  const estaAutorizado = false;
//  const nomes = ['Tarcio', 'Teles', 'Silva', 'Farias', 'Joana', 'José']

  
  function incrementar () {
    estado.contador++;
  }
  
  function decrementar () {
    estado.contador--;
  }
  
  //let contador =0;
  const estado = reactive({
    contador: 0,
    email: '',
    saldo: 5000,
    transferindo: 0,
    nomes: ['Tarcio', 'Teles', 'Silva', 'Farias', 'Joana', 'José'],
    nomeAInserir: '',


  });

  function mostraSaldoFuturo () {
    const {saldo, transferindo} = estado; //de onde iremos tirar os dados.//desestruturação de objetos
    return saldo - transferindo;
  }

  

  function alteraEmail(evento) {
    estado.email = console.log(evento.target.value);
  }

  function validarValor () {
    return estado.transferindo<estado.saldo;
  }

  function cadastrarNome() {
    if (estado.nomeAInserir.length >= 3) {
      estado.nomes.push(estado.nomeAInserir)
    } else {
      alert('Digite mais caracteres')
    }
  }



</script>







<template>
    <h1>
    Olá vue o {{ nome }} te deseja um ótimo Hello Word!!!
    <br>
    {{ 10 * 15 }}
    </h1>
    <h3>
      {{ meuObj.filmeFavorito }}
      <br>
      {{dizOla() }}

    </h3>


    <img v-if="gostaDoOmatematico" :src="ImagemDoFilmeOMatematico" alt="Filme O Matemático">
    <img v-else-if="gostaDoOppehaimer" :src="imagemFilmeOppehaimer" alt="">
    <br><br>
    <button :disabled="botaoEstaDesabilitado">Enviar Menssagem</button>
    
    <h1 v-if="estaAutorizado">Bem-Vindo</h1>
    <h1 v-else>Não possui acesso!</h1>
    <hr>
    {{ estado.contador }}

    <button @click="incrementar" type="button">+</button>
    <button @click="decrementar" type="button">-</button>

    <br><hr><br>

    {{ estado.email }}
    <input type="email" @change="evento => estado.email = evento.target.value">
    <input type="email" @keyup="alteraEmail">

    <br><hr><br>

    Saldo: {{ estado.saldo }} <br>
    Transferindo: {{ estado.transferindo }} <br>
    Saldo depois da transação: {{ mostraSaldoFuturo() }} <br>
    <input :class="campo" class="{invalido: !validarValor() }" @keyup="evento => estado.transferindo = evento.target.value" type="number" placeholder="Quantia para transferir" />
    <button v-if="validarValor()"  type="submit">Transferir</button>
    <span v-else>Saldo indisponível</span>
    <br><hr><br>
    <br><hr><br>

    <ul>
      <li v-for="nome in estado.nomes">
        {{ nome }}
      </li>
    </ul>

    <input @keyup="evento => estado.nomeAInserir = evento.target.value" type="text" placeholder="Digite um novo nome">
    <button @click="cadastrarNome()" type="button">Cadastrar Nome</button>
    <h3 v-for="nome in estado.nomes">{{ nome }}</h3>
  
</template>









<style scoped>
  img {
    max-width: 200px;
    height: 150px;
    border-radius: 18px;
  }

  .invalido {
    outline-color: red;
    border-color: red;

  }

  .campo{
    border: solid 4px black;
  }

</style>
