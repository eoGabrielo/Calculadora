# Calculadora em JavaScript

Este projeto apresenta uma calculadora simples desenvolvida em JavaScript, HTML e CSS. A funcionalidade principal é permitir que os usuários realizem operações matemáticas básicas, como adição, subtração, multiplicação e divisão.

## Utilização

1. Clone este repositório para sua máquina local.
2. Abra o arquivo `index.html` em um navegador web.

## Funcionalidades

- **Adição de Caracteres:** Clique nos botões numerados para adicionar os dígitos desejados.
- **Operações:** Utilize os botões de operações para adicionar operadores à expressão.
- **Limpar Tela:** O botão "AC" limpa a tela, reiniciando a expressão.
- **Inverter Número:** O botão "+/-" inverte o sinal do número atual.
- **Calcular:** O botão "=" realiza o cálculo da expressão matemática e exibe o resultado.

## Detalhes Técnicos

### JavaScript (script.js)

```javascript
function adicionarCaracter(num){
    const valorDisplay = document.querySelector(".display").value
    document.querySelector(".display").value = valorDisplay + num
}

function limpaTela(){
    document.querySelector(".display").value = ""
}

function calcular(){
    const valorDisplay = document.querySelector(".display").value
    document.querySelector(".display").value = eval(valorDisplay)
}

function inverterNumero(){
    const valorDisplay = document.querySelector(".display").value
    document.querySelector(".display").value = valorDisplay * -1
}
```

O código JavaScript utiliza o método `querySelector` para selecionar elementos HTML e manipular dinamicamente o conteúdo do display. A função `eval` é utilizada para avaliar expressões matemáticas fornecidas pelo usuário.

