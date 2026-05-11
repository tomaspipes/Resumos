# Guia de Estudo — Programação Web

---

# PARTE 1 — HTML

## 1.1 Estrutura base de uma página HTML

Todo documento HTML começa com a mesma estrutura. Memoriza isto — é o esqueleto de qualquer página:

```html
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>

    <link rel="icon" type="image/png" href="favicon.png">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- O conteúdo visível vai aqui -->

    <script src="script.js"></script>
</body>
</html>
```

### O que cada parte faz

| Elemento | Para que serve |
|----------|----------------|
| `<!DOCTYPE html>` | Diz ao navegador que é HTML5 |
| `<html lang="pt">` | Elemento raiz; `lang` indica o idioma da página |
| `<meta charset="UTF-8">` | Define a codificação de caracteres (acentos, ç, etc.) |
| `<meta name="viewport" ...>` | Torna a página responsiva em telemóveis — sem isto, o mobile mostra a página em miniatura |
| `<title>` | O texto que aparece no separador do navegador |
| `<link rel="stylesheet">` | Liga um ficheiro CSS externo |
| `<script src="...">` | Liga um ficheiro JavaScript externo |

### Onde colocar o `<script>`?

**Antes de `</body>`** (no final do body). Porquê? Porque o navegador lê o HTML de cima para baixo. Se o script estiver no `<head>`, tenta aceder a elementos que ainda não existem.

Alternativa: colocar no `<head>` com o atributo `defer`:
```html
<script src="script.js" defer></script>
```
O `defer` diz ao navegador: "carrega o script já, mas só o executa depois de todo o HTML estar pronto."

---

## 1.2 Elementos semânticos

O HTML5 introduziu tags que dão **significado** à estrutura da página. Em vez de usar `<div>` para tudo, usamos tags que descrevem o *papel* de cada bloco:

```html
<body>
    <header>
        <nav>
            <!-- menu de navegação -->
        </nav>
    </header>

    <main>
        <section>
            <!-- um bloco temático, ex: "Sobre nós" -->
        </section>

        <section>
            <article></article>  <!-- conteúdo independente, ex: um post -->
            <article></article>
        </section>
    </main>

    <footer>
        <section></section>
        <section></section>
    </footer>
</body>
```

### Quando usar cada tag

| Tag | Quando usar | Exemplo |
|-----|-------------|---------|
| `<header>` | Cabeçalho da página ou de uma secção | Logo + menu de navegação |
| `<nav>` | Bloco de links de navegação | Menu principal |
| `<main>` | Conteúdo principal da página (só 1 por página) | Tudo entre o header e o footer |
| `<section>` | Agrupamento temático de conteúdo | "Sobre nós", "Serviços", "Contactos" |
| `<article>` | Conteúdo independente, que faz sentido sozinho | Um post de blog, um produto, uma notícia |
| `<footer>` | Rodapé da página ou de uma secção | Copyright, links úteis |

**Diferença entre `<section>` e `<article>`:** Um `<article>` faz sentido isoladamente (podes copiar para outro site e continua a fazer sentido). Um `<section>` é apenas um agrupamento dentro do contexto da página.

### Boas práticas de organização

Organizar ficheiros em pastas:
```
projeto/
├── index.html
├── style.css
├── script.js
├── favicon.png
└── assets/
    └── imagens/
```

---

# PARTE 2 — CSS

## 2.1 Seletores CSS

Os seletores definem *quais* elementos HTML recebem determinados estilos.

### Seletor por elemento
Aplica o estilo a **todos** os elementos desse tipo:
```css
h1 {
    color: darkblue;
}

p {
    line-height: 1.5;
}
```

### Agrupamento de seletores
Aplica o mesmo estilo a vários elementos de uma vez:
```css
h1, h2, h3 {
    font-family: Georgia, serif;
}
```

### Seletor por ID (`#`)
Seleciona **um único** elemento pelo seu `id`. O `id` deve ser único na página:
```css
#page_header {
    background-color: #8cc7fb;
}

#page_footer {
    background-color: #0d88f4;
}
```
```html
<header id="page_header">...</header>
<footer id="page_footer">...</footer>
```

