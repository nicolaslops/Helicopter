# HELICOPTER

## Sobre o Projeto

Este projeto consiste em uma simulação física interativa onde o usuário controla um helicóptero com o objetivo de lançar e acertar uma caixa (pacote) dentro de uma caçamba. A aplicação combina HTML, CSS e a biblioteca **p5.js** com a extensão **p5.play**, integrando também a poderosa biblioteca de física de corpos rígidos **Matter.js** para simular gravidade, massa e inércia de forma realista.

A interface renderiza o helicóptero e o pacote em um ambiente bidimensional. O JavaScript gerencia a movimentação da aeronave pelo cenário e o momento exato do desatracamento ou lançamento do pacote, aplicando cálculos reais de queda livre e colisão quando o objeto interage com o solo ou com a caçamba.

---

## Funcionalidades

* Controle de movimentação livre do helicóptero pelo cenário através do teclado.
* Mecânica de lançamento do pacote baseado em comandos de input do usuário.
* Simulação realista de gravidade, peso e atrito aplicada à caixa através da engine `Matter.js`.
* Sistema de detecção de colisões para validar o encaixe ou impacto do pacote com a caçamba.
* Renderização fluida de sprites dinâmicos integrada à simulação de física em tempo real.

---

## Tecnologias Utilizadas

* **HTML5**
* **CSS3**
* **p5.js** (e extensão: p5.play.js)
* **Matter.js** (Engine de física 2D)

---

## Objetivo

O principal objetivo deste projeto é integrar uma engine de física externa (`Matter.js`) ao ecossistema de renderização do p5.js. O foco está em compreender como gerenciar corpos rígidos (Rigid Bodies), aplicar forças gravitacionais constantes sobre objetos dinâmicos e sincronizar as coordenadas da simulação matemática com os sprites desenhados na tela.

---

## Aprendizados

Durante o desenvolvimento deste projeto, foram aplicados conceitos como:

* Inicialização e configuração do motor físico (`Engine`, `World` e `Bodies`) da Matter.js.
* Sincronização contínua das posições e rotações físicas calculadas pela engine com os sprites do p5.js.
* Aplicação de vetores de velocidade e forças para simular a queda livre do pacote de forma natural (gravidade).
* Criação de corpos estáticos (caçamba/chão) e corpos dinâmicos (pacote) com propriedades de massa e restituição (bouncing).
* Manipulação e atualização de estados do objeto (atrelado ao helicóptero versus solto no espaço).

---

## Como Executar

1. Clone este repositório:
```bash
git clone [https://github.com/seu-usuario/HELICOPTER.git](https://github.com/seu-usuario/HELICOPTER.git)
```

2. Acesse a pasta do projeto:

```bash
cd HELICOPTER
```

3. Abra o arquivo index.html em seu navegador de preferência para pilotar o helicóptero e realizar os lançamentos.

---

## Estrutura do Projeto

```text
HELICOPTER/
│
├── assets\img/
│   ├── helicopter.png
│   └── package.png
│
├── scripts/
│   ├── matter.js
│   ├── p5.js
│   ├── p5.play.js
│   └── sketch.js
│
├── style/
│   └── style.css
│
├── index.html
└── README.md
```

--- 

## Licença

Este projeto foi desenvolvido exclusivamente para fins educacionais e de aprendizado.

Desenvolvido como prática de desenvolvimento de jogos e simulações físicas, aplicando gravidade e colisão em um sistema de entrega por helicóptero utilizando p5.js e Matter.js.
