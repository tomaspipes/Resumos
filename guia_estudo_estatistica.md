# 📊 GUIA DE ESTUDO — ESTATÍSTICA
### Baseado no Primeiro Teste - Prova tipo (LEIF004ON1)

---

## 1. NATUREZA DOS DADOS

### O que são dados e a sua natureza?

Os dados recolhidos numa investigação são classificados de acordo com a sua **natureza** (ou tipo de escala de medida). Esta classificação é fundamental porque determina:
- Que representações gráficas se podem utilizar
- Que medidas estatísticas fazem sentido calcular

---

### 1.1 Dados Qualitativos (Categóricos)

São dados que representam **categorias** ou **grupos**. Não têm significado numérico intrínseco, mesmo que sejam codificados com números.

#### 1.1.1 Nominais
- As categorias **não têm ordem** entre si.
- Os números atribuídos são apenas etiquetas.
- Exemplos do teste:
  - **Sistema de entrega preferido**: 0 = Entrega padrão, 1 = Entrega expresso
- Outros exemplos: género, cor dos olhos, país de origem

> ⚠️ Mesmo que o valor seja "0" ou "1", o facto de 1 > 0 **não tem significado**. São apenas rótulos.

#### 1.1.2 Ordinais
- As categorias **têm uma ordem natural** entre si, mas as diferenças entre categorias **não são mensuráveis** de forma igual.
- Exemplos do teste:
  - **Antiguidade do cliente**: 1 = Novos, 2 = Atuais, 3 = Antigos → existe uma ordem (antigos > atuais > novos), mas a diferença entre "novo" e "atual" não é necessariamente igual à diferença entre "atual" e "antigo".
- Outros exemplos: nível de escolaridade, grau de satisfação numa escala de Likert.

---

### 1.2 Dados Quantitativos (Numéricos)

São dados que representam **quantidades** e onde as operações aritméticas fazem sentido.

#### 1.2.1 Discretos
- Resultam de **contagens**.
- Tomam valores **inteiros**; não podem assumir valores intermédios.
- Exemplos do teste:
  - **Nº de reclamações no último trimestre**: 0, 1, 2, 3... (não pode haver 2,5 reclamações)
- Outros exemplos: nº de filhos, nº de defeitos.

#### 1.2.2 Contínuos
- Resultam de **medições**.
- Podem assumir **qualquer valor** dentro de um intervalo.
- Exemplos do teste:
  - **Imagem do departamento de vendas** (escala 0 a 10)
  - **Satisfação com o serviço** (escala 0 a 10)
  - **Intenção de recomendação** (escala 0 a 10)
- Outros exemplos: altura, peso, temperatura.

---

### Tabela-Resumo: Natureza dos Dados

| Tipo | Subtipo | Ordem | Distância mensurável | Exemplos do teste |
|------|---------|:-----:|:-------------------:|-------------------|
| Qualitativo | Nominal | ❌ | ❌ | Sistema de entrega preferido |
| Qualitativo | Ordinal | ✅ | ❌ | Antiguidade do cliente |
| Quantitativo | Discreto | ✅ | ✅ | Nº de reclamações |
| Quantitativo | Contínuo | ✅ | ✅ | Satisfação, Imagem, Intenção de recomendação |

---

## 2. REPRESENTAÇÕES GRÁFICAS

A escolha da representação gráfica depende **sempre** da natureza dos dados.

---

### 2.1 Gráfico de Barras

- Utilizado para variáveis **nominais**, **ordinais** e **quantitativas discretas**.
- Cada barra representa uma categoria/valor e a sua altura corresponde à frequência (absoluta ou relativa).
- As barras têm **espaçamento** entre si (ao contrário do histograma).
- **Quando usar:** Quando os dados são categorias ou contagens de valores específicos.
- Exemplos: distribuição do sistema de entrega preferido; distribuição do nº de reclamações.

---

### 2.2 Gráfico Circular / Diagrama de Setores