### Seletor por classe (`.`)
Seleciona **todos** os elementos com essa classe. Uma classe pode ser usada em vários elementos:
```css
.destaque {
    background-color: #fff3cd;
    border: 1px solid #e0b100;
    font-weight: bold;
    border-radius: 10px;
    text-align: center;
}
```
```html
<p class="destaque">Este parágrafo está em destaque.</p>
<div class="destaque">Este div também.</div>
```

### Seletor descendente
Seleciona elementos que estão **dentro de** outro elemento:
```css
/* Apenas os links que estão dentro de <nav> */
nav a {
    text-decoration: none;
    font-weight: bold;
    color: darkgreen;
}
```
Isto significa: "aplica este estilo a todos os `<a>` que estejam em qualquer nível dentro de um `<nav>`."

### Resumo dos seletores

| Seletor | Sintaxe | O que seleciona |
|---------|---------|-----------------|
| Elemento | `p { }` | Todos os `<p>` |
| Agrupamento | `h1, h2 { }` | Todos os `<h1>` e `<h2>` |
| ID | `#nome { }` | O elemento com `id="nome"` |
| Classe | `.nome { }` | Todos os elementos com `class="nome"` |
| Descendente | `nav a { }` | Todos os `<a>` dentro de `<nav>` |

---

## 2.2 Pseudo-classes

Pseudo-classes definem estilos para **estados especiais** de um elemento. Adicionam-se ao seletor com `:`.

```css
/* Link não clicado */
main a:link {
    color: green;
}

/* Link já visitado */
main a:visited {
    color: green;
}

/* Quando o rato passa por cima */
main a:hover {
    color: red;
}

/* Quando o elemento está a ser clicado */
main a:active {
    color: yellow;
}
```

Também funcionam em outros elementos:
```css
section h2:hover {
    color: blue;
}
```

**Nota:** A ordem importa para links! Deve ser: `:link` → `:visited` → `:hover` → `:active` (mnemónica: **L**o**V**e **HA**te).

---

## 2.3 Box Model

**Todos** os elementos HTML são caixas retangulares. Cada caixa tem 4 camadas, de dentro para fora:

```
┌─────────────────── margin ───────────────────┐
│  ┌─────────────── border ──────────────────┐  │
│  │  ┌─────────── padding ───────────────┐  │  │
│  │  │                                    │  │  │
│  │  │          CONTEÚDO                  │  │  │
│  │  │                                    │  │  │
│  │  └────────────────────────────────────┘  │  │
│  └──────────────────────────────────────────┘  │
└────────────────────────────────────────────────┘
```

| Propriedade | O que faz |
|-------------|-----------|
| `padding` | Espaço **interior** — entre o conteúdo e a borda |
| `border` | A borda em si |
| `margin` | Espaço **exterior** — entre este elemento e os vizinhos |

### Exemplos

```css
.destaque {
    padding: 20px 10px;   /* 20px em cima/baixo, 10px esquerda/direita */
    margin: 40px auto;    /* 40px em cima/baixo, centrado horizontalmente */
}

#page_header {
    padding: 20px;        /* 20px em todos os lados */
    margin-top: 0px;
}
```

**Dica importante:** `margin: Xpx auto` centra um elemento horizontalmente (o `auto` divide o espaço restante igualmente).

### Atalhos de padding/margin

```css
padding: 10px;              /* todos os lados: 10px */
padding: 10px 20px;         /* cima/baixo: 10px, esquerda/direita: 20px */
padding: 10px 20px 30px;    /* cima: 10, esquerda/direita: 20, baixo: 30 */
padding: 10px 20px 30px 40px; /* cima, direita, baixo, esquerda (sentido relógio) */
```

---

## 2.4 Unidades de medida

| Unidade | Descrição | Exemplo |
|---------|-----------|---------|
| `px` | Pixels — valor fixo e absoluto | `font-size: 14px` |
| `em` | Relativa ao tamanho da fonte do **elemento pai** | `padding: 1.5em` (se pai = 14px → 21px) |
| `rem` | Relativa ao tamanho da fonte do **`<html>`** (root) | `margin-top: 3rem` (se html = 14px → 42px) |
| `%` | Percentagem do elemento pai | `width: 100%` |

```css
html {
    font-size: 14px;   /* define o tamanho base */
}

section h2 {
    margin-top: 3rem;  /* 3 × 14px = 42px (sempre relativo ao html) */
}

.destaque {
    padding: 1.5em 1em; /* relativo ao font-size do próprio elemento */
    margin: 2em auto;
}

img {
    max-width: 100%;   /* a imagem nunca ultrapassa o contentor */
}
```

