# Resumos — Algoritmos e Estruturas de Dados

> Recursividade · Listas · Pilhas · Filas · Árvores Genéricas · BST

---

## 1. Recursividade

Uma função é **recursiva** quando se chama a si própria. Toda função recursiva tem:

- **Caso base** — condição de paragem (sem isto → stack overflow)
- **Caso recursivo** — chamada a si própria com um subproblema mais pequeno

### Como funciona internamente

Cada chamada recursiva é colocada na **pilha de chamadas** (call stack). Quando o caso base é atingido, as chamadas resolvem-se de trás para a frente (LIFO).

### Exemplos fundamentais

**Soma dos dígitos de um número:**
```c
int somaDigitos(int n) {
    if (n == 0) return 0;
    return (n % 10) + somaDigitos(n / 10);
}
// somaDigitos(1234) → 4 + 3 + 2 + 1 = 10
```

**Soma multiplicada pela posição:**
```c
int somaMultiplicada(int vetor[], int tamanho, int pos) {
    if (pos == tamanho) return 0;
    return vetor[pos] * pos + somaMultiplicada(vetor, tamanho, pos + 1);
}
```

**Imprimir de 0 até N:**
```c
void imprimirAteN(int atual, int N) {
    if (atual > N) return;
    cout << atual << " ";
    imprimirAteN(atual + 1, N);
}
```

---

## 2. Listas

### Lista simplesmente ligada

Cada nodo contém um **valor** e um ponteiro para o **próximo** nodo.

```
[valor|próx] → [valor|próx] → [valor|NULL]
```

- Travessia apenas num sentido (início → fim)
- Inserção/remoção no início: **O(1)**
- Pesquisa: **O(n)** — percorrer nodo a nodo

### Lista duplamente ligada

Cada nodo contém **anterior**, **valor** e **próximo**.

```
NULL ← [ant|valor|próx] ⇄ [ant|valor|próx] ⇄ [ant|valor|próx] → NULL
```

- Travessia nos dois sentidos
- **Acesso rápido a ambas as extremidades** — ideal para filas
- Mais memória por nodo (dois ponteiros em vez de um)

### Quando usar qual?

| Critério | Simples | Dupla |
|----------|---------|-------|
| Memória limitada | ✅ | ❌ |
| Travessia bidirecional | ❌ | ✅ |
| Acesso a ambas as extremidades | ❌ | ✅ |
| Remoção de nodo conhecido | O(n) | O(1) |

---

## 3. Pilhas (Stack)

**Princípio: LIFO** — Last In, First Out.

Imaginar uma pilha de pratos: só se tira o de cima.

### Operações

| Operação | Descrição | Complexidade |
|----------|-----------|--------------|
| `push(x)` | Colocar elemento no topo | O(1) |
| `pop()` | Remover elemento do topo | O(1) |
| `peek()` / `top()` | Ver o topo sem remover | O(1) |
| `isEmpty()` | Verificar se está vazia | O(1) |

### Aplicações

- Pilha de chamadas recursivas
- Verificação de parênteses balanceados
- Undo/Redo
- Avaliação de expressões pós-fixas

### Exemplo manual

```
push(1) → [1]
push(2) → [1, 2]
push(3) → [1, 2, 3]
pop()   → [1, 2]       (removeu 3)
peek()  → 2            (topo atual)
```

---

## 4. Filas (Queue)

**Princípio: FIFO** — First In, First Out.

Imaginar uma fila de supermercado: o primeiro a chegar é o primeiro a ser atendido.

### Operações

| Operação | Descrição | Complexidade |
|----------|-----------|--------------|
| `enqueue(x)` | Inserir no final | O(1) |
| `dequeue()` | Remover do início | O(1) |
| `front()` | Ver o primeiro sem remover | O(1) |
| `isEmpty()` | Verificar se está vazia | O(1) |

### Aplicações

- Escalonamento de processos
- BFS (pesquisa em largura) em grafos/árvores
- Buffers de impressão

### Pilha vs Fila — não confundir

| | Pilha | Fila |
|--|-------|------|
| Princípio | LIFO | FIFO |
| Insere em | topo | final |
| Remove de | topo | início |
| Analogia | pilha de pratos | fila de supermercado |

---

## 5. Árvores Genéricas

Estrutura hierárquica composta por **nodos** ligados por arestas.

### Terminologia

| Termo | Definição |
|-------|-----------|
| **Raiz** | Nodo sem pai (topo da árvore) |
| **Folha** | Nodo sem filhos |
| **Pai** | Nodo diretamente acima |
| **Filho** | Nodo diretamente abaixo |
| **Altura** | Distância da raiz até à folha mais profunda |
| **Profundidade** | Distância de um nodo até à raiz |
| **Nível** | Conjunto de nodos à mesma profundidade |

### Percursos (recursivos)

- **Pré-ordem:** raiz → filhos (esquerda para direita)
- **Pós-ordem:** filhos → raiz

> **A árvore é a estrutura que usa recursividade para percorrer os seus nodos.**

### Representação

- Filho mais à esquerda + irmão à direita
- Cada nodo: `valor` + `primeiro_filho` + `próximo_irmão`

---

## 6. Árvores Binárias de Pesquisa (BST)

Árvore binária onde cada nodo obedece à regra:
- **Esquerda < Nodo < Direita**

### Pesquisa

1. Começar na raiz
2. Se valor == nodo → encontrado
3. Se valor < nodo → ir para a esquerda
4. Se valor > nodo → ir para a direita
5. Se nodo == NULL → não existe

Complexidade: **O(h)** onde h = altura da árvore.

### Inserção

Seguir o mesmo caminho da pesquisa; quando chegar a NULL, inserir lá.

### Remoção — 3 casos

1. **Folha** → remover diretamente
2. **Um filho** → substituir o nodo pelo seu único filho
3. **Dois filhos** → substituir pelo **sucessor in-order** (menor valor da subárvore direita)

### Percursos

| Percurso | Ordem | Resultado |
|----------|-------|-----------|
| **In-order** | esquerda → raiz → direita | Valores **ordenados crescente** |
| **Pre-order** | raiz → esquerda → direita | Útil para copiar a árvore |
| **Post-order** | esquerda → direita → raiz | Útil para eliminar a árvore |

### Exemplo — inserir: `18, 9, 4, 23, 41, 6, 15, 32`

```
          18
         /  \
        9    23
       / \     \
      4   15    41
       \       /
        6    32
```

**In-order:**   `4, 6, 9, 15, 18, 23, 32, 41`
**Pre-order:**  `18, 9, 4, 6, 15, 23, 41, 32`
**Post-order:** `6, 4, 15, 9, 32, 41, 23, 18`

### Caso degenerado

Se inserir valores já ordenados (`1, 2, 3, 4, 5`), a BST degenera numa **lista ligada** com altura O(n).

---

## 7. Particionamento Espacial

Não confundir com BST:

| Estrutura | Dimensões | Uso |
|-----------|-----------|-----|
| **Quadtree** | 2D | Divide espaço em 4 quadrantes |
| **Octree** | 3D | Divide espaço em 8 octantes |

Usado para simulação de física, deteção de colisões, jogos.

---

## Referência Rápida — Escolha Múltipla

| Pergunta | Resposta |
|----------|----------|
| Estrutura que usa recursividade para percorrer nodos? | **e) Árvores** |
| Quando preferir lista dupla em vez de simples? | **b) Acesso rápido a ambas as extremidades** |
| Estrutura útil para particionamento espacial? | **c) Quadtrees** (2D) / **d) Octrees** (3D) |
