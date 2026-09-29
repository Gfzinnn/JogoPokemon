PokeLike
Projeto de jogo em Java inspirado no universo Pokémon, desenvolvido como trabalho acadêmico para simular batalhas entre Pokémon com escolha de geração, evolução, ataques e chefões finais.

# Jogo Pokémon em Java

Projeto desenvolvido em **Java** com o objetivo de aplicar conceitos de **Programação Orientada a Objetos (POO)** por meio de um jogo de batalhas inspirado no universo Pokémon.

O jogador pode escolher um Pokémon inicial entre diferentes gerações, enfrentar adversários, ganhar experiência, evoluir seu Pokémon e avançar por diferentes mundos até enfrentar os chefões.

## Funcionalidades

- Escolha de Pokémon inicial
- Pokémon das três primeiras gerações
- Sistema de batalha por turnos
- Ataque normal e ataque especial
- Sistema de defesa
- Velocidade para determinar quem ataca primeiro
- Fraquezas e eficácias entre tipos
- Sistema de vida
- Sistema de experiência
- Evolução dos Pokémon iniciais
- Diferentes mundos de batalha
- Adversários aleatórios
- Batalhas contra Pokémon lendários
- Sistema de chefões
- Opção de continuar ou encerrar a jornada

## Progressão do jogo

O jogo é dividido em três mundos.

### Mundo 1

O jogador enfrenta Pokémon em sua primeira forma evolutiva.

**Chefão:** Darkrai

### Mundo 2

O jogador passa a enfrentar Pokémon em sua segunda forma evolutiva.

**Chefão:** Mewtwo

### Mundo 3

O jogador enfrenta Pokémon em sua forma final.

**Chefão:** Arceus

Ao derrotar Arceus, o jogador conclui o jogo.

## Sistema de batalha

Durante cada turno, o jogador pode escolher entre:

- Atacar
- Defender

Ao atacar, também é possível escolher entre:

- Ataque normal
- Ataque especial

A velocidade dos Pokémon determina qual deles realiza sua ação primeiro.

Ataques especiais também levam em consideração a eficácia e a fraqueza dos tipos dos Pokémon.

Quando o jogador utiliza a defesa, o dano recebido é reduzido.

## Sistema de experiência e evolução

Ao vencer batalhas, o Pokémon do jogador recebe experiência.

Ao atingir determinadas quantidades de experiência, os Pokémon iniciais podem evoluir.

Exemplo:

```text
Charmander
   ↓
Charmeleon
   ↓
Charizard
```

Outras linhas evolutivas presentes no projeto incluem:

```text
Bulbasaur → Ivysaur → Venusaur
Squirtle → Wartortle → Blastoise

Cyndaquil → Quilava → Typhlosion
Chikorita → Bayleef → Meganium
Totodile → Croconaw → Feraligatr

Torchic → Combusken → Blaziken
Treecko → Grovyle → Sceptile
Mudkip → Marshtomp → Swampert
```

## Estrutura do projeto

O projeto foi separado em diferentes classes para melhorar sua organização:

```text
Jogo/
│
├── Pokemon.java
├── PokemonInicial.java
├── PokemonLendario.java
├── Pokemons.java
├── Batalha.java
└── Evolucoes.java
```

### Pokemon.java

Classe principal do projeto.

Contém os atributos e comportamentos básicos dos Pokémon, getters e setters e o fluxo principal do jogo.

### PokemonInicial.java

Subclasse de `Pokemon` utilizada para representar os Pokémon iniciais.

Também possui métodos de aumento de ataque utilizados durante as evoluções.

### PokemonLendario.java

Subclasse de `Pokemon` utilizada para representar os Pokémon lendários que aparecem como chefões.

### Pokemons.java

Responsável por armazenar os Pokémon disponíveis no jogo e as listas utilizadas nos diferentes mundos.

### Batalha.java

Responsável pelo sistema de combate, incluindo:

- ataque do jogador;
- ataque do inimigo;
- defesa;
- cálculo de dano;
- velocidade;
- experiência após vitórias.

### Evolucoes.java

Responsável pelo sistema de evolução dos Pokémon iniciais.

A classe verifica a experiência acumulada e realiza as alterações de nome, vida, ataque, ataque especial e velocidade quando uma evolução acontece.

## Conceitos de POO utilizados

Durante o desenvolvimento foram utilizados diversos conceitos de Programação Orientada a Objetos, como:

- Classes e objetos
- Atributos e métodos
- Construtores
- Encapsulamento
- Getters e setters
- Herança
- Sobrescrita de métodos (`@Override`)
- Sobrecarga de métodos
- `instanceof`
- Downcasting
- Modificadores de acesso
- Collections e `ArrayList`

## Tecnologias utilizadas

- Java
- Programação Orientada a Objetos
- `ArrayList`
- `Scanner`
- `Random`

## Como executar

Clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
```

Entre na pasta do projeto e compile os arquivos Java.

Depois, execute a classe `Pokemon`, que contém o método `main`.

É necessário possuir o **Java JDK** instalado no computador.

## Objetivo do projeto

O objetivo principal deste projeto é colocar em prática os conhecimentos adquiridos em **Programação Orientada a Objetos**, utilizando um jogo de batalha Pokémon como forma de aplicar os conceitos estudados de maneira prática.

O projeto também busca trabalhar organização de código, separação de responsabilidades entre classes, herança, encapsulamento e interação entre objetos.

## Integrantes

-Gabriel Fernandes Stringuetti RA 2608590
-João Gabriel Siman Tescaro RA 2610426
-Murillo Oliveira RA 2612391
-Victor H Bissoli RA 2612837

## Disciplina

**Programação Orientada a Objetos**

**Professor:** Jesse Guimarães  
**Instituição:** UniAnchieta

---

Projeto acadêmico desenvolvido para fins de aprendizagem.