**Quando usar o quê:**
- `rem` → tamanhos consistentes em toda a página (margens, espaçamentos gerais)
- `em` → tamanhos que devem escalar com o texto do elemento (padding dentro de botões, por ex.)
- `px` → bordas, sombras, coisas que devem ser exatas
- `%` → larguras responsivas

---

## 2.5 Display: block, inline e inline-block

Todo elemento HTML tem um valor `display` por defeito. Compreender isto é **essencial**:

| Tipo | Comportamento | Aceita width/height? | Exemplos |
|------|---------------|----------------------|----------|
| `block` | Ocupa toda a largura, começa numa nova linha | ✅ Sim | `<div>`, `<p>`, `<h1>`, `<section>` |
| `inline` | Ocupa só o espaço do conteúdo, fica na mesma linha | ❌ Não | `<span>`, `<a>`, `<strong>`, `<em>` |
| `inline-block` | Fica na mesma linha MAS aceita width/height | ✅ Sim | Nenhum por defeito — atribui-se manualmente |

### Exemplo prático

```css
/* <strong> é inline por defeito — width e height são ignorados */
.caixa strong {
    width: 50em;      /* NÃO funciona! */
    height: 3em;      /* NÃO funciona! */
}

/* Com inline-block, passa a aceitar dimensões */
.caixa strong {
    display: inline-block;
    width: 15em;      /* Agora funciona! */
    background-color: red;
}
```

**Resumo:** Se precisas que um elemento inline (como `<a>` ou `<strong>`) tenha largura, altura, ou margin/padding vertical → usa `display: inline-block`.

---

## 2.6 Variáveis CSS (Custom Properties)

Variáveis CSS servem para **evitar repetição**, **manter consistência** e **facilitar alterações globais**.

Declaram-se em `:root` (que representa o `<html>`) e usam-se com `var()`:

```css
:root {
    --cor-principal: #1e3a5f;
    --cor-destaque: #fff3cd;
    --cor-borda-destaque: #e0b100;

    --fonte-principal: Arial, sans-serif;
    --fonte-titulos: Georgia, serif;

    --espacamento-medio: 1em;
    --espacamento-grande: 2em;

    --raio-padrao: 8px;
}

/* Utilização */
html {
    font-family: var(--fonte-principal);
    color: var(--cor-principal);
}

h1, h2, h3 {
    font-family: var(--fonte-titulos);
    color: var(--cor-principal);
}

.destaque {
    background-color: var(--cor-destaque);
    border: 1px solid var(--cor-borda-destaque);
    border-radius: var(--raio-padrao);
}
```

**Vantagem:** Se quiseres mudar a cor principal do site inteiro, mudas **num único sítio** (`--cor-principal`) em vez de em 20 regras diferentes.

---

## 2.7 Flexbox

Flexbox é a forma moderna de alinhar elementos numa **direção** (linha ou coluna). Aplica-se ao **contentor pai**.

### Como funciona

```css
/* O pai torna-se um flex container */
nav ul {
    display: flex;       /* ativa o flexbox */
    gap: 1rem;           /* espaço entre os items */
    flex-wrap: wrap;     /* permite que os items quebrem linha */
}
```

### Direção e alinhamento

```css
nav ul {
    flex-direction: row;     /* em linha (padrão) */
    flex-direction: column;  /* em coluna */

    /* Alinhamento horizontal (no eixo principal) */
    justify-content: flex-start;     /* à esquerda (padrão) */
    justify-content: center;         /* centrado */
    justify-content: space-between;  /* distribuído com espaço entre */
}
```

### Exemplo completo: cards em flex

```css
.card {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;      /* permite que os cards mudem de linha */
}

.card article {
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 8px;
    flex-basis: 20rem;    /* largura ideal de cada card */
}
```

**`flex-basis`** define a largura ideal do item. Com `flex-wrap: wrap`, quando não cabe mais na linha, vai para a linha seguinte.

**`flex-grow: 1`** faz o item crescer para preencher espaço restante.

### Quando usar Flexbox
Ideal para: menus de navegação, grelhas de cards, centrar elementos, distribuir itens numa linha.

