# Plano de Estudo — Teste de Programação Web

## Ficheiros de Estudo
- `template-1.html`, `template-2.html`, `template-3.html` → estrutura HTML base
- `styles-1.css`, `styles-2.css` → CSS progressivo
- `js-1-fundamentos.html` → fundamentos de JavaScript
- `js-2-dom.html` → DOM, eventos, formulários, estado

---

## MÓDULO 1 — HTML: Estrutura e Semântica
**Ficheiros:** template-1.html → template-2.html → template-3.html

### O que estudar
- Estrutura mínima de um documento HTML (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`)
- Elementos do `<head>`: `<meta charset>`, `<meta viewport>`, `<title>`, `<link>` (CSS), `<script>` (JS)
- **Semântica**: `<header>`, `<nav>`, `<main>`, `<footer>`, `<section>`, `<article>`
- Boas práticas: indentação, comentários, organização de ficheiros (`css/`, `js/`, `assets/`)

### Perguntas para testar
1. Qual é a diferença entre `<section>` e `<article>`?
2. Onde colocar o `<script>` e porquê? (antes de `</body>`)
3. Para que serve `<meta name="viewport">`?

---

## MÓDULO 2 — CSS: Seletores, Box Model e Unidades
**Ficheiro:** styles-1.css (primeira metade)

### O que estudar
- **Seletores**: por elemento (`h1`), por id (`#id`), por classe (`.classe`), descendente (`nav a`), agrupamento (`h1, h2`)
- **Pseudo-classes**: `:link`, `:visited`, `:hover`, `:active`
- **Box Model**: `margin`, `padding`, `border`, `border-radius`
- **Unidades**: `px`, `em`, `rem`, `%`
- `max-width: 100%` para imagens responsivas

### Perguntas para testar
1. Qual a diferença entre `margin` e `padding`?
2. O que é `margin: 2em auto`? (centralizar horizontalmente)
3. Diferença entre `em` e `rem`?
4. Como selecionar apenas links dentro de `<main>`?

---

## MÓDULO 3 — CSS: Display, Flexbox, Grid e Media Queries
**Ficheiro:** styles-1.css (segunda metade) + styles-2.css

### O que estudar
- **Display**: `block`, `inline`, `inline-block` — diferenças e quando usar
- **CSS Variables** (`--nome-variavel`, `:root`, `var()`) — evitar repetição, consistência
- **Flexbox**:
  - `display: flex`, `gap`, `flex-wrap`, `flex-direction`
  - `justify-content`: `flex-start`, `center`, `space-between`
  - `flex-basis`, `flex-grow`
- **Media Queries**: `@media (max-width: 600px)`, `@media (prefers-color-scheme: dark)`
- **Grid**: `display: grid`, `grid-template-columns`, `1fr`, `gap`
- **Helper classes**: `.centrado`, `.negrito`

### Perguntas para testar
1. O que faz `display: inline-block` que `inline` não consegue?
2. Como centrar items num flex container horizontalmente? (`justify-content: center`)
3. Como fazer um grid de 3 colunas iguais? (`grid-template-columns: 1fr 1fr 1fr`)
4. Como adaptar o layout para mobile com media query?
5. Como declarar e usar uma variável CSS?

---

## MÓDULO 4 — JavaScript: Fundamentos
**Ficheiro:** js-1-fundamentos.html

### O que estudar
#### Como executar JS
- Inline em atributos HTML (evitar)
- `<script>` dentro do HTML
- Ficheiro externo (preferencial)

#### Variáveis e Tipos
- `var`, `let`, `const` — diferenças e boas práticas (`const` por defeito, `let` quando varia)
- Tipos: `string`, `number`, `boolean`, `null`, `undefined`

#### Operadores
- Aritméticos: `+`, `-`, `*`, `/`, `%`
- Atribuição: `=`, `+=`, `-=`
- Incremento/decremento: `++`, `--`
- Comparação: `==` vs `===` (preferir `===`), `!=`, `!==`, `<`, `>`
- Lógicos: `&&`, `||`, `!`

#### Conversão de Tipos
- `Number()`, `parseInt()`, `parseFloat()`
- `String()`, template literals (`` `Olá ${nome}` ``)
- `Boolean()` — valores falsy: `0`, `""`, `null`, `undefined`, `NaN`, `false`

#### Condicionais
- `if / else if / else`

#### Repetição
- `for`, `while`
- `forEach` em arrays

#### Funções
- Declaração: `function nome(params) { }`
- Arrow functions: `const nome = (params) => { }`

#### Arrays
- Criar, aceder, `.push()`, `.pop()`, `.length`
- Iterar com `for` e `forEach`

#### Objetos
- `{ chave: valor }`, aceder com `.chave` ou `["chave"]`
- Arrays de objetos

#### Strings
- `.length`, `.toUpperCase()`, `.toLowerCase()`, `.includes()`, `.split()`, `.trim()`

#### Scope
- Variáveis locais vs globais

### Perguntas para testar
1. Diferença entre `==` e `===`?
2. O que é um valor "falsy"?
3. Como criar uma arrow function?
4. Como iterar um array com `forEach`?
5. Como aceder à propriedade `nome` de um objeto `pessoa`?

---

## MÓDULO 5 — JavaScript: DOM, Eventos e Formulários
**Ficheiro:** js-2-dom.html

### O que estudar
#### DOM
- O que é o DOM (Document Object Model) — árvore de nós
- Para que serve: manipular estrutura/conteúdo/estilos da página

#### Seleção de Elementos
- `getElementById("id")` → 1 elemento por id
- `querySelector("seletor CSS")` → 1º elemento que corresponde
- `querySelectorAll("seletor CSS")` → NodeList com todos

#### Eventos
- `addEventListener("evento", função)`
- Eventos comuns: `click`, `input`, `submit`, `change`, `keydown`
- O objeto `event` (`event.target`, `event.preventDefault()`)

#### Alteração Dinâmica
- Conteúdo: `elemento.textContent`, `elemento.innerHTML`
- Atributos: `elemento.getAttribute()`, `elemento.setAttribute()`
- Classes: `classList.add()`, `classList.remove()`, `classList.toggle()`, `classList.contains()`
- Estilos: `elemento.style.propriedade = "valor"`

#### Validação de Formulários
- Evento `submit` + `event.preventDefault()`
- Ler valores: `input.value`
- Mostrar mensagens de erro no DOM
- Validação em tempo real com evento `input`

#### Estado da Aplicação
- O que é o estado (dados que a aplicação precisa de guardar)
- Representar estado em variáveis/objetos
- Atualizar a interface a partir do estado

### Perguntas para testar
1. Diferença entre `querySelector` e `querySelectorAll`?
2. Como impedir que um formulário faça submit para o servidor?
3. Como adicionar/remover uma classe a um elemento?
4. Diferença entre `textContent` e `innerHTML`?
5. O que é o estado de uma aplicação? Dá um exemplo.

---

## Ordem de Estudo Recomendada

| Ordem | Tema | Ficheiro |
|-------|------|----------|
| 1 | Estrutura HTML | template-1 → 2 → 3 |
| 2 | CSS Seletores + Box Model | styles-1.css (início) |
| 3 | CSS Flexbox + Grid + Media Queries | styles-1.css (fim) + styles-2.css |
| 4 | JS Fundamentos | js-1-fundamentos.html |
| 5 | JS DOM + Eventos + Formulários | js-2-dom.html |

---

## Checklist Antes do Teste
- [ ] Sei criar a estrutura HTML semântica de raiz
- [ ] Sei aplicar seletores CSS (elemento, id, classe, descendente, pseudo-classes)
- [ ] Sei usar Flexbox para alinhar elementos
- [ ] Sei criar media queries para mobile
- [ ] Sei declarar variáveis e usar condicionais/loops em JS
- [ ] Sei selecionar elementos DOM e modificar conteúdo/classes
- [ ] Sei adicionar event listeners
- [ ] Sei validar um formulário com JS
