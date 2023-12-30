﻿# Classes-de-um-jogo
// Definição da classe Heroi
class Heroi {
  // Construtor da classe
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  // Método para o herói atacar
  atacar() {
    let ataque;

    // Determina o tipo de ataque com base no tipo do herói
    if (this.tipo === "mago") {
      ataque = "usou magia";
    } else if (this.tipo === "guerreiro") {
      ataque = "usou espada";
    } else if (this.tipo === "monge") {
      ataque = "usou artes marciais";
    } else if (this.tipo === "ninja") {
      ataque = "usou shuriken";
    } else {
      ataque = "usou um ataque genérico";
    }

    // Exibe a mensagem do ataque
    console.log(`O ${this.tipo} ${this.nome} atacou usando ${ataque}`);
  }
}

// Exemplo de uso da classe Heroi
const heroi1 = new Heroi("Aragorn", 30, "guerreiro");
const heroi2 = new Heroi("Gandalf", 1000, "mago");

// Chamando o método atacar para cada herói
heroi1.atacar(); // Saída esperada: O guerreiro Aragorn atacou usando espada
heroi2.atacar(); // Saída esperada: O mago Gandalf atacou usando magia