---

## 2.8 Grid Layout

Grid serve para layouts em **duas dimensões** (linhas E colunas ao mesmo tempo).

```css
.grelha {
    display: grid;
    gap: 1rem;
    grid-template-columns: 1fr 1fr 1fr;  /* 3 colunas iguais */
}
```

`1fr` significa "1 fração do espaço disponível". Três `1fr` = 3 colunas iguais.

**Flexbox vs Grid:**
- **Flexbox** → alinhar numa direção (linha OU coluna)
- **Grid** → organizar em linhas E colunas simultaneamente

---

## 2.9 Media Queries (Design Responsivo)

Media queries permitem **adaptar o layout** a diferentes tamanhos de ecrã:

```css
/* Ecrãs até 768px de largura (tablets) */
@media (max-width: 768px) {
    body {
        width: 90%;
        margin: 0 auto;
    }

    .grelha {
        grid-template-columns: 1fr 1fr;  /* passa a 2 colunas */
    }
}

/* Ecrãs até 600px de largura (telemóveis) */
@media (max-width: 600px) {
    nav ul {
        flex-direction: column;   /* menu fica vertical */
    }

    .grelha {
        grid-template-columns: 1fr;  /* passa a 1 coluna */
    }

    .card article {
        flex-basis: 100%;  /* cada card ocupa toda a largura */
    }
}
```

Também existe media query para dark mode:
```css
@media (prefers-color-scheme: dark) {
    body {
        background-color: #121212;
        color: white;
    }
}
```

### Helper classes
Classes utilitárias reutilizáveis:
```css
.centrado {
    text-align: center;
}

.negrito {
    font-weight: bold;
}
```
```html
<p class="centrado negrito">Texto centrado e a negrito</p>
```

---

# PARTE 3 — JavaScript: Fundamentos

## 3.1 Como executar JavaScript

Existem 3 formas, da **pior** à **melhor**:

**1. Inline (evitar):**
```html
<button onclick="alert('Olá!')">Clique</button>
```

**2. Dentro do HTML com `<script>`:**
```html
<script>
    console.log("Olá!");
</script>
```

**3. Ficheiro externo (recomendado):**
```html
<script src="script.js"></script>
```

---

## 3.2 Variáveis e tipos de dados

```javascript
let contador = 1;       // pode mudar
const incremento = 2;   // constante — não pode mudar

let nome = "Ana";        // string
let aprovado = true;     // boolean
let nota = 15;           // number
const pi = 3.14;         // number

let x;                   // undefined (declarada mas sem valor)
let artigo = null;       // null (intencionalmente vazio)

const frutas = ["Maçã", "Banana"];  // array

const aluno = {          // object
    nome: "João",
    idade: 20
};
```

**Regra:** Usar `const` por defeito. Usar `let` apenas quando o valor vai mudar. Evitar `var`.

---

## 3.3 Operadores

### Comparação: `==` vs `===`

Esta é uma pergunta clássica de teste:

```javascript
// == compara apenas o VALOR (faz conversão automática)
5 == "5"       // true  (converte "5" para 5)
true == 1      // true  (converte true para 1)
"" == 0        // true

// === compara VALOR e TIPO (sem conversão)
5 === "5"      // false (number vs string)
true === 1     // false (boolean vs number)
"" === 0       // false (string vs number)
```

**Usar sempre `===` e `!==`.** É mais seguro e previsível.

### Operadores lógicos

```javascript
const idade = 20;
const temBilhete = true;

// AND: ambas as condições têm de ser verdadeiras
const podeEntrar = idade >= 18 && temBilhete;  // true

// OR: basta uma condição ser verdadeira
const temDesconto = idade < 12 || idade > 65;  // false

// NOT: inverte o valor
const naoTemBilhete = !temBilhete;  // false
```

---

## 3.4 Conversão de tipos

**Cuidado com o `+`** — é o único operador que concatena strings em vez de converter:

```javascript
"2" * 3    // 6  (converte para número)
"10" - 2   // 8  (converte para número)
"2" + 3    // "23" (concatena como string!)
```

### Conversões explícitas

```javascript
Number("42")        // 42
Number("abc")       // NaN (Not a Number)
parseInt("25.9")    // 25 (só parte inteira)
parseFloat("3.14")  // 3.14

String(50)          // "50"
Boolean(0)          // false
Boolean("Olá")      // true
```