- Utilizado para variáveis **nominais** (e por vezes ordinais).
- Mostra a **proporção** de cada categoria em relação ao total.
- **Limitação:** Difícil de comparar quando há muitas fatias ou valores similares.
- **Quando usar:** Para mostrar a composição de um todo.

---

### 2.3 Histograma

- Utilizado para variáveis **quantitativas contínuas**.
- As barras são **adjacentes** (sem espaço entre elas) porque representam intervalos contínuos.
- O eixo X representa os **intervalos de classe** e o eixo Y a **frequência**.
- **Quando usar:** Para visualizar a distribuição de uma variável contínua e identificar a forma da distribuição.
- Exemplo: distribuição da "Satisfação com o serviço" (0 a 10).

> 🔑 Diferença-chave: **Barras = espaço entre elas** (dados discretos/qualitativos) vs **Histograma = sem espaço** (dados contínuos).

---

### 2.4 Box Plot (Diagrama de Caixa)

- Representa graficamente as **medidas de ordem** (quartis, mínimo, máximo).
- Útil para variáveis **quantitativas**.
- Permite identificar: mediana, dispersão, assimetria e **outliers**.
- **Quando usar:** Para comparar distribuições e identificar outliers.

---

### 2.5 Diagrama de Dispersão (Scatter Plot)

- Representa pares de valores (x, y) de **duas variáveis quantitativas**.
- Utilizado para estudar a **relação/associação** entre duas variáveis.
- **Quando usar:** Para analisar correlação entre duas variáveis numéricas.
- Exemplo: relação entre "Satisfação com o serviço" e "Intenção de recomendação".

---

### Tabela-Resumo: Qual Gráfico Usar?

| Natureza dos Dados | Representação Gráfica Adequada |
|--------------------|-------------------------------|
| Nominal | Gráfico de barras, Gráfico circular |
| Ordinal | Gráfico de barras |
| Quantitativo Discreto | Gráfico de barras |
| Quantitativo Contínuo | Histograma, Box Plot |
| Relação entre 2 variáveis quantitativas | Diagrama de dispersão |

---

## 3. MEDIDAS DE LOCALIZAÇÃO CENTRAL

As medidas de localização central procuram **resumir** um conjunto de dados num único valor representativo.

---

### 3.1 Moda

- O valor (ou intervalo) que **ocorre com maior frequência**.
- **Possível para:** todos os tipos de dados (nominal, ordinal, quantitativo).
- **Quando é a única opção válida:** dados **nominais**.
- Pode haver uma moda (unimodal), duas modas (bimodal) ou nenhuma.

---

### 3.2 Mediana

- O valor que **divide a distribuição em duas metades iguais** (50% dos valores abaixo, 50% acima).
- **Possível para:** dados **ordinais** e **quantitativos**.
- **Não faz sentido para:** dados nominais (não há ordem).
- **Vantagem:** Não é influenciada por valores extremos (outliers).
- **Cálculo:**
  - Se n for ímpar: posição = (n+1)/2
  - Se n for par: média dos valores nas posições n/2 e n/2 + 1

---

### 3.3 Média Aritmética

- Soma de todos os valores dividida pelo nº de observações:

```
x̄ = (x₁ + x₂ + ... + xₙ) / n
```

- **Possível para:** apenas dados **quantitativos** (discretos ou contínuos).
- **Não faz sentido para:** dados nominais e ordinais (operações aritméticas sem significado).
- **Desvantagem:** É fortemente influenciada por **outliers**.

---

### Tabela-Resumo: Medidas de Localização Central

| Medida | Nominal | Ordinal | Quantitativo Discreto | Quantitativo Contínuo |
|--------|:-------:|:-------:|:--------------------:|:--------------------:|
| Moda | ✅ | ✅ | ✅ | ✅ |
| Mediana | ❌ | ✅ | ✅ | ✅ |
| Média | ❌ | ❌ | ✅ | ✅ |

---

### 3.4 Média vs Mediana vs Moda: Qual usar?

A escolha depende da **forma da distribuição**:

