Estudo de javascipt com gustavo guanabara

# Estudos de JavaScript

Repositório de exercícios feitos durante os estudos de JavaScript com o curso do Gustavo Guanabara. Os exemplos usam HTML, CSS e JavaScript no mesmo arquivo para praticar a interação com o navegador.

## O que estou aprendendo

A sequência trabalha os fundamentos da linguagem e, depois, mostra como o JavaScript pode modificar uma página HTML:

- receber dados com `window.prompt()`;
- mostrar mensagens com `window.alert()`;
- guardar valores em variáveis;
- converter textos para números com `Number()`;
- fazer operações matemáticas;
- usar template strings e concatenação;
- manipular textos e suas propriedades;
- acessar elementos HTML pelo DOM;
- alterar estilos e conteúdo da página;
- responder a eventos como clique e movimento do mouse;
- criar funções para organizar ações.

## Exercícios

### `ex001.html` - Primeiro contato e número aleatório

O arquivo mostra uma página simples com o texto "Olá, Mundo!". Em seguida, o JavaScript:

1. pede um número ao usuário com `window.prompt()`;
2. mostra o número digitado com `window.alert()`;
3. gera um número aleatório;
4. compara o número digitado com o número gerado usando `if`;
5. informa quando o usuário acerta.

**O que estou aprendendo:** entrada de dados, variáveis, template strings, geração de números aleatórios, comparação e estrutura condicional.

**Observação:** a expressão `Math.floor(Math.random() * 1) + 1` sempre gera `1`. Para sortear números de 1 a 10, por exemplo, seria necessário usar `Math.floor(Math.random() * 10) + 1`.

### `ex002.html` - Nome do usuário

O programa pergunta o nome da pessoa, guarda a resposta na variável `nome` e exibe uma saudação usando o operador `+` para juntar textos e valores.

**O que estou aprendendo:** variáveis, entrada de texto, concatenação e montagem de mensagens dinâmicas.

### `ex003.html` - Soma de dois números

O programa solicita dois valores, converte as respostas de texto para números com `Number()`, soma os valores e mostra o resultado.

**O que estou aprendendo:** conversão de tipos, variáveis intermediárias, operadores aritméticos e template strings.

A conversão é necessária porque o `prompt()` retorna texto. Sem `Number()`, o operador `+` poderia juntar os valores como texto em vez de somá-los.

### `ex004.html` - Manipulação de strings

O programa pede um nome e escreve na página:

- a quantidade de letras com `nome.length`;
- o nome em minúsculas com `nome.toLowerCase()`;
- o nome em maiúsculas com `nome.toUpperCase()`.

**O que estou aprendendo:** propriedades e métodos de strings, template strings e escrita de conteúdo no documento com `document.write()` e `document.writeln()`.

### `ex005.html` - Primeiros passos com o DOM

O exercício apresenta uma página com parágrafos e uma `div`. O JavaScript acessa elementos HTML de diferentes formas:

- `getElementsByTagName('p')[1]` seleciona o segundo parágrafo;
- `getElementById('msg')` seleciona a `div` pelo `id`;
- `querySelector('div#msg')` seleciona a mesma `div` usando um seletor CSS.

Depois, altera as cores da `div` com `style.backgroundColor` e `style.color`.
  
**O que estou aprendendo:** DOM, seleção de elementos, índices de coleções, seletores CSS e alteração de estilos com JavaScript.

### `ex006.html` - Rascunho de uma soma com evento

Este arquivo parece ser um rascunho de uma atividade para somar os valores `20`, `50` e `10` quando um elemento com `id="gamepad"` fosse clicado. O resultado seria exibido em um elemento com `id="history"`.

**O que estou aprendendo ou tentando praticar:** eventos de clique, `addEventListener()`, atualização de conteúdo com `innerHTML` e organização de uma interação entre HTML e JavaScript.

**Situação atual:** o exercício não executa como está. A tag `<script>` não foi fechada corretamente e existem declarações inválidas, como `var 20 = 20` e `inputs keyboard = ...`. Além disso, os elementos `#gamepad`, `#history` e `#keyboard` não aparecem no HTML. O arquivo representa uma tentativa importante, mas ainda precisa ser corrigido para funcionar.

### `ex010.html` - Eventos do mouse

O exercício cria uma área verde e associa três eventos à `div` com `id="Area"`:

- `click`: troca o texto para "clicou!" e a cor para vermelho;
- `mouseenter`: troca o texto para "entrou!" e a cor para azul;
- `mouseout`: troca o texto para "saiu!" e a cor para verde.

As ações ficam separadas nas funções `clicar()`, `entrar()` e `sair()`.

**O que estou aprendendo:** seleção de elementos, eventos do mouse, `addEventListener()`, funções, alteração de texto com `innerText` e alteração de estilos.

### `ex010p2.html` - Soma usando formulário

O usuário digita dois números em campos `input` e clica no botão **Somar**. O botão chama a função `somar()`, que:

1. acessa os campos e a área de resultado pelo `id`;
2. lê os valores com `.value`;
3. converte os valores para números com `Number()`;
4. soma os números;
5. atualiza a `div` de resultado com `innerHTML`.

**O que estou aprendendo:** funções, formulários, acesso ao valor de inputs, conversão de dados, eventos de clique e atualização dinâmica do conteúdo da página.

## Resumo da evolução

| Exercício | Principal aprendizado |
| --- | --- |
| `ex001` | Prompt, alert, aleatoriedade e `if` |
| `ex002` | Variáveis e concatenação |
| `ex003` | Conversão para número e soma |
| `ex004` | Propriedades e métodos de strings |
| `ex005` | Seleção e alteração de elementos do DOM |
| `ex006` | Rascunho de eventos e atualização do DOM |
| `ex010` | Eventos do mouse e funções |
| `ex010p2` | Inputs, funções e cálculo na página |