### Valores falsy (que se convertem em `false`)

São exatamente 6: `0`, `""` (string vazia), `null`, `undefined`, `NaN`, `false`.

**Tudo o resto é truthy** (incluindo `"0"`, `" "`, `[]`, `{}`).

---

## 3.5 Template Literals

Em vez de concatenar com `+`, usa backticks e `${}`:

```javascript
const nome = "Rute";
const idade = 20;

// Forma antiga
const msg1 = "O meu nome é " + nome + " e tenho " + idade + " anos.";

// Template literal (mais legível)
const msg2 = `O meu nome é ${nome} e tenho ${idade} anos.`;

// Pode ter expressões
console.log(`A soma é ${5 + 3}.`);  // "A soma é 8."
```

---

## 3.6 Condicionais e ciclos

```javascript
// if / else if / else
const nota = 17;
if (nota >= 18) {
    console.log("Excelente");
} else if (nota >= 10) {
    console.log("Aprovado");
} else {
    console.log("Reprovado");
}

// for — quando sabemos quantas vezes
for (let i = 0; i < 5; i++) {
    console.log(i);
}

// while — quando depende de uma condição
let tentativas = 0;
while (tentativas < 3) {
    tentativas++;
}

// forEach — para iterar arrays
const nomes = ["Ana", "Bruno", "Carla"];
nomes.forEach(nome => console.log(nome.toUpperCase()));
// ANA, BRUNO, CARLA

// forEach com índice
nomes.forEach((nome, i) => {
    console.log(`Índice ${i}: ${nome}`);
});
```

---

## 3.7 Funções

```javascript
// Declaração clássica
function somar(a, b) {
    return a + b;
}

// Com parâmetro opcional
function cumprimentar(nome = "Visitante") {
    console.log(`Olá, ${nome}.`);
}

cumprimentar("Maria");  // Olá, Maria.
cumprimentar();         // Olá, Visitante.
```

---

## 3.8 Arrays

```javascript
const nomes = ["Maria", "Sofia", "Leonor"];

nomes.length        // 3
nomes[0]             // "Maria"
nomes[nomes.length - 1]  // "Leonor" (último)
nomes[10]            // undefined (não dá erro)

nomes.push("Ana");   // adiciona ao final
nomes.pop();         // remove do final

// Iterar
for (let i = 0; i < nomes.length; i++) {
    console.log(nomes[i]);
}

nomes.forEach(n => console.log(n));
```

---

## 3.9 Objetos

```javascript
const aluno = {
    nome: "Ana",
    idade: 20,
    curso: "Informática",
    notas: [10, 15]
};

// Aceder
aluno.nome           // "Ana"
aluno["idade"]       // 20
aluno.notas[1]       // 15

// Alterar
aluno.idade = 21;

// Adicionar
aluno.aprovado = true;

// Array de objetos
const alunos = [
    { nome: "Ana", nota: 20 },
    { nome: "Maria", nota: 8 },
    { nome: "Carla", nota: 12 }
];

// Média das notas
let soma = 0;
alunos.forEach(a => soma += a.nota);
console.log(soma / alunos.length);  // 13.33
```

---

## 3.10 Strings

```javascript
const nome = "Ana";

nome.length              // 3
nome.toUpperCase()       // "ANA"
nome.toLowerCase()       // "ana"
nome[0]                  // "A"

// Strings são imutáveis
nome[0] = "Z";           // NÃO funciona, continua "Ana"

"  Sim  ".trim()         // "Sim" (remove espaços)
"Bem-vindo ao JS".includes("JS")  // true

// Comparações são case-sensitive
"Ana" === "ANA"          // false
"Ana".toUpperCase() === "ANA"  // true
```

---

# PARTE 4 — JavaScript: DOM e Interatividade

## 4.1 O que é o DOM

O **DOM** (Document Object Model) é a representação do HTML como uma **árvore de objetos** que o navegador cria. O JavaScript usa o DOM para ler, alterar, adicionar e remover elementos da página **sem recarregar**.

```
document
└── html
    ├── head
    │   └── title
    └── body
        ├── h1
        ├── p
        └── ul
            ├── li
            ├── li
            └── li
```

---

## 4.2 Seleção de elementos