- **Distribuição simétrica** → Média ≈ Mediana ≈ Moda → usar **média** (mais eficiente).
- **Distribuição assimétrica** → Média ≠ Mediana → usar **mediana** (mais robusta ao enviesamento).

> ⚠️ Uma distribuição assimétrica **não implica necessariamente a existência de outliers**. A assimetria resulta de uma cauda mais longa de um dos lados da distribuição — pode ocorrer sem nenhum valor extremo isolado. Os outliers podem agravar a assimetria, mas não são a sua causa obrigatória.

**Como detetar assimetria comparando as três medidas:**

| Relação | Tipo de assimetria | O que acontece no gráfico |
|---------|-------------------|--------------------------|
| Moda > Mediana > Média | **Assimetria negativa** (cauda à esquerda) | O pico (moda) está à direita; a cauda puxa a média para baixo |
| Moda ≈ Mediana ≈ Média | **Distribuição simétrica** | O pico está ao centro; ambos os lados são iguais |
| Média > Mediana > Moda | **Assimetria positiva** (cauda à direita) | O pico (moda) está à esquerda; a cauda puxa a média para cima |

**Leitura intuitiva:**
- A **moda** indica o **pico** da distribuição (onde os dados se concentram mais).
- A **mediana** indica o **centro exato** (divide os dados em dois grupos iguais).
- A **média** é "puxada" para o lado da **cauda** — é a mais sensível a valores extremos.

Quanto maior a diferença entre estas três medidas, mais pronunciada é a assimetria.

> 📌 Se o Coeficiente de Variação (CV) for elevado (> 30%), a média está enviesada e a mediana é mais adequada.

---

## 4. TABELA DE FREQUÊNCIAS

---

### 4.1 Conceitos-Chave

| Conceito | Símbolo | Definição |
|----------|---------|-----------|
| Frequência Absoluta | fᵢ | Nº de vezes que o valor/classe ocorre |
| Frequência Relativa | frᵢ | Proporção: fᵢ / n |
| Frequência Relativa (%) | frᵢ% | frᵢ × 100 |
| Frequência Acumulada | Fᵢ | Soma das frequências absolutas até à classe i |
| Frequência Relativa Acumulada | Frᵢ | Fᵢ / n |

---

### 4.2 Como Construir uma Tabela de Frequências

**Para variáveis discretas (ex: nº de reclamações):**

1. Listar todos os valores possíveis.
2. Contar quantas vezes cada valor aparece → frequência absoluta (fᵢ).
3. Dividir pelo total n → frequência relativa (frᵢ).
4. Somar cumulativamente → frequência acumulada (Fᵢ).
5. Dividir Fᵢ por n → frequência relativa acumulada (Frᵢ).

**Exemplo (hipotético para nº reclamações, n=200):**

| Nº Reclamações | fᵢ | frᵢ | frᵢ% | Fᵢ | Frᵢ |
|:-:|:-:|:-:|:-:|:-:|:-:|
| 0 | 40 | 0,200 | 20,0% | 40 | 0,200 |
| 1 | 50 | 0,250 | 25,0% | 90 | 0,450 |
| 2 | 45 | 0,225 | 22,5% | 135 | 0,675 |
| 3 | 35 | 0,175 | 17,5% | 170 | 0,850 |
| 4 | 20 | 0,100 | 10,0% | 190 | 0,950 |
| 5 | 10 | 0,050 | 5,0% | 200 | 1,000 |
| **Total** | **200** | **1,000** | **100%** | — | — |

---

### 4.3 Erros Comuns

