---
marp: true
theme: gaia
backgroundColor: white
color: black
paginate: true
footer: Introdução à Programação - Fabrício Barros Cabral <<fabricio.cabral@ead.ifpe.edu.br>>
---
<style>
img[alt~="center"] {
    display: block;
    margin: 0 auto;
}
</style>

<!-- _paginate: false -->
# **Introdução à Programação**

## Capítulo 12 - Exceções

---

## Exceção

- Mecanismo para tratamento de erros
- Interrompe o fluxo normal de execução de um programa
  - Uma exceção é *lançada* para indicar quando o erro aconteceu
- Permite que o programa tente se recuperar do erro
  - Exibir uma mensagem de erro
  - Tentar corrigir o erro e continuar a execução

---

## Sintaxe

- Lançar uma exceção
  ```javascript
  throw expressao;
  ```
  
  Em que `expressao` especifica o valor da exceção

- Exemplos
  ```javascript
  throw "Isto é um erro";
  throw 42;
  throw Error("Uma mensagem de erro");
  ```

---

## Exemplo
  
```javascript
function divide(x, y) {
    if (y == 0) {
        throw new Error("Não é possível dividir por zero");
    }
    return x / y;
}
```

---

## Sintaxe

- Tratamento de exceções

```javascript
try {
    // Instruções que podem lançar uma exceção
} catch (excecao) {
    // Instruções para tratar a exceção
} finally {
    // Instruções que são sempre executadas
}
```

Observação: `finally` é opcional

---

## Exemplo

```javascript
try {
    document.write(divide(10, 2)); // imprime 5
    document.write(divide(10, 0)); // lança exceção
} catch (error) {
    document.write(error); // imprime "Não é possível dividir por zero"
}
```

---

## Exemplo

```javascript
try {
    // Tenta executar algumas instruções
} catch (error) {
    // Se deu algum erro, faça alguma coisa
    //   - Escrever o erro em um log
    //   - Mostrar alguma mensagem de erro
} finally {
    // Libera algum recurso
    //   - Fechar conexão com banco de dados
    //   - Fechar algum arquivo
}
```