| Método | Retorna | Exemplo |
|--------|---------|---------|
| `getElementById("id")` | 1 elemento | `document.getElementById("titulo")` |
| `querySelector("seletor")` | 1º que corresponde | `document.querySelector(".mensagem")` |
| `querySelectorAll("seletor")` | Todos (coleção) | `document.querySelectorAll("p")` |

```javascript
// Por ID
const titulo = document.getElementById("titulo");

// Por classe (primeiro que encontrar)
const msg = document.querySelector(".mensagem");

// Seletor CSS complexo
const p2 = document.querySelector("section > div > p:nth-of-type(2)");

// Todos os parágrafos
const paragrafos = document.querySelectorAll("p");
for (const p of paragrafos) {
    console.log(p.textContent);
}
```

---

## 4.3 Eventos

Eventos permitem que o JavaScript **reaja** a ações do utilizador.

### addEventListener

```javascript
const botao = document.getElementById("btnEnviar");

botao.addEventListener("click", tratarClique);

function tratarClique() {
    console.log("Botão clicado!");
}
```

### Eventos mais comuns

| Evento | Quando ocorre |
|--------|---------------|
| `click` | Clique num elemento |
| `input` | Valor de um campo vai sendo alterado (tecla a tecla) |
| `change` | Alteração de um campo fica concluída |
| `submit` | Formulário é submetido |
| `keydown` | Tecla é premida |
| `mouseover` | Rato passa sobre o elemento |

### O objeto `event`

Quando um evento ocorre, a função recebe um objeto `event` com informação sobre o que aconteceu:

```javascript
function tratarClique(event) {
    console.log(event.type);           // "click"
    console.log(event.currentTarget);  // o elemento que recebeu o evento
}
```

**`event.preventDefault()`** — impede o comportamento padrão (essencial em formulários para não recarregar a página).

---

## 4.4 Alteração dinâmica da página

### Alterar conteúdo

```javascript
const titulo = document.getElementById("titulo");

// Só texto
titulo.textContent = "Novo título";

// Com HTML (cuidado com conteúdo de utilizadores!)
titulo.innerHTML = "Título em <strong>negrito</strong>";
```

**Diferença:** `textContent` insere texto puro. `innerHTML` interpreta tags HTML.

### Alterar atributos

```javascript
const imagem = document.getElementById("foto");

// Diretamente
imagem.src = "nova-foto.png";
imagem.alt = "Descrição da nova foto";

// Com setAttribute
imagem.setAttribute("src", "nova-foto.png");
```

### Alterar classes CSS (forma preferencial de mudar estilos!)

```javascript
const elemento = document.getElementById("paraDestacar");

elemento.classList.add("red");        // adiciona classe
elemento.classList.remove("red");     // remove classe
elemento.classList.toggle("oculto");  // alterna (add/remove)
elemento.classList.contains("red");   // verifica → true/false
```

Exemplo de mostrar/ocultar:
```css
.oculto { display: none; }
```
```javascript
btnToggle.addEventListener("click", function() {
    painel.classList.toggle("oculto");
});
```

### Alterar estilos diretamente (usar com moderação)

```javascript
elemento.style.color = "red";
elemento.style.fontSize = "20px";
elemento.style.backgroundColor = "#f0f0f0";
```

**Nota:** As propriedades CSS com hífen (`font-size`) passam a camelCase em JS (`fontSize`).

---

## 4.5 Validação de formulários

### Padrão de validação

```javascript
const formulario = document.getElementById("meuForm");

formulario.addEventListener("submit", function(event) {
    // 1. Impedir o envio automático
    event.preventDefault();

    // 2. Ler os valores
    const nome = document.getElementById("nome").value;
    const email = document.getElementById("email").value;

    // 3. Validar
    if (nome.trim() === "") {
        resultado.textContent = "O nome é obrigatório.";
        return;  // para aqui, não continua
    }

    if (!email.includes("@")) {
        resultado.textContent = "Email inválido.";
        return;
    }

    // 4. Sucesso
    resultado.textContent = "Formulário válido!";
});
```

### Validação com múltiplos erros