1. **Frequências relativas não somam 1 (ou 100%)** → Erro de cálculo; verificar divisões.
2. **Frequências acumuladas não terminam em n (ou 1)** → Erro na soma cumulativa.
3. **Intervalos sobrepostos** → Ex: [0-2] e [2-4] — o valor 2 aparece em ambos; correto: [0-2[ e [2-4[.
4. **Intervalos com amplitude diferente** → Torna o histograma enganador.
5. **Omissão de valores com frequência zero** → Falha na representação completa.
6. **Confundir frequência absoluta com relativa** → fᵢ soma n; frᵢ soma 1.

---

### 4.4 Percentagem de Clientes sem Queixas

```
% clientes sem queixas = (f₀ / n) × 100 = frᵢ% do valor 0
```

---

## 5. QUARTIS

Os quartis são **medidas de ordem** que dividem a distribuição em quatro partes iguais.

---

### 5.1 Definição dos Quartis

| Quartil | Símbolo | O que representa |
|---------|---------|-----------------|
| Primeiro Quartil | Q1 | 25% dos dados são ≤ a este valor |
| Segundo Quartil (Mediana) | Q2 | 50% dos dados são ≤ a este valor |
| Terceiro Quartil | Q3 | 75% dos dados são ≤ a este valor |

---

### 5.2 Como Calcular os Quartis

**Posições:**
- Q1: posição = (n+1) × 0,25
- Q2: posição = (n+1) × 0,50
- Q3: posição = (n+1) × 0,75

Se a posição for decimal (ex: 50,25), interpola-se:
```
Qₖ = valor_inferior + parte_decimal × (valor_superior - valor_inferior)
```

**Usando a tabela de frequências acumuladas:**
- Q1 → primeiro valor cuja Frᵢ ≥ 0,25
- Q2 → primeiro valor cuja Frᵢ ≥ 0,50
- Q3 → primeiro valor cuja Frᵢ ≥ 0,75

---

### 5.3 Como Interpretar os Quartis em Contexto

**Modelo de interpretação:**

- **Q1 = x** → "25% dos clientes têm [variável] igual ou inferior a x."
- **Q2 = x** → "Metade dos clientes (50%) têm [variável] igual ou inferior a x."
- **Q3 = x** → "75% dos clientes têm [variável] igual ou inferior a x. Apenas 25% dos clientes têm [variável] superior a x."

**Exemplo no contexto do teste (nº reclamações, valores hipotéticos):**
- Q1 = 1 → "25% dos clientes apresentaram 1 ou menos reclamações no último trimestre."
- Q2 = 2 → "Metade dos clientes apresentaram 2 ou menos reclamações no último trimestre."
- Q3 = 4 → "75% dos clientes apresentaram 4 ou menos reclamações. Apenas 1 em cada 4 clientes apresentou mais de 4 reclamações."

---

### 5.4 Amplitude Interquartil (IQR)

```
IQR = Q3 - Q1
```

- Representa a dispersão dos **50% centrais** dos dados.
- É robusta a outliers.
- Usada para calcular os limites dos outliers no box plot.

---

## 6. HISTOGRAMA E BOX PLOT — COMO INTERPRETAR

---

### 6.1 Interpretação do Histograma

#### 6.1.1 Classe Modal
- A barra mais alta = classe com **maior frequência** (classe modal).
- A frequência percentual da classe modal lê-se diretamente no eixo Y.

#### 6.1.2 Forma da Distribuição
- **Simétrica:** Padrão em sino; média ≈ mediana.
- **Assimétrica positiva (enviesada à direita):** Cauda longa para a direita; média > mediana.
- **Assimétrica negativa (enviesada à esquerda):** Cauda longa para a esquerda; média < mediana.

#### 6.1.3 O que extrair de um histograma
- Classe modal (intervalo mais frequente).
- Forma da distribuição (simetria/assimetria).
- Amplitude dos dados (valor mínimo e máximo visíveis).
- Concentração dos dados.

---

### 6.2 Interpretação do Box Plot (Diagrama de Caixa)

```
     |<----- IQR ------>|
     ┌─────────┬─────────┐
─────┤   Q1    │Q2    Q3 ├─────     × outlier
     └─────────┴─────────┘
  ▲                        ▲
Bigode inferior       Bigode superior
```

| Elemento | O que representa |
|----------|-----------------|
| Linha dentro da caixa | Mediana (Q2) |
| Extremo esquerdo da caixa | Q1 (25º percentil) |
| Extremo direito da caixa | Q3 (75º percentil) |
| Largura da caixa | IQR = Q3 - Q1 |
| Bigodes (whiskers) | Extensão até ao mínimo/máximo (excluindo outliers) |
| Pontos fora dos bigodes (×) | Outliers |

#### 6.2.1 Como Identificar Outliers pelo Box Plot

**Passo 1 — Calcular os limites teóricos:**
```
Limite inferior = Q1 - 1,5 × IQR
Limite superior = Q3 + 1,5 × IQR
```

**Passo 2 — Comparar os limites com os valores reais (mínimo e máximo da tabela/dados):**
- Se o **mínimo real** < limite inferior → o mínimo é **outlier**; o bigode esquerdo estende-se até ao **menor valor real que ainda está dentro do limite**.
- Se o **máximo real** > limite superior → o máximo é **outlier**; o bigode direito estende-se até ao **maior valor real que ainda está dentro do limite**.
- Se os valores reais estiverem todos dentro dos limites → não existem outliers; os bigodes chegam ao mínimo e máximo reais.

> ⚠️ Os limites (Q1 − 1,5×IQR e Q3 + 1,5×IQR) são **valores teóricos de corte** — não são necessariamente valores que existem nos dados. O que se classifica como outlier é qualquer **valor real** da tabela que ultrapasse esses limites.

**Exemplo:** Q1 = 4, Q3 = 7, IQR = 3
```
Limite inferior = 4 - 1,5 × 3 = -0,5
Limite superior = 7 + 1,5 × 3 = 11,5
```
- Se o mínimo real for 1 → 1 > -0,5 → não é outlier; bigode esquerdo vai até 1.
- Se o máximo real for 14 → 14 > 11,5 → **é outlier**; bigode direito vai até ao maior valor real ≤ 11,5.

#### 6.2.2 Assimetria no Box Plot
- **Simétrica:** Mediana centrada na caixa; bigodes iguais.
- **Assimetria positiva:** Mediana mais próxima de Q1; bigode direito mais longo.
- **Assimetria negativa:** Mediana mais próxima de Q3; bigode esquerdo mais longo.

---

### 6.3 Coeficiente de Variação (CV)

```
CV = (desvio-padrão / média) × 100%
```

| CV | Dispersão |
|----|-----------|
| < 15% | Baixa (distribuição homogénea) |
| 15% a 30% | Moderada |
| > 30% | **Elevada** (distribuição heterogénea; média pode não ser representativa) |

---

### 6.4 Leitura Conjunta Histograma + Box Plot

| O que ver | Histograma | Box Plot |
|-----------|------------|---------|
| Centro | Barra mais alta (moda) | Linha da mediana |
| Dispersão | Largura das barras | Largura da caixa (IQR) |
| Forma | Simetria/assimetria visual | Posição da mediana na caixa |
| Outliers | Não mostra diretamente | Pontos fora dos bigodes |

---

## 7. DIAGRAMA DE DISPERSÃO E COEFICIENTE DE CORRELAÇÃO DE PEARSON

---

### 7.1 Diagrama de Dispersão

- Representa pares de valores (X, Y); cada ponto = uma observação.
- Permite **visualizar a relação** entre duas variáveis quantitativas.
- Eixo X: variável independente (ex: satisfação com o serviço).
- Eixo Y: variável dependente (ex: intenção de recomendação).

---

### 7.2 Tipos de Associação

#### Associação Positiva
- Quando X aumenta, Y também tende a aumentar.
- Nuvem de pontos inclinada **para cima** (da esquerda para a direita).
- Exemplo: satisfação ↑ → intenção de recomendar ↑

#### Associação Nula (Sem Associação)
- Não existe padrão; pontos dispersos **aleatoriamente**.
- X e Y não têm relação linear.

#### Associação Negativa
- Quando X aumenta, Y tende a diminuir.
- Nuvem de pontos inclinada **para baixo** (da esquerda para a direita).
- Exemplo: preço ↑ → quantidade vendida ↓

---

### 7.3 Coeficiente de Correlação Linear de Pearson (r)

Quantifica a **força e direção** da associação linear entre duas variáveis.

#### 7.3.1 Fórmula

```
r = Cov(X,Y) / (s_X × s_Y)
```

Onde:
- **Cov(X,Y)** = covariância entre X e Y
- **s_X** = desvio-padrão de X
- **s_Y** = desvio-padrão de Y

**Resolução da Pergunta 4 do teste:**
```
r = 1,02 / (1,241 × 1,083)
r = 1,02 / 1,343643
r ≈ 0,759
```

#### 7.3.2 Propriedades de r

- Varia sempre entre -1 e +1
- r > 0: associação positiva
- r < 0: associação negativa
- r = 0: ausência de correlação linear
- r = +1 ou r = -1: correlação linear perfeita

#### 7.3.3 Interpretação da Intensidade

| Valor absoluto |r| | Intensidade |
|:---:|---|
| 0,00 – 0,19 | Muito fraca (ou nula) |
| 0,20 – 0,39 | Fraca |
| 0,40 – 0,69 | Moderada |
| 0,70 – 0,89 | **Forte** |
| 0,90 – 1,00 | Muito forte |

**Interpretação completa do exemplo do teste (r ≈ 0,759):**
"Existe uma correlação linear **positiva** e de intensidade **forte** entre a satisfação com o serviço e a intenção de recomendação. Clientes com maior satisfação tendem a ter maior intenção de recomendar a empresa."

#### 7.3.4 Atenção!
- **Correlação não implica causalidade.**
- O coeficiente de Pearson mede apenas relações **lineares**. Pode existir relação não-linear com r ≈ 0.

---

## 8. PROBABILIDADES

---

### 8.1 Conceitos Fundamentais

| Conceito | Definição |
|----------|-----------|
| Espaço amostral (Ω) | Conjunto de todos os resultados possíveis |
| Acontecimento (A) | Subconjunto do espaço amostral |
| Probabilidade P(A) | Número entre 0 e 1 que mede a "chance" de A ocorrer |

```
0 ≤ P(A) ≤ 1
P(Ω) = 1
P(∅) = 0
```

---

### 8.2 Acontecimento Complementar

O complementar de A (lê-se "não A") — quando A **não** ocorre:

```
P(Aᶜ) = 1 - P(A)
```

**Exemplo — Pergunta 5 do teste:**
```
P(não emite hidrocarbonetos) = 1 - P(emite hidrocarbonetos)
                              = 1 - 0,15
                              = 0,85
```
**Resposta: 0,85** ✅

---

### 8.3 União de Acontecimentos — Regra da Adição

Probabilidade de ocorrer A **ou** B (ou ambos):

```
P(A ∪ B) = P(A) + P(B) - P(A ∩ B)
```

O termo P(A ∩ B) é subtraído para não **contar duas vezes** os casos em que ambos ocorrem.

**Exemplo — Pergunta 6 do teste:**

Dados:
- H = "emite hidrocarbonetos em excesso" → P(H) = 0,15
- C = "emite monóxido de carbono em excesso" → P(C) = 0,12
- P(H ∩ C) = "emite ambos em excesso" = 0,08

```
P(H ∪ C) = 0,15 + 0,12 - 0,08 = 0,19
```

**Resposta: 0,19** ✅

---

### 8.4 Intersecção de Acontecimentos — Regra da Multiplicação

Probabilidade de ocorrer A **e** B simultaneamente:

```
P(A ∩ B) = P(A) × P(B|A)
```

---

### 8.5 Probabilidade Condicional

Probabilidade de B ocorrer **dado que** A já ocorreu:

```
P(B|A) = P(A ∩ B) / P(A)
```

**Exemplo do teste:**
```
P(C|H) = P(H ∩ C) / P(H) = 0,08 / 0,15 ≈ 0,533
```
"Dado que o veículo emite hidrocarbonetos em excesso, a probabilidade de também emitir monóxido de carbono em excesso é de aproximadamente 53,3%."

---

### 8.6 Acontecimentos Independentes vs Dependentes

**A e B são independentes** se a ocorrência de um **não afeta** a probabilidade do outro.

**Condição de independência:**

```
A e B independentes  ⟺  P(A ∩ B) = P(A) × P(B)
```

Equivalentemente:
```
A e B independentes  ⟺  P(B|A) = P(B)
```

---

**Exemplo — Pergunta 7 do teste (resolução completa):**

**Identificação dos acontecimentos:**
- H: "veículo emite hidrocarbonetos em excesso" → P(H) = 0,15
- C: "veículo emite monóxido de carbono em excesso" → P(C) = 0,12
- P(H ∩ C) = 0,08

**Verificação da condição de independência:**
```
P(H) × P(C) = 0,15 × 0,12 = 0,018
P(H ∩ C)    = 0,08
```

Como 0,018 ≠ 0,08 → **os acontecimentos são DEPENDENTES**.

**Verificação alternativa (via probabilidade condicional):**
```
P(C|H) = P(H ∩ C) / P(H) = 0,08 / 0,15 ≈ 0,533
P(C)   = 0,12
```

Como P(C|H) ≈ 0,533 ≠ P(C) = 0,12 → **dependentes**.

**Conclusão:**
"A emissão excessiva de hidrocarbonetos e a emissão excessiva de monóxido de carbono são acontecimentos **dependentes**, pois P(H ∩ C) = 0,08 ≠ P(H) × P(C) = 0,018. Saber que um veículo emite hidrocarbonetos em excesso aumenta significativamente a probabilidade de emitir monóxido de carbono em excesso (de 12% para aproximadamente 53,3%)."

---

### 8.7 Tabela-Resumo das Fórmulas de Probabilidade

| Situação | Fórmula |
|----------|---------|
| Complementar | P(Aᶜ) = 1 - P(A) |
| União | P(A ∪ B) = P(A) + P(B) - P(A ∩ B) |
| Condicional | P(B\|A) = P(A ∩ B) / P(A) |
| Multiplicação | P(A ∩ B) = P(A) × P(B\|A) |
| Independência | P(A ∩ B) = P(A) × P(B) |

---

## 9. RESOLUÇÃO GUIADA DAS QUESTÕES DO TESTE

---

### Pergunta 1 — Natureza, Representação e Medidas de Localização

| Variável | Natureza dos Dados | Representação Gráfica | Medidas de Localização Central |
|----------|:------------------:|:---------------------:|:------------------------------:|
| Antiguidade do cliente | **Ordinal** | **Gráfico de barras** | Moda, Mediana |
| Sistema de entrega preferido | **Nominal** | **Gráfico de barras** (ou circular) | Apenas Moda |
| Satisfação global com o serviço | **Quantitativo Contínuo** | **Histograma** | Moda, Mediana, Média |

**Justificação:**
- "Antiguidade" é ordinal porque existe uma ordem (novo < atual < antigo) mas a diferença entre categorias não é mensurávelda mesma forma.
- "Sistema de entrega" é nominal porque 0 e 1 são apenas rótulos sem ordem.
- "Satisfação" é quantitativo contínuo (escala 0 a 10 contínua).

---

### Pergunta 2 — Tabela de Frequências, Quartis e Medida de Localização

**A.** Construir tabela de frequências a partir do gráfico de barras:
- Ler a altura de cada barra → frequência absoluta
- Calcular frᵢ = fᵢ / 200
- Calcular Fᵢ (acumulada) e Frᵢ = Fᵢ / 200

**B.** Calcular os quartis com base na tabela de frequências acumuladas.

**C.** Escolha da medida de localização central:
- Calcular CV = (1,25 / 2,49) × 100 ≈ 50,2%
- CV > 30% → dispersão elevada; a distribuição pode ser assimétrica; a **mediana** é a medida mais robusta.
- Alternativa: verificar se Média (2,49) ≠ Mediana → assimetria → mediana preferível.

**D.** % de clientes sem queixas:
```
% = (f₀ / 200) × 100
```
(ler f₀ diretamente do gráfico de barras para o valor 0)

---

### Pergunta 3 — Histograma + Box Plot

A questão pede para preencher uma frase com base nos gráficos (histograma e box plot):

| Blank | O que preencher | De onde ler |
|-------|-----------------|-------------|
| "Metade atribui valor de ___ ou menos" | Q2 (mediana) | Box plot (linha central da caixa) |
| "Valores com maior frequência (___%) entre ___ e ___" | frᵢ% da classe modal; limites da classe | Histograma (barra mais alta) |
| "Em média os clientes atribuem ___" | Média (x̄) | Tabela de dados |
| "Distribuição é ___" (simetria/assimetria) | Verificar se Média > ou < Mediana | Comparar média e mediana |
| "Um quarto dos clientes atribui valor superior/inferior a ___" | Q1 ou Q3 | Box plot (extremos da caixa) |
| "Elevada dispersão observada ___%" | CV | Calcular CV = (s/x̄) × 100 |
| "Outlier qualquer valor superior/inferior a ___" | Limite superior ou inferior | Q3 + 1,5×IQR ou Q1 - 1,5×IQR |
| "Representação da esquerda é ___" | histograma | Identificação visual |
| "Representação da direita é ___" | box plot | Identificação visual |

---

### Pergunta 4 — Diagrama de Dispersão + Pearson

**Gráfico:** Diagrama de dispersão (scatter plot).

**Cálculo do coeficiente de Pearson:**
```
r = Cov(X,Y) / (s_X × s_Y)
r = 1,02 / (1,241 × 1,083)
r = 1,02 / 1,343643
r ≈ 0,759
```

**Interpretação:**
- Sinal + → associação **positiva**
- |r| = 0,759 → intensidade **forte** (0,70 – 0,89)

---

### Pergunta 5 — Complementar

```
P(não emite HC) = 1 - 0,15 = 0,85
```
**Resposta correta: 0,85** ✅

---

### Pergunta 6 — União (Regra da Adição)

```
P(H ∪ C) = 0,15 + 0,12 - 0,08 = 0,19
```
**Resposta correta: 0,19** ✅

---

### Pergunta 7 — Independência/Dependência

```
P(H) × P(C) = 0,15 × 0,12 = 0,018  ≠  P(H ∩ C) = 0,08
→ DEPENDENTES
```

---

## 10. PONTOS-CHAVE PARA NÃO ESQUECER

| # | Regra |
|---|-------|
| 1 | **Nominal** → só moda; gráfico de barras ou circular |
| 2 | **Ordinal** → moda e mediana; gráfico de barras |
| 3 | **Quantitativo** → moda, mediana e média; histograma (contínuo) ou barras (discreto) |
| 4 | **Barras ≠ Histograma**: barras têm espaço; histograma não tem |
| 5 | Se **Média > Mediana** → assimetria positiva (cauda à direita) |
| 6 | Se **Média < Mediana** → assimetria negativa (cauda à esquerda) |
| 7 | **CV > 30%** → elevada dispersão; preferir mediana à média |
| 8 | **Outlier** = valor fora de [Q1 - 1,5×IQR ; Q3 + 1,5×IQR] |
| 9 | **r de Pearson** = Cov(X,Y) / (s_X × s_Y); varia entre -1 e +1 |
| 10 | **Independência**: P(A ∩ B) = P(A) × P(B); se falhar → **dependentes** |
| 11 | **P(A ∪ B)** = P(A) + P(B) − P(A ∩ B) — nunca esquecer subtrair a intersecção! |
| 12 | **P(Aᶜ)** = 1 − P(A) — sempre! |

---

*Guia de estudo criado com base no Primeiro Teste - Prova tipo da UC LEIF004ON1. Estatística*
