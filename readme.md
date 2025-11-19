# ⚔️ Desafio Classificador de Nível de Herói em JavaScript

Este projeto simples em JavaScript resolve um desafio de lógica de programação focado no uso de variáveis, operadores lógicos e estruturas de decisão (`if/else if/else`). O objetivo é classificar o nível de um herói com base em sua quantidade de Experiência (XP).

---

## ✨ Objetivo

Crie uma variável para armazenar o nome e a quantidade de experiência (XP) de um herói, e utilize uma estrutura de decisão para determinar e exibir seu nível, conforme as regras estabelecidas.

## 🚀 Como Executar

Para rodar este código, você pode:
1.  Salvar o código em um arquivo chamado `classificador.js`.
2.  Executar via Node.js no seu terminal:
    ```bash
    node classificador.js
    ```
3.  Ou, colar o código no console de desenvolvimento de qualquer navegador.

## 📋 Regras de Classificação

O nível do herói é determinado pela sua XP, seguindo as seguintes faixas:

| Faixa de XP | Nível |
| :---: | :---: |
| XP $\le 1.000$ | Ferro |
| XP $1.001$ a $2.000$ | Bronze |
| XP $2.001$ a $5.000$ | Prata |
| XP $5.001$ a $7.000$ | Ouro |
| XP $7.001$ a $8.000$ | Platina |
| XP $8.001$ a $9.000$ | Ascendente |
| XP $9.001$ a $10.000$ | Imortal |
| XP $\ge 10.001$ | Radiante |

## 💻 Código-Fonte (JavaScript)

```javascript
// Variáveis para armazenar o nome e a XP do herói
let nome = "Thor";
let experiencia = 2004; // Altere este valor para testar diferentes níveis!
let nivel; // Variável que armazenará a string do nível

// Estrutura de Decisão
if (experiencia < 1000) {
    nivel = "Ferro";
} else if (experiencia >= 1001 && experiencia <= 2000) {
    nivel = "Bronze";
} else if (experiencia >= 2001 && experiencia <= 5000) {
    nivel = "Prata";
} else if (experiencia >= 5001 && experiencia <= 7000) {
    nivel = "Ouro";
} else if (experiencia >= 7001 && experiencia <= 8000) {
    nivel = "Platina";
} else if (experiencia >= 8001 && experiencia <= 9000) {
    nivel = "Ascendente";
} else if (experiencia >= 9001 && experiencia <= 10000) {
    nivel = "Imortal";
} else {
    nivel = "Radiante";
}

// Saída final
console.log(`O Herói de nome **${nome}** está no nível de **${nivel}**`);