```javascript
formulario.addEventListener("submit", function(event) {
    event.preventDefault();

    const erros = [];

    if (nome.value.trim() === "") {
        erros.push("O nome é obrigatório.");
    }
    if (password.value.length < 6) {
        erros.push("A password deve ter pelo menos 6 caracteres.");
    }
    if (password.value !== confirmacao.value) {
        erros.push("As passwords não coincidem.");
    }

    if (erros.length > 0) {
        let html = "<ul>";
        for (const erro of erros) {
            html += "<li>" + erro + "</li>";
        }
        html += "</ul>";
        mensagens.innerHTML = html;
    } else {
        mensagens.innerHTML = "<p>Registo válido!</p>";
    }
});
```

### Validação em tempo real (evento `input`)

```javascript
const campo = document.getElementById("utilizador");
const ajuda = document.getElementById("ajuda");

campo.addEventListener("input", function() {
    if (campo.value.trim().length < 4) {
        ajuda.textContent = "Deve ter pelo menos 4 caracteres.";
        ajuda.style.color = "red";
    } else {
        ajuda.textContent = "Nome válido.";
        ajuda.style.color = "inherit";
    }
});
```

---

## 4.6 Estado da aplicação

O **estado** é o conjunto de dados que representa a situação atual da aplicação. A ideia central:

1. **Evento** acontece (ex: clique)
2. **Estado** é alterado (variáveis JS)
3. **Interface** é atualizada (DOM)

```javascript
// Estado
const estado = {
    categoria: "todas",
    carrinho: []
};

// Função que atualiza o DOM a partir do estado
function atualizarInterface() {
    textoCategoria.textContent = "Categoria: " + estado.categoria;
    textoCarrinho.textContent = "Produtos: " + estado.carrinho.length;
}

// Evento muda o estado → atualiza interface
seletor.addEventListener("change", function() {
    estado.categoria = seletor.value;   // altera o estado
    atualizarInterface();                // atualiza o DOM
});

btnAdicionar.addEventListener("click", function() {
    estado.carrinho.push("Produto");    // altera o estado
    atualizarInterface();                // atualiza o DOM
});

// Inicializar
atualizarInterface();
```

**Porquê usar estado?** Em vez de alterar o DOM de forma dispersa, centralizas os dados num sítio e tens uma função que "desenha" a interface. Código mais organizado e fácil de manter.

---

# Checklist Final — Antes do Teste

### HTML
- [ ] Sei escrever a estrutura base de uma página HTML de memória
- [ ] Sei para que servem `charset`, `viewport`, `defer`
- [ ] Sei usar tags semânticas: `header`, `nav`, `main`, `section`, `article`, `footer`
- [ ] Sei a diferença entre `section` e `article`

### CSS — Seletores e Box Model
- [ ] Sei usar os 5 tipos de seletores (elemento, id, classe, agrupamento, descendente)
- [ ] Sei usar pseudo-classes (`:hover`, `:active`, etc.)
- [ ] Sei explicar o box model (margin, padding, border)
- [ ] Sei a diferença entre `px`, `em`, `rem`, `%`

### CSS — Layout
- [ ] Sei a diferença entre `block`, `inline` e `inline-block`
- [ ] Sei declarar e usar variáveis CSS
- [ ] Sei montar um layout com Flexbox (`display: flex`, `gap`, `justify-content`, `flex-wrap`)
- [ ] Sei criar uma grelha com Grid (`grid-template-columns: 1fr 1fr 1fr`)
- [ ] Sei escrever media queries para adaptar a mobile

### JavaScript — Fundamentos
- [ ] Sei a diferença entre `let`, `const` e `var`
- [ ] Sei a diferença entre `==` e `===`
- [ ] Sei o que são valores falsy
- [ ] Sei usar template literals
- [ ] Sei escrever funções, loops e condicionais
- [ ] Sei trabalhar com arrays (`.push()`, `.pop()`, `.forEach()`)
- [ ] Sei trabalhar com objetos e arrays de objetos

### JavaScript — DOM e Interatividade
- [ ] Sei selecionar elementos (`getElementById`, `querySelector`, `querySelectorAll`)
- [ ] Sei usar `addEventListener` para reagir a eventos
- [ ] Sei a diferença entre `textContent` e `innerHTML`
- [ ] Sei usar `classList` (`.add()`, `.remove()`, `.toggle()`)
- [ ] Sei validar um formulário com `submit` + `preventDefault()`
- [ ] Sei o que é o estado da aplicação e como o usar
