# 📚 Guia de Estudo — Interfaces e Usabilidade
> LEI EaD — Universidade Europeia | Prof.ª Paula Neves
> Compilado a partir das Aulas 02 a 06

---

## 📋 Índice

1. [Unidade 01 — Interação Pessoa-Máquina (Aula 02)](#unidade-01)
2. [Unidade 02 — Modelos de Interação: Metáforas e Modelos Mentais (Aula 03)](#unidade-02-aula03)
3. [Unidade 02 — Design de Interação, Princípios e Leis UX (Aula 04)](#unidade-02-aula04)
4. [Unidade 02 — Modelo GOMS (Aula 05)](#unidade-02-aula05)
5. [Unidade 03 — Componentes UI, Acessibilidade e Metodologia UX/UI (Aula 06)](#unidade-03)
6. [Resumo Rápido para o Teste](#resumo-rapido)

---

## 🔷 Unidade 01 — Interação Pessoa-Máquina <a name="unidade-01"></a>
*(Aula 02 — 12 Março 2026)*

### O que é HCI / IPM?

**Human-Computer Interaction (HCI)** ou **Interação Pessoa-Máquina (IPM)** é o estudo e a prática de como os seres humanos interagem com sistemas computacionais, tecnologias e dispositivos.

> Envolve: comunicação, controlo e uso de dispositivos por meio de interfaces (ecrãs, teclados, rato, voz, etc.)

Esta área envolve tanto o **design dessas interfaces** quanto a **compreensão das capacidades e limitações humanas**, garantindo que as interações sejam eficientes, eficazes e satisfatórias. O design do próprio sistema onde as interfaces estão inseridas também faz parte do HCI.

### Conceitos-chave do HCI

| Conceito | Definição |
|---|---|
| **Interface de Utilizador (UI)** | Ponto de contacto entre utilizador e máquina. Pode ser gráfica (GUI), baseada em texto, voz, touch, etc. |
| **Usabilidade** | Facilidade e eficiência com que utilizadores realizam tarefas + satisfação geral |
| **Feedback** | Resposta do sistema após uma ação (visual, sonora, tátil) — indica que a ação realmente aconteceu |
| **Ergonomia** | Adaptação do sistema às características físicas e cognitivas dos utilizadores |
| **Acessibilidade** | Design que considera a diversidade de utilizadores, incluindo pessoas com deficiências |
| **UX (User Experience)** | Experiência global do utilizador: fluida, intuitiva e agradável |

---

### Evolução Tecnológica do HCI

| Geração | Período | Características |
|---|---|---|
| 1.ª — Válvulas (Tubos de Vácuo) | 1930–1956 | Computadores gigantescos (ENIAC). Linguagem máquina. Entrada por cartões perfurados e fita de papel. Saída impressa. Limitados a um problema de cada vez. |
| 2.ª — Transístores | 1947–1963 | Invenção do transístor na Bell Labs (1947). Computadores mais pequenos, rápidos e robustos. Linguagem simbólica (assembler). Batch processing. |
| 3.ª — Circuitos Integrados | 1964–1971 | Integração de circuitos. Maior portabilidade. Primeiros ecrãs rudimentares e interfaces por linha de texto (CLI). |
| 4.ª — Microprocessadores | 1972–2010 | Intel 4004 (1971) — primeiro microprocessador comercial. PC, Apple Lisa (1983), GUI, World Wide Web (1991), Mobile (2000s). Efeitos 3D nas interfaces. |
| 5.ª — Inteligência Artificial | 2010–presente | IA, interfaces conversacionais, AR/VR. No futuro: computação quântica e nanotecnologia. |

**Marcos importantes:**

- **1968** — *"Mother of All Demos"* por **Doug Engelbart** (San Francisco): demonstrou o rato, teclado, videoconferência, múltiplas janelas e trabalho colaborativo. Apresentou a visão do **"Homem Aumentado"** — o computador como potencializador do intelecto humano, transformando mudanças quantitativas em qualitativas. Engelbart retirou o foco do design da máquina para o utilizador: o ecrã, o teclado e o rato seriam tão importantes quanto os circuitos. O rato tornou-se uma extensão da ação humana (manipulação direta), atravessando a fronteira física entre o ser humano e o computador.
- **1974/75** — **Xerox PARC**: primeiro editor WYSIWYG e interface **WIMP** (Windows, Icons, Menus, Pointer). O desktop como metáfora de secretária humanizou a relação homem-máquina — ficheiros como papel, pastas de ficheiros, caixote do lixo no ecrã.
- **1983** — **Apple Lisa**: primeiro computador com ecrã integrado + rato.
- **1984** — **Apple Macintosh**: primeira GUI acessível ao grande público — produto mais pequeno, mais barato e mais apetecível.

> 💡 **Reflexão da aula:** Após décadas com paradigmas de interface virtualmente idênticos aos do Xerox PARC, questiona-se se a IA, realidade aumentada ou interfaces embutidas em óculos criarão um novo paradigma. O **Liquid Glass** (Apple, 2025/2026) é visto como tendência visual/estética 3D, ainda sem componente de IA.

---

### Fatores Humanos & HCI

**Definição (IEA):** A ergonomia (ou fatores humanos) é a disciplina científica que se ocupa da compreensão das interações entre os seres humanos e outros elementos de um sistema, aplicando teoria, princípios e métodos para otimizar o bem-estar humano e o desempenho global do sistema.

**Origem histórica:** A disciplina tem raízes na **Revolução Industrial** e na **Segunda Guerra Mundial** — especificamente no design de cockpits de aeronaves. Num cockpit, o piloto tem de controlar o avião, lançar bombas e defender-se, tudo simultaneamente em ambiente de extremo perigo. A colocação incorreta de controlos provocava erros fatais. Engenheiros de design e psicólogos industriais colaboraram para otimizar as interfaces dos cockpits. As empresas perceberam que o sucesso de um produto dependia de um bom design de fatores humanos.

**Objetivos dos Fatores Humanos:**
- Eficácia funcional → reduzir erros, aumentar produtividade e disponibilidade do sistema
- Bem-estar humano → melhorar segurança, saúde e conforto

**HFE (Human Factors Engineering):** aplicação de princípios psicológicos e fisiológicos à engenharia e design de produtos, processos e sistemas.

> Negligenciar os fatores humanos → fraca usabilidade, maior carga cognitiva, frustração, redução de produtividade.

---

### Evolução do Modelo: Racional → Contextual

| Modelo Racional (1.ª Fase) | Modelo Contextual (2.ª Fase — a partir dos anos 80) |
|---|---|
| Visão do Homem-Máquina como sistema funcional | Inclui contexto (ambiente, cultura, normas sociais) |
| Limites antropométricos | Identificação da utilização real |
| Sensibilidade visual e motora | Ambientes de utilização |
| Tempo de resposta | Especificação da utilização |
| Capacidade cognitiva | Avaliação dos riscos |
| Limites de memória | Frequência de utilização |
| Capacidade de carga de trabalho | Aspetos humanistas e sociológicos |

> "O comportamento humano é moldado pelo contexto — não pode ser simplesmente mecanicista!"

A evolução passa de um modelo do **ser humano isolado** (sujeito apenas a limitações biológicas) para o modelo do **ser humano social e cultural** moldado pelo seu ambiente.

---

### As 4 Dimensões dos Fatores Humanos na HCI

1. **Dimensão Física (Ergonómica)**
   - Capacidades motoras e sensoriais
   - Postura, esforço físico, conforto
   - Tamanho de botões, teclado, touchscreen; campo visual; capacidade auditiva
   - *Exemplo: botões muito pequenos num smartphone dificultam a interação*
   - *Exemplo real da aula: câmaras em substituição de espelhos retrovisores em camiões/autocarros para eliminar pontos mortos*

2. **Dimensão Cognitiva**
   - Atenção, memória, perceção
   - Tomada de decisão, carga cognitiva, aprendizagem
   - Modelos mentais, processamento de informação, resolução de problemas
   - *Exemplo: interfaces com muitos menus aumentam o esforço mental*

3. **Dimensão Emocional**
   - Satisfação, frustração, confiança, motivação
   - *Exemplo: sistema de navegação que demora a responder → frustração; comando de voz que funciona → satisfação*

4. **Dimensão Social e Contextual**
   - Ambiente (trabalho, casa, carro, etc.)
   - Colaboração entre utilizadores; normas sociais; pressão social
   - Cultura e hábitos
   - *Exemplo: no carro, passageiros sugerem música; status social associado a certos sistemas de navegação*

---

### ISO 9241 — Norma Internacional de Ergonomia

**ISO 9241** é uma norma internacional de ergonomia para interação humano-sistema, publicada pela ISO (International Standard Organization).

**ISO 9241-210:2010** — fornece requisitos e recomendações para princípios de design centrado no humano ao longo do ciclo de vida de sistemas interativos.

#### Os 7 Princípios de Interação (ISO 9241-110):
1. Adequação às tarefas do utilizador
2. Auto-descritivo — o sistema explica o que faz
3. Conformidade com as expectativas do utilizador
4. Capacidade de aprendizagem
5. Controlabilidade — o utilizador controla o fluxo
6. Robustez em erros no uso — tolera e recupera erros
7. **Engajamento / Envolvimento do utilizador** *(adição recente — reflete a preocupação com o aspeto emocional/satisfação)*

> 💡 O número 7 (Engajamento) foi uma atualização recente e significativa — reflete a preocupação com a satisfação e o aspeto emocional, que nas normas anteriores não estava contemplado explicitamente.

---

### Métodos de Avaliação dos Fatores Humanos

| Método | Descrição |
|---|---|
| **Avaliação Heurística** | Especialistas analisam a interface usando heurísticas (ex: Nielsen: consistência, feedback, prevenção de erros). Feita **antes** de apresentar ao utilizador. |
| **Avaliação de Usabilidade** | Utilizadores reais realizam tarefas → avalia dificuldades, erros, tempo, satisfação. Feita com **protótipo**. Ferramentas: observação, gravação de ecrã, questionários |
| **Questionários de Usabilidade** | SUS (System Usability Scale), UEQ (User Experience Questionnaire) |
| **Análise de Tarefas** | Estudo detalhado das ações para completar uma tarefa → identifica passos desnecessários, simplifica fluxos |

> Distinção importante: a **avaliação heurística** é atestada por especialistas (antes do produto chegar ao utilizador); a **avaliação de usabilidade** testa com pessoas reais usando um protótipo.

#### 🔖 Atividade de aula — Aplicar as 4 Dimensões a interfaces reais:
Exemplo dado: sistema de **navegação automóvel**
- **Físico:** visibilidade do ecrã, tempo de reação, coordenação motora, capacidade auditiva
- **Emocional:** frustração quando o sistema demora; confiança quando as instruções são claras; stresse se muitas ações simultâneas; satisfação quando o comando de voz funciona
- **Social:** passageiros interagem com o sistema (música, destino); norma social de não usar telemóvel ao conduzir → maior dependência do sistema do carro; status associado a certos sistemas
- *Outros exemplos sugeridos na aula: ATM, quiosques check-in de aeroporto, sistema de senha num hospital, painel de ar-condicionado*

---

## 🔷 Unidade 02 — Metáforas Conceptuais e Modelos Mentais <a name="unidade-02-aula03"></a>
*(Aula 03 — 20 Março 2026)*

### Os 3 Paradigmas do HCI

| Paradigma | Metáfora | Foco |
|---|---|---|
| **Engenharia** | "Match of human and machine" | Funcionalidade, confiabilidade, desempenho, prevenção de erros |
| **Informação Humana** | "Human minds are like information processors" | Processos da mente humana; como a informação é percebida, acedida e transformada |
| **Design Thinking** | "Experiencing meaning within an artifact and its use" | Qualidade experiencial; o utilizador experimenta significado no contexto do artefato |

---

### Tipologias de Interfaces

- **GUI** — Interface Gráfica do Utilizador
- **CLI** — Interface de Linha de Comando
- **Interface baseada em formulário**
- **Interface orientada pelo menu**
- **Interface de linguagem natural**

---

### Modelos Mentais no HCI

**Origem:** Kenneth Craik, *"The Nature of Explanation"* (1943) — as pessoas têm na sua mente um modelo em pequena escala de como o mundo funciona.

**Definição:** Um modelo comprimido baseado no que pensamos saber sobre um sistema e o seu funcionamento.

> Os modelos mentais não são necessariamente corretos ou objetivos — são crenças pessoais sobre o funcionamento de um sistema.

**Como se formam:**
- Baseados na experiência prévia, conhecimento adquirido e expectativas
- Quando um utilizador encontra um sistema semelhante a outro já conhecido, aplica o mesmo modelo mental
- São comportamentos **automáticos** integrados na memória — não são "vícios", são modelos mentais funcionais

**Importância para o Design:**
> "Boas experiências de utilização ocorrem quando o design está alinhado com o modelo mental dos utilizadores."

**Reduzir o fosso** entre os modelos mentais dos designers e dos utilizadores é um dos principais desafios no design de interação. Para isso usam-se: entrevistas, personas, jornadas do utilizador, mapas de empatia.

#### Exemplos de Convenções de UX que os utilizadores esperam:
- Hiperligações sublinhadas ou em cor diferente
- Botões em caixas coloridas
- Caixas de pesquisa no canto superior direito
- Logótipos no canto superior esquerdo
- Navegação global no topo ou lado esquerdo

#### Exemplos de Modelos Mentais em Prática:

| Exemplo | Modelo Mental | Problema potencial |
|---|---|---|
| Carrinho de compras online | Cesto de supermercado físico | Utilizadores sem experiência com lojas físicas podem não reconhecer a metáfora |
| Botão Retroceder | Voltar ao ecrã anterior | Quando há overlay, o utilizador espera fechar o overlay, não voltar 2 páginas atrás |
| Botão Delete | Eliminar permanentemente | Quando Delete faz outra ação ou não clarifica se é permanente → confusão |
| Barra de pesquisa | Uma única barra para encontrar informação | Múltiplas barras de pesquisa → confusão sobre qual usar |

#### 🔖 Exemplo da Aula — Ignição de Automóvel:
Três tipos de ignição como ilustração de modelos mentais:
- **Ignição física** (chave giratória) → modelo mental claro, comportamento motor automático e integrado
- **Ignição digital** (botão que lê chave digital/código) → ainda intuitivo para a maioria
- **Ignição automática** (o carro liga automaticamente) → pode contradizer o modelo mental de quem espera "fazer algo" para ligar

Marcas que colocam o botão de ignição no mesmo sítio em todos os modelos respeitam o modelo mental — um comportamento já integrado na memória motora do condutor.

#### 🔖 Exemplo da Aula — Controlos de Volume (slider):
Três designs de slider de volume foram comparados na aula:
- **Barra deslizante horizontal** (esquerda = mais baixo, direita = mais alto) → modelo mental que a maioria reconhece; intuitivo
- **Selector vertical que funciona horizontalmente** → contradiz completamente o modelo mental e as expectativas; concebido propositadamente como exemplo de mau design
- **Selector circular** (estilo Apple) → reconhecível para utilizadores de iPhone; associado a subir/descer

> Um selector pode parecer vertical mas funcionar horizontalmente — isso **contradiz o modelo mental** e causa confusão imediata.

**Conclusão:** Ignorar modelos mentais → confusão, erros, frustração. Explorá-los adequadamente → interação mais natural e previsível.

---

## 🔷 Unidade 02 — Design de Interação, Princípios e Leis UX <a name="unidade-02-aula04"></a>
*(Aula 04 — 26 Março 2026)*

### Definições de Design de Interação

> "Interaction Design is the creation of a dialogue between a person and a product, system, or service. This dialogue is both physical and emotional in nature." — John Kolko (2011)

> "IxD is the design of interactive products and services in which a designer's focus goes beyond the item in development to include the way users will interact with it." — Interaction Design Foundation

### Princípios Fundamentais de UX no Design de Interação
- **Usabilidade** — facilidade com que um utilizador pode aprender e usar o produto
- **Navegação intuitiva** — sem confusão ou esforço desnecessário
- **Satisfação do utilizador** — experiência agradável que satisfaz necessidades e objetivos

---

### As 5 Dimensões do Design de Interação
*(Gillian Crampton Smith)*

| Dimensão | Descrição |
|---|---|
| **1D — Palavras** | Texto, linguagem, conteúdo verbal |
| **2D — Representações visuais** | Imagens, ícones, gráficos, tipografia |
| **3D — Objetos físicos ou espaço** | Hardware, espaço físico de interação |
| **4D — Tempo** | Duração da interação, animações, som, vídeo |
| **5D — Comportamento** | Como o utilizador responde, reações, consequências |

---

### Os 7 Princípios Fundamentais do Design de Interação
*(Dan Norman — "The Design of Everyday Things")*

| Princípio | Definição |
|---|---|
| **Visibilidade** | Quanto mais visíveis forem as funções, mais facilmente o utilizador sabe o que fazer a seguir |
| **Feedback** | O sistema deve informar o utilizador sobre o seu estado atual |
| **Restrições** | Pistas que limitam o leque de ações possíveis para direcionar o utilizador para a ação correta |
| **Mapeamento** | Relação aparente entre os controlos e o efeito que produzem |
| **Consistência** | Elementos e interações de design devem comportar-se de forma previsível em toda a interface |
| **Affordance** | Propriedades de um objeto que determinam como pode ser utilizado (ex: botão parece clicável) |
| **Carga Cognitiva** | O design deve manter a carga cognitiva do utilizador ao mínimo — eliminar tarefas desnecessárias |

---

### Leis da UX (Psicologia no Design de Interação)

#### 🔵 Lei de Fitts
> O tamanho e a distância do alvo afetam o tempo de interação.
- Alvos tácteis devem ser suficientemente grandes para seleção precisa
- *Aplicação: botões grandes → mais fácil de carregar; botões pequenos → maior tempo e erro*

#### 🔵 Lei de Hick
> Quanto mais opções o utilizador tiver, mais tempo demora a tomar uma decisão.
- Minimizar escolhas quando tempos de resposta são críticos
- Dividir tarefas complexas em etapas mais pequenas (reduz carga cognitiva)
- *Estratégias: menu curto, realçar opções recomendadas, dividir em passos*

#### 🔵 Lei de Miller
> Os utilizadores podem guardar **7 ± 2 itens** na memória de curto prazo.
- Organizar conteúdo em "chunks" (partes menores)
- A capacidade varia consoante o indivíduo e o contexto situacional
- *Aplicação: menus com poucas opções, agrupamento de informação*

#### 🔵 Lei de Jacob
> Os utilizadores tendem a desenvolver expectativas com base na experiência noutros sites que já conhecem.
- Tirar partido dos modelos mentais existentes reduz a carga cognitiva
- Seguir convenções de design já estabelecidas
- *Se inovar muito: incluir tutoriais/onboarding*

---

### Design de Interação & Psicologia Cognitiva

Dimensões cognitivas relevantes para UX:
- **Atenção e Perceção**
- **Carga Cognitiva**
- **Memória**
- **Resolução de Problemas e Tomada de Decisão**
- **Linguagem e Compreensão**

---

## 🔷 Unidade 02 — Modelo GOMS <a name="unidade-02-aula05"></a>
*(Aula 05 — 9 Abril 2026)*

### O que é o Modelo GOMS?

**GOMS** (Goals, Operators, Methods, Selection Rules) é uma estrutura cognitiva que descreve como os utilizadores interagem com sistemas, dividindo as tarefas em 4 componentes.

Permite **esquematizar** as várias fases em que o utilizador está perante algo que precisa de fazer, compartimentando e categorizando as ações, tornando-as mensuráveis.

### Os 4 Componentes do GOMS

| Componente | O que é | Exemplo (enviar e-mail) |
|---|---|---|
| **Goals** (Objetivos) | O que o utilizador quer alcançar | Enviar um e-mail |
| **Operators** (Operadores) | As ações básicas que o utilizador pode realizar | Abrir programa, escrever, anexar |
| **Methods** (Métodos) | Sequências de operadores para alcançar o objetivo | Abrir e-mail → escrever assunto → escrever corpo → anexar → clicar "Enviar" |
| **Selection Rules** (Regras de Seleção) | Como o utilizador escolhe qual método usar | Se quer enviar e-mail → usa o método de enviar e-mail |

### Para que serve?
- Analisar a complexidade das tarefas
- **Prever o tempo de execução**
- Melhorar a experiência do utilizador
- Identificar pontos de melhoria e otimizar a interface
- Apoiar decisões de design

> O GOMS estima o tempo de cada passo/operador e permite calcular o tempo total da tarefa → indicador de eficiência e usabilidade.

### 🔖 Exercício GOMS da Aula (Exemplo — Enviar Mensagem):

**Passos do exercício:**
1. Definir o **cenário** e o **perfil do utilizador** (ponto de partida — nunca a tecnologia, sempre o utilizador)
2. Listar as **ações** que o utilizador precisa de realizar para concluir a tarefa
3. Atribuir **tempos** a cada operação para medir eficiência
4. Calcular o **somatório** dos tempos

*Resultado do exercício da turma: ~580 segundos (~9,66 min) para uma tarefa complexa de envio de mensagem com formulário.*

### Dimensões e Componentes de Interação (complemento ao GOMS)

Ao aplicar GOMS, também se analisam as **dimensões de interação**:

| Dimensão | Exemplos |
|---|---|
| **Tempo** | Sequência rápida e contínua das ações |
| **Espaço** | Layout vertical (mobile) ou horizontal; espaço de acesso à interface |
| **Ação** | Toque háptico, escrita, preenchimento de formulário, comando de voz |
| **Feedback** | Visual (mensagem no ecrã), sonoro, confirmação com check |
| **Contexto** | Uso em mobilidade (mobile), ambiente de trabalho, condições físicas |

**Componentes de interação:**
- **Input mode:** teclado virtual, toque, voz
- **Output mode:** mensagem no ecrã, som, notificação
- **Controlos:** botões para enviar, abrir chats, navegar
- **Sistema:** APP (mobile), web app, desktop

---

## 🔷 Unidade 03 — Componentes UI, Acessibilidade e Metodologia UX/UI <a name="unidade-03"></a>
*(Aula 06 — 16 Abril 2026)*

### Componentes da Interface do Utilizador (UI Components)

**UI Components** são os elementos com os quais os utilizadores interagem. É através deles que todas as manifestações dos princípios de design de interação (mapeamento, feedback, affordance, etc.) se concretizam.

| Categoria | Exemplos |
|---|---|
| **Input Controls** (Controlos de Entrada) | Checkboxes, radio buttons, dropdown lists, list boxes, buttons, toggles, text fields, date fields |
| **Navigational Components** (Navegação) | Breadcrumb, slider, search field, pagination, tags, icons |
| **Informational Components** (Informativos) | Tooltips, icons, progress bar, notifications, message boxes, modal windows |
| **Containers** | Accordion |

#### Design Systems de Referência:
- **Material Design** (Google) — sistema open-source, disponível para Figma
- **Apple Human Interface Guidelines** — boas práticas para apps Apple
- **Microsoft Teams UI Kit** — disponível para Figma

---

### Acessibilidade Digital

**UX e Acessibilidade:** Don Norman definiu UX como a totalidade da experiência de uma pessoa ao interagir com um produto. Isso inclui **todas as pessoas**.

**Definição:** Projetar produtos e serviços digitais de forma que possam ser utilizados por todas as pessoas, independentemente das suas capacidades físicas, sensoriais, cognitivas ou do contexto de uso.

**Por que são importantes as diretrizes de acessibilidade?**
1. Promovem inclusão e equidade
2. Garantem cumprimento de requisitos legais
3. Melhoram a usabilidade para TODOS (não só pessoas com deficiência)
4. Ampliam o alcance do público
5. Criam designs melhores e preparados para o futuro

---

### WCAG — Web Content Accessibility Guidelines

**Criadas por:** W3C (World Wide Web Consortium) através da WAI (Web Accessibility Initiative)
- WCAG 1.0 — 1999
- WCAG 2.0, 2.1, 2.2 — versões mais abrangentes

---

### Os 4 Princípios das WCAG — **POUR**

| Princípio | Definição | Exemplo |
|---|---|---|
| **P — Perceptível** | A informação deve ser apresentada de forma que todos os utilizadores a possam perceber | Alt text em imagens, contraste adequado, legendas em vídeos |
| **O — Operável** | Os componentes devem ser utilizáveis por diferentes formas de interação | Navegação por teclado, botões com área clicável suficiente, foco visível |
| **U — Compreensível** | A informação e o funcionamento devem ser claros e previsíveis | Linguagem simples, mensagens de erro claras, consistência nos menus |
| **R — Robusto** | O conteúdo deve funcionar com diferentes navegadores e tecnologias de apoio | HTML semântico, compatibilidade com leitores de ecrã, formulários com labels |

---

### Níveis de Conformidade WCAG

| Nível | Nome | Descrição |
|---|---|---|
| **Level A** | Acessibilidade básica | Requisitos mínimos. Ex: alt text em imagens |
| **Level AA** | Remove as principais barreiras | Padrão de referência na indústria. Ex: descrições áudio para vídeos |
| **Level AAA** | Maior nível de acessibilidade | Ideal, mas nem sempre prático. Ex: transcrições + língua gestual |

> **Level AA** é o padrão adotado pela indústria como referência.

#### Exemplo — Apple iOS (acessibilidade avançada):
- **VoiceOver** → transforma interface visual em experiência auditiva; compatível com Braille (levanta questões interessantes sobre implementação em superfície lisa)
- **Texto Dinâmico** → utilizador pode aumentar tamanho da tipografia
- **Ajustes de Cor e Contraste** → filtros para daltonismo
- **Controlo por Voz** → navegar sem toque
- **Emergency SOS via Satélite** (iPhone 14+) → acessibilidade em zonas remotas sem rede; já salvou vidas

> 💡 **Discussão da aula:** A professora defende que o Emergency SOS via Satélite deveria ser **obrigatório em todos os sistemas operativos** — é um serviço de um aparelho que usamos constantemente e que deve proteger-nos em momentos de crise. Atualmente depende de investimento em satélites (modelo Apple/SpaceX). Em Portugal, o rádio-amadorismo desempenhou um papel crítico durante catástrofes (incêndios em Leiria/Coimbra, apagão) — funciona sem infraestrutura de rede.

---

### Metodologia UX/UI — Design Thinking

#### As 5 Camadas de JJ Garrett
*(The Elements of User Experience, Jesse James Garrett, 2003)*

| Camada | Foco | Atividades |
|---|---|---|
| **Strategy** (Estratégia) | Para quem e o quê? | Definição do produto, pesquisa de utilizadores, objetivos |
| **Scope** (Âmbito) | O que inclui? | Pesquisa de concorrentes, pesquisa de utilizadores-alvo, definição de funcionalidades |
| **Structure** (Estrutura) | Como se organiza? | Arquitetura de informação, fluxogramas, wireframes |
| **Skeleton** (Esqueleto) | Como se apresenta? | UI Components, protótipos funcionais, especificações do produto |
| **Surface** (Superfície) | O que o utilizador vê? | App final, marketing, suporte ao cliente |

> Cada camada evolui a partir da anterior — **do abstrato para o concreto**.

---

### Análise Estratégica

#### Web Analytics
Plataformas de análise quantitativa (Data-driven UX Research):
- Google Analytics, Google Search Console, Google Trends, SimilarWeb

**O que permitem analisar:**
- Número de utilizadores e sessões
- Taxa de rejeição (bounce rate)
- Tempo médio na página
- Fluxos de navegação (user flow)
- Conversões e funis (funnels)
- Dispositivos, localização, dados demográficos

#### Benchmarking
Método comparativo para analisar produtos/interfaces concorrentes.

**O que permite analisar:**
- Usabilidade — clareza da navegação, eficiência dos fluxos
- Arquitetura de Informação — organização de conteúdos, hierarquias
- Funcionalidades — quais existem e quais acrescentam mais valor
- Fluxos de Utilizador — passos para completar tarefas-chave
- Design Visual e UI — grelha, tipografia, cor, consistência
- Padrões e Convenções — soluções que os utilizadores já reconhecem
- Acessibilidade — conformidade com WCAG
- Posicionamento e Experiência Global

---

### Stakeholders & User Groups

| Tipo | Definição | Foco |
|---|---|---|
| **Stakeholders** | Indivíduo, grupo ou organização com interesse no projeto | Interesses financeiros, operacionais, sociais |
| **Users (Utilizadores)** | Pessoas que interagem diretamente com o produto | Necessidades e experiências; usabilidade e satisfação |

**Stakeholders Internos:** Executivos, Product Team, Engineering Team, Marketing/Sales, Customer Service

**Stakeholders Externos:** Clientes/Utilizadores, Clientes (em agências), Fornecedores, Investidores, Autoridades Reguladoras, Comunidade

> Todos os utilizadores são stakeholders, mas nem todos os stakeholders são utilizadores.

**Por que são importantes para UX?**
1. Fornecem informações valiosas e especializadas
2. Facilitam a tomada de decisões (prioridades, orçamento)
3. Garantem o sucesso do projeto

---

### User Modelling — Empatizar com os Utilizadores

#### Empatia
> Capacidade neurocognitiva e emocional de reconhecer, compreender e partilhar os estados mentais, emoções e perspetivas de outra pessoa.
*(Goleman, 1995 — "inteligência social")*

A empatia é fundamental na pesquisa do utilizador — permite compreender o outro e moldar o comportamento do designer face às necessidades reais do utilizador.

> 💡 **Reflexão da aula:** A empatia está presente em contextos profissionais variados — suporte técnico, mecânica, atendimento ao cliente. A chave está em **mudar o nosso comportamento** face à perceção das emoções e necessidades do outro.

---

#### Mapa de Empatia
Ferramenta de UX Research que ajuda a compreender melhor o utilizador, organizando visualmente o que ele:
- **Pensa e sente**
- **Vê**
- **Ouve**
- **Diz e faz**
- **Dores** (pains)
- **Necessidades** (gains)

*Usado para sintetizar insights de investigação e apoiar a criação de personas.*

---

#### Persona
> "Each persona is a description of a specific individual who is given a name, a life, a personality, and a profile as a person, especially with respect to how they use the new product or system." — UX Book

**Elementos-chave de uma Persona:**
- Nome, idade, género e imagem (com contexto de fundo)
- Slogan (o que faz ou considera relevante na sua vida)
- Experiência e competências relevantes na área do produto
- Contexto de como interage com o produto
- Objetivos, atitudes e preocupações ao usar o produto
- Citações ou breve cenário que indicam a sua atitude

> A persona é sempre o **ponto de partida** — a tecnologia nunca vem primeiro. Primeiro define-se quem vai utilizar o sistema e como isso impacta a perceção e uso da solução.

---

#### User Journey (Jornada do Utilizador)
**Definição:** Representação do percurso que um utilizador faz para alcançar um objetivo específico ao interagir com um produto/serviço/sistema digital.

**Descreve sequencialmente:**
- Etapas e ações
- Pontos de contacto (touchpoints)
- Emoções e pensamentos
- Possíveis dificuldades

**Propósito — identificar:**
- Pontos de contacto (touchpoints)
- Ações realizadas em cada etapa
- Emoções e perceções
- Dificuldades e pontos de fricção
- **Oportunidades de melhoria**

**Zonas do Mapa de Jornada (Deconstruction - NNGroup):**
- **Zona A** — Lente: persona ("quem") + cenário ("o quê")
- **Zona B** — Coração: fases da jornada, ações, pensamentos, emoções
- **Zona C** — Resultado: insights, pontos problemáticos, oportunidades, ownership

---

#### User Scenario (Cenário do Utilizador)
**Definição:** História que descreve, de forma narrativa, como o utilizador vai interagir com o produto numa situação específica da vida quotidiana.

**O cenário descreve:**
- Quem é o utilizador (persona)
- Em que contexto se encontra (local, dispositivo, condições)
- Qual é o seu objetivo
- Que ações realiza

**Template:** *"As a [type of user], I want to [action], so that [benefit]"*

---

#### Storyboard
**Definição:** Sequência visual que comunica o cenário de utilizador, garantindo que a narrativa visual do produto reflete as necessidades, motivações e contexto do utilizador.

**Como criar:**
1. Começa pelo cenário do utilizador (persona, objetivos, contexto, problemas)
2. Cria o storyboard baseado nesse cenário (cada quadro = um passo do cenário)
3. Faz a conexão explícita: emoções e decisões do utilizador refletem os objetivos e frustrações do cenário

**Benefícios:**
- Visualiza o utilizador em ação (não apenas dados abstratos)
- Facilita a comunicação de experiência e emoções
- Serve como base para testes de usabilidade e refinamento do design

---

#### User Task Flow (Fluxo da Tarefa do Utilizador)
**Definição:** Diagrama linear que mapeia visualmente as ações essenciais que um utilizador realiza para concluir uma tarefa específica.

**Características:**
- **Caminho linear** — sequência única e direta (sem ramificações)
- **Orientado para objetivos** — foca um objetivo específico
- **Alto nível** — concentra-se na tarefa em questão, não em todos os caminhos possíveis

**Elementos-chave:**
- Personagem (utilizador/actor)
- Caminho linear de ações

**Passos para criar:**
1. Compreender a jornada do utilizador
2. Combinar objetivos do produto com aspirações do utilizador (persona + jornada)
3. Identificar os pontos de entrada do utilizador
4. Criar os passos para completar a tarefa (conteúdo entre ponto de entrada e objetivo final)
5. Visualizar o fluxo

> O User Task Flow dá origem ao **fluxo de wireframes**.

**Relação entre ferramentas:**
> Jornada do utilizador → conta a história de toda a experiência
> Storyboard → visualiza de forma emocional
> User Task Flow → foco no percurso funcional; como os utilizadores atingem objetivos dentro da interface
> Juntos: transição da compreensão narrativa para a execução concreta do design

---

## 🎯 Resumo Rápido para o Teste <a name="resumo-rapido"></a>

### 📌 Conceitos Essenciais

**HCI/IPM** = estudo e prática da interação humano-computador; envolve UI, UX, Usabilidade, Feedback, Ergonomia, Acessibilidade.

**Fatores Humanos** = disciplina que adapta sistemas às capacidades humanas (física, cognitiva, emocional, social). Origem na WWII. Evolução: modelo racional → modelo contextual.

**ISO 9241** = norma internacional de ergonomia. 7 princípios: adequação à tarefa, auto-descritivo, conformidade com expectativas, aprendizagem, controlabilidade, robustez a erros, envolvimento.

**Modelos Mentais** = o que o utilizador pensa saber sobre o sistema. Devem alinhar com o design para boa UX. Exemplos: slider de volume, ignição de carro, carrinho de compras.

**GOMS** = Goals, Operators, Methods, Selection Rules → analisa e prevê tempo de execução de tarefas. Mede eficiência.

**Princípios Norman** = Visibilidade, Feedback, Restrições, Mapeamento, Consistência, Affordance, Carga Cognitiva.

**Leis UX** = Fitts (tamanho/distância do alvo) + Hick (nº opções ↑ → decisão mais lenta) + Miller (7±2 itens em memória) + Jacob (expectativas baseadas noutros sites).

**WCAG POUR** = Perceptível, Operável, Compreensível, Robusto. Níveis: A (básico) → AA (referência) → AAA (ideal).

**5 Camadas JJ Garrett** = Strategy → Scope → Structure → Skeleton → Surface.

**Ferramentas UX** = Mapa de Empatia → Persona → User Journey → User Scenario → Storyboard → User Task Flow.

---

### 📌 Quadro Resumo Final

| Tema | Detalhe-chave |
|---|---|
| HCI definição | Estudo e prática de como humanos interagem com sistemas computacionais |
| Evolução HCI | 5 gerações; marcos: Engelbart 1968, WIMP Xerox 1975, Mac 1984 |
| Engelbart 1968 | "Homem Aumentado" — rato, múltiplas janelas, videoconferência; rato = extensão da ação humana |
| Fatores Humanos | 4 dimensões: física, cognitiva, emocional, social/contextual. Origem WWII (cockpits de aeronaves). |
| Modelos Racional vs Contextual | Racional: humano isolado com limites biológicos. Contextual: humano social moldado pelo ambiente. |
| ISO 9241 | 7 princípios de interação; centrado no humano; inclui envolvimento (atualização recente) |
| Avaliação | Heurística (especialistas, antes do produto), Usabilidade (utilizadores reais + protótipo), SUS/UEQ, Análise de Tarefas |
| Paradigmas HCI | Engenharia → Informação Humana → Design Thinking |
| Modelos Mentais | Representação simplificada do sistema na mente do utilizador; exemplos: slider de volume, ignição de carro |
| 5 Dimensões IxD | Palavras, Visuais, Objetos/Espaço, Tempo, Comportamento |
| Princípios Norman | Visibilidade, Feedback, Restrições, Mapeamento, Consistência, Affordance, Carga Cognitiva |
| Leis UX | Fitts, Hick, Miller (7±2), Jacob |
| GOMS | Goals + Operators + Methods + Selection Rules; mede eficiência; ponto de partida = utilizador, não a tecnologia |
| Dimensões de Interação | Tempo, Espaço, Ação, Feedback, Contexto; Input mode / Output mode |
| UI Components | Input Controls, Navigational, Informational, Containers |
| WCAG | POUR; Níveis A/AA/AAA; criada por W3C/WAI |
| Acessibilidade Apple | VoiceOver, Texto Dinâmico, Controlo por Voz, Emergency SOS via Satélite |
| 5 Camadas Garrett | Strategy, Scope, Structure, Skeleton, Surface |
| Análise Estratégica | Web Analytics + Benchmarking |
| Stakeholders | Internos vs Externos; todos os utilizadores são stakeholders |
| Ferramentas UX | Empatia → Mapa Empatia → Persona → User Journey → Scenario → Storyboard → Task Flow |

---

## 🧪 Preparação para a Avaliação — Tipos de Perguntas

> **Estrutura do exame:**
> - Parte I — Quiz Teórico: 16 perguntas de escolha múltipla (4 opções, 1 correta) → 8 pontos
> - Parte II — 3 Perguntas de Desenvolvimento → 12 pontos

---

### 📝 Parte I — Escolha Múltipla

**1. Qual das seguintes opções descreve corretamente uma das principais etapas da evolução tecnológica das interfaces de computador?**
- a) Transição de interfaces baseadas em texto para interfaces gráficas e interativas. ✅
- b) Substituição de teclados e mouses por comandos de voz em todos os sistemas operacionais.
- c) Desenvolvimento de interfaces exclusivamente baseadas em inteligência artificial.
- d) Adoção de sistemas exclusivamente baseados em toque e gestos desde o início da informática.

---

**2. Como a evolução dos fatores humanos influenciou o desenvolvimento dos paradigmas do "Human Computer Interaction" (HCI)?**
- a) A evolução dos fatores humanos não teve impacto significativo nos paradigmas do HCI, que sempre se focaram apenas na tecnologia.
- b) O foco nos fatores humanos resultou no desenvolvimento de interfaces mais acessíveis, intuitivas e centradas no usuário, com ênfase em ergonomia. ✅
- c) A evolução dos fatores humanos levou à simplificação das interfaces, priorizando a estética em vez da funcionalidade.
- d) A melhoria nos fatores humanos gerou a necessidade de interfaces mais complexas, com múltiplas opções para os usuários.

---

**3. Quais são os aspectos centrais do Human-Computer Interaction (HCI) que devem ser considerados no design de interfaces para garantir uma experiência de usuário eficaz e eficiente?**
- a) Otimização do desempenho do sistema, compatibilidade com hardware de baixo custo e personalização do design visual.
- b) Velocidade de resposta do sistema, compatibilidade com dispositivos móveis e integração com redes sociais.
- c) Usabilidade, acessibilidade, consistência na interação e adaptação do sistema às necessidades do usuário e contexto de uso. ✅
- d) Foco em funcionalidades complexas, segurança de dados e integração com plataformas de terceiros.

---

**4. Como é que a evolução dos fatores humanos influenciou o desenvolvimento dos paradigmas de interação humano-computador (HCI) ao longo do tempo?**
- a) A evolução dos fatores humanos resultou na simplificação das interfaces, priorizando a estética visual e a complexidade do software em vez da experiência do usuário.
- b) Os fatores humanos não tiveram influência significativa nos paradigmas do HCI, que sempre se basearam exclusivamente em avanços tecnológicos.
- c) Com o foco nos fatores humanos, os paradigmas do HCI passaram a valorizar a usabilidade, ergonomia e interação centrada no usuário, promovendo interfaces mais acessíveis e intuitivas. ✅
- d) A evolução dos fatores humanos direcionou os paradigmas do HCI para a construção de interfaces de alta complexidade, com múltiplas funcionalidades avançadas sem considerar as limitações cognitivas do usuário.

---

**5. Qual é o papel dos modelos mentais em Human-Computer Interaction (HCI) e como é que estes modelos influenciam a interação do usuário com sistemas computacionais?**
- a) Modelos mentais são criados automaticamente por sistemas inteligentes, que ajustam a interface de acordo com o comportamento do usuário, sem necessidade de consideração por parte do designer.
- b) Modelos mentais têm pouca relevância em HCI, pois os usuários geralmente compreendem a interface de forma intuitiva sem a necessidade de qualquer representação interna.
- c) Modelos mentais ajudam os usuários a formar representações internas do funcionamento de um sistema, facilitando a interação e a previsibilidade das ações, mas podem levar a falhas de usabilidade se os sistemas não corresponderem às expectativas dos usuários. ✅
- d) Modelos mentais em HCI são exclusivamente teóricos e não influenciam diretamente a forma como os usuários interagem com interfaces de sistemas.

---

**6. Quais são as principais dimensões dos fatores humanos em Human-Computer Interaction (HCI) que influenciam o design de interfaces e a interação com os usuários?**
- a) Frequência de uso de dispositivos móveis, largura de banda da rede e complexidade algorítmica.
- b) Capacidade de processamento de dados, velocidade de resposta do sistema e compatibilidade com hardware.
- c) Memória, atenção, percepção visual, habilidades motoras, fatores emocionais e sociais. ✅
- d) Capacidade do usuário de realizar múltiplas tarefas simultaneamente, ignorando aspetos cognitivos e físicos.

---

**7. Quais das seguintes dimensões do design de interação NÃO são consideradas fundamentais para uma interface eficaz e a experiência do usuário?**
- a) Acessibilidade, personalização da experiência do usuário e a capacidade de adaptação a diferentes dispositivos e contextos.
- b) Clareza na navegação, facilidade de aprendizado e a redução de erros do usuário.
- c) Feedback do sistema, consistência nas interações, usabilidade e adaptabilidade ao contexto de uso e às necessidades do usuário.
- d) Complexidade no design visual com elementos gráficos e animações para atrair a atenção do usuário. ✅

---

**8. Quais das seguintes alternativas descrevem corretamente as 5 dimensões do design de interação e como impactam a criação de interfaces de usuário?**
- a) 1D é caracterizado pela interação por comandos, 2D é a manipulação de gráficos de alta resolução, 3D descreve ambientes virtuais, 4D utiliza gestos, e 5D é a aplicação de inteligência artificial para prever comportamentos.
- b) 1D refere-se ao uso de interfaces de linha de comando, 2D envolve elementos visuais fixos, 3D diz respeito a gráficos em três dimensões, 4D envolve o controle da interação através do som, e 5D descreve interações através de emoções e sentimentos.
- c) 1D envolve o uso de palavras como meio principal de interação, 2D lida com representações visuais, 3D usa objetos físicos ou espaço tridimensional, 4D se refere ao uso de tempo como animações ou transições, e 5D considera o comportamento do usuário e como a interação pode se adaptar a ele. ✅
- d) 1D está relacionado à interação com texto, 2D foca em imagens estáticas, 3D envolve o uso de realidade aumentada, 4D refere-se ao comportamento do usuário ao longo do tempo, e 5D é a manipulação de objetos físicos no mundo real.

---

**9. Qual é a principal aplicação da Lei de Fitts no design de interação e como afeta esta Lei a eficácia das interfaces?**
- a) A Lei de Fitts propõe que o tempo necessário para uma ação é maior quando há muitos elementos em uma interface, o que obriga os usuários a realizar mais passos.
- b) A Lei de Fitts afirma que a perceção visual do usuário é afetada principalmente pelo design gráfico, e não pela distância ou tamanho dos controlos.
- c) A Lei de Fitts sugere que o número de opções disponíveis em uma interface deve ser o maior possível, garantindo que o usuário tenha uma escolha ampla para cada ação.
- d) A Lei de Fitts afirma que a facilidade de interação com um controlo depende da sua distância do usuário e do tamanho do alvo, recomendando que alvos maiores e mais próximos ao usuário facilitam a interação e reduzem o tempo necessário para a ação. ✅

---

**10. Como a Lei de Hicks, Lei de Miller, e Lei de Jacob influenciam o design de interfaces de usuário, considerando a quantidade de escolhas e a carga cognitiva?**
- a) A Lei de Hicks recomenda que mais opções devem ser apresentadas para criar mais oportunidades de interação, a Lei de Miller argumenta que o usuário pode processar quantas informações quiser, e a Lei de Jacob sugere que a interface deve ser muito complexa para estimular o aprendizado contínuo.
- b) A Lei de Hicks sugere que a quantidade de escolhas aumenta proporcionalmente o tempo de decisão; a Lei de Miller afirma que a quantidade de informações que um usuário pode processar é limitada a sete itens por vez; e a Lei de Jacob enfatiza que interfaces devem ser projetadas com base nos modelos mentais já existentes nos utilizadores, seguindo convenções conhecidas. ✅
- c) A Lei de Hicks defende que mais escolhas sempre melhoram a usabilidade, a Lei de Miller sugere que o número de itens visíveis na tela deve ser infinito, e a Lei de Jacob propõe que os usuários devem ser constantemente desafiados com novas opções para engajá-los.
- d) A Lei de Hicks afirma que a decisão do usuário se torna mais rápida com mais opções; a Lei de Miller sugere que a carga cognitiva deve ser limitada a mais de sete opções para otimizar a interação; e a Lei de Jacob defende que a interface deve ser minimalista, com pouca ou nenhuma mudança entre estados.

---

**11. No contexto da interação pessoa-máquina, o que representam a lacuna da execução e a lacuna da avaliação no design de interfaces?**
- a) A lacuna da execução e a da avaliação são barreiras exclusivamente relacionadas com a estética da interface.
- b) A lacuna da execução diz respeito à dificuldade do utilizador em saber o que fazer; a lacuna da avaliação diz respeito à dificuldade em perceber o que aconteceu após a ação. ✅
- c) A lacuna da execução refere-se à dificuldade de perceber os resultados de uma ação; a lacuna da avaliação refere-se à dificuldade de saber como executar uma ação.
- d) Ambas as lacunas referem-se apenas a problemas técnicos no código que afetam o desempenho da interface.

---

**12. No design de interfaces digitais, diferentes áreas do conhecimento contribuem para compreender melhor o comportamento e as necessidades dos utilizadores. Qual das seguintes afirmações descreve corretamente a forma como disciplinas como a psicologia cognitiva e a antropologia influenciam o design de interfaces?**
- a) A psicologia cognitiva propõe estratégias como o chunking, que consiste em dividir a informação em partes menores para facilitar o processamento e a navegação pelos utilizadores. ✅
- b) A psicologia cognitiva recomenda aumentar a quantidade de informação apresentada numa interface para estimular a memória do utilizador.
- c) A antropologia sugere que os elementos visuais devem ser universais, evitando qualquer adaptação cultural nas interfaces digitais.
- d) A antropologia defende que as cores têm sempre o mesmo significado em todas as culturas, permitindo padronizar o design globalmente.

---

**13. No contexto do modelo GOMS (Goals, Operators, Methods, and Selection Rules), o design de uma interface deve facilitar a relação entre os objetivos do utilizador e as ações necessárias para os alcançar. O que caracteriza uma interface bem concebida segundo este modelo?**
- a) Uma interface que limita as ações do utilizador para evitar erros durante a interação.
- b) Uma interface em que o utilizador consegue definir um objetivo, compreender os passos necessários e executar as ações de forma intuitiva através do sistema. ✅
- c) Uma interface que exige que o utilizador memorize todos os comandos antes de iniciar a interação.
- d) Uma interface que apresenta o maior número possível de funcionalidades no ecrã principal para reduzir o número de cliques.

---

**14. No design de interação, compreender as limitações cognitivas e emocionais dos utilizadores é essencial para criar interfaces eficazes e experiências positivas. Qual das seguintes afirmações descreve corretamente a relação entre cognição, emoção e design de interfaces?**
- a) As limitações cognitivas dizem respeito apenas à velocidade de processamento da informação, não estando relacionadas com memória ou atenção.
- b) Cognição e emoção são interdependentes: estados emocionais como frustração ou satisfação podem influenciar a tomada de decisões e a forma como os utilizadores interagem com uma interface. ✅
- c) Sistemas digitais devem evitar qualquer tipo de feedback emocional para garantir uma interação mais objetiva e racional.
- d) As emoções dos utilizadores têm pouca influência na interação com sistemas digitais, sendo a cognição o único fator relevante para o design.

---

**15. No design de produtos e serviços digitais inclusivos, é importante considerar diferentes tipos de barreiras de acessibilidade que podem afetar os utilizadores.**
- a) As barreiras de acessibilidade podem ser visuais, motoras, auditivas ou cognitivas e podem afetar qualquer utilizador, seja de forma permanente, temporária ou devido ao contexto de utilização. ✅
- b) Problemas de acessibilidade surgem apenas em interfaces complexas e não afetam aplicações simples ou do dia a dia.
- c) As barreiras de acessibilidade dizem respeito apenas a utilizadores com deficiências permanentes, não sendo necessário considerar situações temporárias ou contextuais.
- d) A acessibilidade em interfaces digitais é resolvida apenas através do aumento do tamanho do texto e do contraste visual.

---

**16. As Web Content Accessibility Guidelines (WCAG) definem três níveis de conformidade — A, AA e AAA. Qual das seguintes afirmações descreve corretamente a relação entre estes níveis?**
- a) Os níveis A, AA e AAA são modelos alternativos de design, sendo necessário escolher apenas um durante o desenvolvimento.
- b) O nível AA define apenas requisitos técnicos de programação e não inclui orientações relacionadas com a experiência dos utilizadores.
- c) O nível A corresponde ao nível máximo de acessibilidade, enquanto AA e AAA representam apenas recomendações adicionais sem impacto relevante na experiência.
- d) O nível A estabelece requisitos básicos de acessibilidade, AA acrescenta critérios que melhoram significativamente a utilização e AAA representa recomendações adicionais avançadas. ✅

---

### 📝 Parte II — Perguntas de Desenvolvimento (4 pontos cada)

**Pergunta 17 — 5 Dimensões do Design de Interação**

> No design de interação, as cinco dimensões propostas para a conceção de interfaces devem ser compreendidas como elementos interligados que, em conjunto, moldam a experiência do utilizador. Analise de que forma decisões tomadas em uma ou mais dimensões podem influenciar o comportamento do utilizador e a forma como a experiência se desenvolve ao longo do tempo. Explique a relação de interdependência entre estas dimensões e apresente um exemplo de uma interface digital em que essa relação seja evidente, discutindo tanto os impactos positivos como eventuais problemas que possam surgir quando essas dimensões não estão devidamente alinhadas.

*Pontos-chave: definir as 5 dimensões (1D Palavras, 2D Visuais, 3D Espaço/Objetos, 4D Tempo, 5D Comportamento); explicar interdependência (ex: 1D+2D alinham expectativa, 4D comunica causalidade, 5D é o resultado emergente); exemplo concreto (ex: Google Maps, app bancária); impactos positivos (fluxo natural, confiança no sistema); problemas de desalinhamento (frustração, erros, abandono).*

---

**Pergunta 18 — Modelos Mentais**

> Os modelos mentais influenciam fortemente a forma como os utilizadores interagem com interfaces digitais. Explique o que são modelos mentais no contexto do design de interação e analise como a discrepância entre o modelo mental do utilizador e o modelo do sistema pode gerar problemas de usabilidade. Ilustre com um exemplo e proponha estratégias de design que minimizem essa discrepância.

*Pontos-chave: definição (representação interna do funcionamento do sistema, formada por experiência prévia e expectativas); discrepância = rutura de expectativa → frustração, erros, abandono; exemplo (slider de volume horizontal vs. vertical que funciona horizontalmente, ignição de carro física vs. botão); estratégias (seguir convenções — Lei de Jacob, onboarding, feedback imediato, affordances claras).*

---

**Pergunta 19 — Contexto de Uso no Design**

> De que forma o contexto em que um produto ou serviço será utilizado influencia o processo de design de interfaces e a experiência do utilizador? Explique como fatores como ambiente, cultura, necessidades do utilizador e objetivos específicos podem moldar as decisões de design, e discuta exemplos em que essas variáveis impactam significativamente o sucesso ou fracasso de uma interface.

*Pontos-chave: contexto físico (luz intensa → contraste, mobilidade → botões grandes, ruído → alternativa visual ao som); contexto cultural (cores com significados diferentes, direção de leitura RTL vs LTR); necessidades e objetivos (utilizador novato vs. expert, uso pontual vs. diário); exemplos de sucesso/fracasso (app de mapas que não funciona offline em zonas sem rede, quiosque de aeroporto em vários idiomas).*


## ✅ Respostas Completas — Parte I (Escolha Múltipla)

---

**1. Qual das seguintes opções descreve corretamente o conceito de "Affordance" segundo Don Norman?**

**Resposta: b) A propriedade de um objeto que indica como pode ser utilizado.**

Affordance refere-se às propriedades percecionadas de um objeto que sugerem ao utilizador como ele pode ser usado. Por exemplo, um botão saliente "convida" a ser pressionado, uma pega "convida" a ser agarrada. A opção (a) descreve Feedback, a (c) descreve Mapeamento e a (d) descreve Restrições — todos princípios diferentes de Norman.

---

**2. A "Mother of All Demos" (1968) foi apresentada por:**

**Resposta: c) Doug Engelbart.**

Doug Engelbart apresentou a célebre "Mother of All Demos" em 1968, em San Francisco, onde demonstrou pela primeira vez o rato, múltiplas janelas, videoconferência e trabalho colaborativo. Engelbart propôs a visão do "Homem Aumentado" — o computador como potencializador do intelecto humano. Steve Jobs (a) foi fundador da Apple; Alan Kay (b) foi pioneiro na Xerox PARC; Tim Berners-Lee (d) criou a World Wide Web em 1991.

---

**3. Segundo a Lei de Miller, quantos itens consegue o ser humano reter na memória de curto prazo?**

**Resposta: c) 7 ± 2.**

A Lei de Miller (George Miller, 1956) estabelece que a capacidade da memória de curto prazo humana é de aproximadamente 7 ± 2 itens (ou seja, entre 5 e 9). Esta lei é fundamental em UX para justificar a organização de conteúdo em "chunks" (partes menores) — por exemplo, menus com poucas opções e agrupamento lógico de informação.

---

**4. Qual é o nível de conformidade WCAG adotado como referência pela indústria?**

**Resposta: b) Level AA.**

As WCAG definem três níveis de conformidade: Level A (acessibilidade básica — requisitos mínimos), Level AA (remove as principais barreiras — padrão de referência da indústria) e Level AAA (máximo nível de acessibilidade, ideal mas nem sempre prático). O Level AA é o standard adotado pela maioria das organizações e legislações como requisito de acessibilidade.

---

**5. No modelo GOMS, o que representam os "Operators"?**

**Resposta: c) As ações básicas que o utilizador pode realizar.**

No modelo GOMS (Goals, Operators, Methods, Selection Rules), os Operators são as ações básicas/elementares que o utilizador executa — como clicar num botão, escrever texto, mover o rato. A opção (a) descreve Goals (objetivos), a (b) descreve Selection Rules (regras de seleção) e a (d) descreve Methods (métodos/sequências de operadores).

---

**6. A sigla POUR nos princípios das WCAG corresponde a:**

**Resposta: b) Perceptível, Operável, Compreensível, Robusto.**

POUR é o acrónimo dos 4 princípios fundamentais das WCAG: **P**erceptível (a informação deve ser apresentada de forma que todos a possam perceber), **O**perável (os componentes devem ser utilizáveis por diferentes formas de interação), **U** (Understandable/Compreensível — a informação deve ser clara e previsível) e **R**obusto (o conteúdo deve funcionar com diferentes tecnologias e navegadores).

---

**7. Qual das seguintes NÃO é uma das 5 dimensões do Design de Interação (Gillian Crampton Smith)?**

**Resposta: c) Acessibilidade.**

As 5 dimensões do Design de Interação de Gillian Crampton Smith são: 1D — Palavras, 2D — Representações visuais, 3D — Objetos físicos ou espaço, 4D — Tempo, 5D — Comportamento. Acessibilidade é um conceito transversal ao design, mas não faz parte das 5 dimensões do IxD.

---

**8. A avaliação heurística distingue-se da avaliação de usabilidade porque:**

**Resposta: b) É realizada por especialistas antes do produto chegar ao utilizador.**

A avaliação heurística é conduzida por especialistas em UX/usabilidade que analisam a interface com base em heurísticas reconhecidas (ex: as 10 heurísticas de Nielsen), sem envolver utilizadores reais. A avaliação de usabilidade, por contraste, envolve utilizadores reais a realizar tarefas com um protótipo. A (a) descreve a avaliação de usabilidade, a (c) descreve questionários como SUS/UEQ e a (d) descreve o modelo GOMS.

---

**9. Segundo a Lei de Hick, o que acontece quando o número de opções apresentadas ao utilizador aumenta?**

**Resposta: c) O tempo de decisão aumenta.**

A Lei de Hick (Hick-Hyman) estabelece uma relação logarítmica entre o número de opções disponíveis e o tempo necessário para tomar uma decisão. Quanto mais opções, mais tempo o utilizador demora a decidir. Em UX, isto justifica estratégias como menus curtos, realce de opções recomendadas e divisão de tarefas complexas em etapas mais pequenas.

---

**10. Qual das seguintes camadas do modelo de JJ Garrett corresponde à definição de funcionalidades e pesquisa de concorrentes?**

**Resposta: b) Scope (Âmbito).**

No modelo das 5 camadas de Jesse James Garrett, a camada de Scope (Âmbito) define "o que inclui" o produto — envolve pesquisa de concorrentes, pesquisa de utilizadores-alvo e definição de funcionalidades. A Strategy (a) define "para quem e o quê" (objetivos e público), a Structure (c) organiza a arquitetura de informação e a Skeleton (d) trata dos componentes UI e protótipos.

---

**11. O conceito de "Homem Aumentado" de Engelbart refere-se a:**

**Resposta: b) O computador como potencializador do intelecto humano.**

Doug Engelbart apresentou na "Mother of All Demos" (1968) a visão de que o computador deveria servir como potencializador do intelecto humano — transformando mudanças quantitativas em qualitativas. Engelbart deslocou o foco do design da máquina para o utilizador: o ecrã, o teclado e o rato seriam tão importantes quanto os circuitos internos. Não se trata de implantes cibernéticos (a), substituição do trabalho humano (c) ou exoesqueletos (d).

---

**12. A interface WIMP (Windows, Icons, Menus, Pointer) foi introduzida pela:**

**Resposta: c) Xerox PARC, em 1974/75.**

A interface WIMP (Windows, Icons, Menus, Pointer) foi criada no Xerox PARC em 1974/75, juntamente com o primeiro editor WYSIWYG e a metáfora do desktop (secretária com ficheiros, pastas e caixote do lixo). A Apple Macintosh (1984) popularizou este paradigma junto do grande público, mas não o inventou. O Apple Lisa (1983) foi o primeiro computador da Apple com GUI, e o Windows 1.0 da Microsoft surgiu em 1985.

---

**13. Qual dos seguintes é um componente do tipo "Informational" na UI?**

**Resposta: c) Tooltip.**

Os componentes informativos (Informational Components) incluem tooltips, ícones, progress bars, notificações, message boxes e modal windows. Checkbox (a) e Radio button (d) são Input Controls (controlos de entrada), e Breadcrumb (b) é um componente de Navegação (Navigational Component).

---

**14. A ISO 9241-110 inclui um princípio adicionado recentemente que reflete a preocupação com o aspeto emocional. Qual é?**

**Resposta: c) Engajamento / Envolvimento do utilizador.**

O sétimo princípio da ISO 9241-110 — Engajamento/Envolvimento do utilizador — foi uma adição recente e significativa à norma. Reflete a preocupação com a satisfação e o aspeto emocional da interação, que nas versões anteriores da norma não estava contemplado explicitamente. Os outros 6 princípios são: adequação às tarefas, auto-descritivo, conformidade com expectativas, capacidade de aprendizagem, controlabilidade e robustez em erros.

---

**15. No mapa de empatia, qual dos seguintes NÃO é um dos quadrantes/secções?**

**Resposta: d) Funcionalidades do produto.**

O Mapa de Empatia organiza visualmente o que o utilizador: Pensa e sente, Vê, Ouve, Diz e faz, e identifica as suas Dores (pains) e Necessidades (gains). "Funcionalidades do produto" não é uma secção do mapa de empatia — esta ferramenta foca-se exclusivamente na perspetiva e vivência do utilizador, não nas características técnicas do produto.

---

**16. Qual é a ordem correta das 5 camadas de JJ Garrett, do abstrato para o concreto?**

**Resposta: b) Strategy → Scope → Structure → Skeleton → Surface.**

As 5 camadas de Jesse James Garrett evoluem do abstrato para o concreto: Strategy (Estratégia — para quem e porquê) → Scope (Âmbito — o que inclui) → Structure (Estrutura — como se organiza) → Skeleton (Esqueleto — como se apresenta) → Surface (Superfície — o que o utilizador vê). Cada camada depende e evolui da anterior.

---

## ✅ Respostas Completas — Parte II (Perguntas de Desenvolvimento)

---

### Pergunta 1 — Modelos Mentais e Design de Interação (≈3 pontos)

> Explique o conceito de modelo mental no contexto do HCI. Dê dois exemplos concretos (abordados nas aulas) em que um design de interface respeita ou contradiz o modelo mental do utilizador, e analise as consequências para a experiência do utilizador em cada caso.

**Resposta:**

**Definição e origem do conceito:**
O conceito de modelo mental tem origem no trabalho de Kenneth Craik, na obra *"The Nature of Explanation"* (1943), que propôs que as pessoas constroem na sua mente um modelo em pequena escala de como o mundo funciona. No contexto do HCI, um modelo mental é uma representação comprimida e simplificada que o utilizador tem sobre o funcionamento de um sistema — baseada no que ele pensa saber, e não necessariamente na realidade objetiva.

**Como se formam:**
Os modelos mentais formam-se a partir da experiência prévia, do conhecimento adquirido e das expectativas do utilizador. Quando alguém encontra um sistema semelhante a outro que já conhece, aplica automaticamente o mesmo modelo mental. Estes comportamentos são automáticos, integrados na memória, e não devem ser confundidos com "vícios" — são modelos funcionais que guiam a interação.

**Importância para o design:**
Boas experiências de utilização ocorrem quando o design está alinhado com o modelo mental dos utilizadores. Reduzir o fosso entre os modelos mentais dos designers e dos utilizadores é um dos principais desafios no design de interação, recorrendo-se a entrevistas, personas, jornadas do utilizador e mapas de empatia.

**Exemplo 1 — Design que RESPEITA o modelo mental: Slider de volume horizontal**
Na aula, foram comparados três designs de slider de volume. A barra deslizante horizontal (esquerda = mais baixo, direita = mais alto) respeita o modelo mental da maioria dos utilizadores porque segue a convenção de que o movimento para a direita aumenta o valor. O utilizador interage de forma imediata, sem hesitação, porque o comportamento do controlo corresponde exatamente à sua expectativa. A consequência é uma interação natural, fluida e previsível — o utilizador não precisa de pensar, simplesmente age.

**Exemplo 2 — Design que CONTRADIZ o modelo mental: Selector vertical que funciona horizontalmente**
Na mesma comparação, foi apresentado um selector que visualmente parecia vertical mas funcionava com movimento horizontal. Este design contradiz completamente o modelo mental: o utilizador vê um controlo vertical e espera que funcione verticalmente (cima = mais alto, baixo = mais baixo), mas na realidade exige movimento horizontal. A consequência é confusão imediata, frustração e erros — o utilizador precisa de reaprender como o controlo funciona, o que aumenta a carga cognitiva e deteriora a experiência.

**Conclusão:**
Ignorar modelos mentais conduz a confusão, erros e frustração. Respeitá-los resulta numa interação mais natural e previsível. O designer deve investigar ativamente os modelos mentais do seu público-alvo e alinhar o design com essas expectativas. Quando é necessário inovar e quebrar convenções, devem incluir-se tutoriais ou mecanismos de onboarding para reconfigurar gradualmente o modelo mental do utilizador.

---

### Pergunta 2 — Princípios de Norman aplicados a um cenário (≈3 pontos)

> Considere o seguinte cenário: um quiosque de check-in num aeroporto. Identifique e explique como pelo menos 4 dos 7 princípios de design de interação de Don Norman se aplicam (ou devem aplicar) ao design deste quiosque. Para cada princípio, dê um exemplo concreto de boa ou má aplicação.

**Resposta:**

Don Norman, na obra *"The Design of Everyday Things"*, definiu 7 princípios fundamentais do design de interação: Visibilidade, Feedback, Restrições, Mapeamento, Consistência, Affordance e Carga Cognitiva. Aplicando estes princípios a um quiosque de check-in num aeroporto:

**1. Visibilidade**
Quanto mais visíveis forem as funções, mais facilmente o utilizador sabe o que fazer. Num quiosque de check-in, as opções principais (fazer check-in, imprimir cartão de embarque, despachar bagagem) devem estar claramente visíveis no ecrã inicial, com botões grandes e bem identificados. *Boa aplicação:* ecrã inicial com apenas 3–4 opções em destaque, com ícones e texto descritivo. *Má aplicação:* funcionalidades escondidas em submenus que o utilizador não consegue encontrar sob pressão de tempo.

**2. Feedback**
O sistema deve informar o utilizador sobre o resultado das suas ações. Isto é crítico num aeroporto, onde o stresse é elevado e os utilizadores precisam de confiança de que o processo está a correr bem. *Boa aplicação:* após o scan do passaporte ou do código de reserva, o quiosque apresenta uma mensagem de confirmação visual ("Reserva encontrada — João Silva, Voo TP1234") acompanhada de um som subtil de confirmação. *Má aplicação:* o utilizador faz scan do passaporte e o ecrã fica em branco durante vários segundos sem qualquer indicação de que está a processar — gerando ansiedade e levando o utilizador a repetir a ação.

**3. Restrições**
As restrições limitam o leque de ações possíveis para direcionar o utilizador para a ação correta. Num quiosque, isto é essencial para prevenir erros. *Boa aplicação:* desativar (greyout) o botão "Imprimir Cartão de Embarque" até que o utilizador tenha completado o check-in com sucesso; impedir a seleção de assentos já ocupados. *Má aplicação:* permitir que o utilizador avance para o passo de impressão antes de confirmar os dados do voo, gerando erros e necessidade de recomeçar.

**4. Affordance**
As propriedades de um objeto devem indicar como pode ser utilizado. No contexto do quiosque, os elementos interativos devem parecer interativos. *Boa aplicação:* botões com aspeto tridimensional e cor contrastante que "convidam" ao toque; zona de scan do passaporte claramente identificada com uma moldura visual e uma seta indicando onde colocar o documento. *Má aplicação:* zona de scan sem qualquer indicação visual — o utilizador não sabe onde colocar o passaporte e tenta múltiplas posições.

**5. Carga Cognitiva (bónus)**
O design deve manter a carga cognitiva ao mínimo. Num aeroporto, os utilizadores estão frequentemente stressados, com pressa e distraídos. *Boa aplicação:* processo de check-in dividido em passos simples (scan → confirmação → seleção de assento → impressão), com um máximo de 2–3 opções por ecrã, linguagem simples e multilíngue. *Má aplicação:* ecrã com 15 opções simultâneas, terminologia técnica e sem indicação clara do passo atual no processo.

**Conclusão:**
A aplicação correta dos princípios de Norman num quiosque de check-in é crucial porque o contexto de uso envolve utilizadores sob pressão temporal, com diferentes níveis de literacia digital, e onde erros podem ter consequências significativas (perder o voo). Um bom design torna o processo intuitivo, rápido e tranquilizador.

---

### Pergunta 3 — GOMS aplicado a uma tarefa (≈3 pontos)

> Aplique o modelo GOMS à tarefa de "fazer uma reserva de mesa num restaurante através de uma app mobile". Identifique os Goals, Operators, Methods e Selection Rules. Estime tempos razoáveis para cada operador e calcule o tempo total da tarefa.

**Resposta:**

O modelo GOMS (Goals, Operators, Methods, Selection Rules) é uma estrutura cognitiva que descreve como os utilizadores interagem com sistemas, dividindo as tarefas em 4 componentes. Permite esquematizar, categorizar e medir as ações do utilizador, tornando-as mensuráveis para avaliar a eficiência de uma interface.

**Cenário:** Um utilizador adulto (30 anos, familiarizado com apps mobile) pretende reservar mesa para 2 pessoas, amanhã às 20h, num restaurante italiano do qual já se lembra do nome.

**Goals (Objetivos):**
- **Goal principal:** Reservar uma mesa num restaurante via app mobile
- **Sub-goals:** (1) Encontrar o restaurante, (2) Selecionar data/hora, (3) Selecionar número de pessoas, (4) Confirmar a reserva

**Operators (Operadores) e Tempos Estimados:**

| # | Operador | Tipo | Tempo (s) |
|---|----------|------|-----------|
| 1 | Desbloquear telemóvel | Motor | 2 |
| 2 | Localizar e tocar no ícone da app | Motor/Visual | 3 |
| 3 | Aguardar carregamento da app | Sistema | 3 |
| 4 | Tocar no campo de pesquisa | Motor | 2 |
| 5 | Escrever nome do restaurante (ex: "Trattoria Roma") | Motor/Cognitivo | 15 |
| 6 | Analisar resultados de pesquisa | Cognitivo/Visual | 5 |
| 7 | Tocar no restaurante correto | Motor | 2 |
| 8 | Aguardar carregamento da página do restaurante | Sistema | 2 |
| 9 | Tocar em "Reservar Mesa" | Motor | 2 |
| 10 | Selecionar data (amanhã) | Motor/Cognitivo | 5 |
| 11 | Selecionar hora (20h) | Motor/Cognitivo | 5 |
| 12 | Selecionar número de pessoas (2) | Motor | 3 |
| 13 | Verificar os detalhes da reserva | Cognitivo/Visual | 5 |
| 14 | Tocar em "Confirmar Reserva" | Motor | 2 |
| 15 | Aguardar confirmação do sistema | Sistema | 3 |
| 16 | Ler mensagem de confirmação | Cognitivo/Visual | 3 |

**Tempo total estimado: ~62 segundos (~1 minuto)**

**Methods (Métodos):**

*Método A — Pesquisa por nome:*
Operadores 1 → 2 → 3 → 4 → 5 → 6 → 7 → 8 → 9 → 10 → 11 → 12 → 13 → 14 → 15 → 16

*Método B — Acesso por favoritos (se o restaurante estiver nos favoritos):*
Operadores 1 → 2 → 3 → Tocar em "Favoritos" (2s) → Tocar no restaurante (2s) → 8 → 9 → 10 → 11 → 12 → 13 → 14 → 15 → 16
Tempo estimado: ~49 segundos (elimina escrita + análise de resultados)

**Selection Rules (Regras de Seleção):**
- **Se** o utilizador já tem o restaurante nos favoritos **→** usar Método B (favoritos) — mais rápido
- **Se** o utilizador não tem o restaurante nos favoritos **→** usar Método A (pesquisa por nome)
- **Se** o utilizador não se lembra do nome exato **→** variante do Método A com pesquisa por localização/tipo de cozinha (tempo adicional estimado: +15s)

**Conclusão:**
A análise GOMS demonstra que a tarefa pode ser concluída em aproximadamente 1 minuto pelo Método A e em ~49 segundos pelo Método B. A diferença de ~13 segundos entre métodos revela que a funcionalidade de "Favoritos" melhora significativamente a eficiência para utilizadores recorrentes. O ponto de partida da análise é sempre o utilizador (perfil, contexto, experiência) e nunca a tecnologia. O GOMS permite identificar operadores que consomem mais tempo (ex: escrita do nome) e orientar decisões de design (ex: sugestões automáticas de pesquisa para reduzir o tempo do operador 5).

---

### Pergunta 4 — WCAG e Acessibilidade (≈3 pontos)

> Explique os 4 princípios das WCAG (POUR) e, para cada um, dê um exemplo prático de como um website de e-commerce pode cumprir esse princípio. Refira ainda os 3 níveis de conformidade e qual é o padrão de referência na indústria.

**Resposta:**

As WCAG (Web Content Accessibility Guidelines) foram criadas pelo W3C (World Wide Web Consortium) através da WAI (Web Accessibility Initiative). Definem diretrizes para tornar o conteúdo web acessível a todas as pessoas, independentemente das suas capacidades. Don Norman definiu UX como a totalidade da experiência de uma pessoa ao interagir com um produto — e isso inclui todas as pessoas. Os 4 princípios fundamentais formam o acrónimo POUR:

**P — Perceptível (Perceivable)**
A informação e os componentes da interface devem ser apresentados de forma que todos os utilizadores os possam perceber, independentemente de limitações sensoriais.

*Exemplo em e-commerce:* Todas as imagens de produtos devem ter atributos alt text descritivos (ex: "Ténis de corrida Nike Air Max 90, cor preta, tamanho 42") para que utilizadores com deficiência visual que usam leitores de ecrã possam compreender o produto. Os preços devem ter contraste adequado entre texto e fundo (ex: texto escuro sobre fundo claro). Vídeos de demonstração de produtos devem incluir legendas para utilizadores surdos ou com dificuldades auditivas.

**O — Operável (Operable)**
Os componentes da interface e a navegação devem ser utilizáveis por diferentes formas de interação, não apenas rato.

*Exemplo em e-commerce:* O website deve ser totalmente navegável por teclado (Tab para avançar entre elementos, Enter para selecionar, Esc para fechar modais). O botão "Adicionar ao carrinho" deve ter uma área clicável suficientemente grande (respeitando também a Lei de Fitts). O foco do teclado deve ser visível (com outline ou destaque) em todos os elementos interativos. Não devem existir limites de tempo excessivamente curtos no processo de checkout que impeçam utilizadores mais lentos de completar a compra.

**U — Compreensível (Understandable)**
A informação e o funcionamento da interface devem ser claros, previsíveis e fáceis de entender.

*Exemplo em e-commerce:* As mensagens de erro no formulário de checkout devem ser claras e específicas (ex: "O número do cartão de crédito deve ter 16 dígitos" em vez de "Erro no campo"). A linguagem das descrições de produtos deve ser simples e acessível. A navegação e os menus devem ser consistentes em todas as páginas — se o menu principal está no topo na homepage, deve estar no topo em todas as outras páginas. As ações irreversíveis (ex: eliminar conta) devem ter confirmação explícita.

**R — Robusto (Robust)**
O conteúdo deve funcionar corretamente com diferentes navegadores, dispositivos e tecnologias de apoio (assistive technologies).

*Exemplo em e-commerce:* Utilizar HTML semântico correto (ex: `<nav>` para navegação, `<main>` para conteúdo principal, `<button>` para botões) para garantir compatibilidade com leitores de ecrã como JAWS ou NVDA. Todos os campos de formulário no checkout devem ter labels HTML associadas (`<label for="email">`). O website deve ser testado com diferentes navegadores (Chrome, Firefox, Safari, Edge) e com tecnologias assistivas para garantir que funciona em todos.

**Níveis de Conformidade:**

| Nível | Descrição |
|-------|-----------|
| **Level A** | Acessibilidade básica — requisitos mínimos. Exemplo: alt text em imagens. Sem este nível, muitos utilizadores ficam completamente excluídos. |
| **Level AA** | Remove as principais barreiras — é o **padrão de referência adotado pela indústria** e por grande parte da legislação internacional. Exemplo: descrições áudio para vídeos, contraste mínimo de 4.5:1 para texto normal. |
| **Level AAA** | Maior nível de acessibilidade — ideal, mas nem sempre prático para todo o conteúdo. Exemplo: transcrições completas + língua gestual para todos os vídeos. |

**Conclusão:**
O Level AA é o padrão de referência na indústria e deve ser o objetivo mínimo de qualquer website de e-commerce. Cumprir as WCAG não beneficia apenas pessoas com deficiência — melhora a usabilidade para TODOS os utilizadores (ex: legendas em vídeos ajudam quem está num ambiente barulhento; contraste adequado ajuda quem usa o telemóvel ao sol). Além disso, garante cumprimento de requisitos legais e amplia o alcance do público.

---

### Pergunta 5 — Metodologia UX completa (≈3 pontos)

> Descreva, de forma encadeada, como as ferramentas de UX Research (Mapa de Empatia, Persona, User Journey, User Scenario, Storyboard e User Task Flow) se complementam no processo de design centrado no utilizador. Ilustre com um exemplo prático de uma app de transportes públicos.

**Resposta:**

No processo de design centrado no utilizador, as ferramentas de UX Research seguem uma sequência lógica e encadeada — cada uma alimenta a seguinte, evoluindo da compreensão empática do utilizador até à especificação concreta das interações na interface. A chave é que o ponto de partida é **sempre o utilizador**, nunca a tecnologia.

**1. Mapa de Empatia — Compreender o utilizador**
O Mapa de Empatia é o ponto de partida. Organiza visualmente o que o utilizador pensa e sente, vê, ouve, diz e faz, e identifica as suas dores (pains) e necessidades (gains). É construído a partir de investigação qualitativa (entrevistas, observação).

*Exemplo — App de transportes públicos:*
- **Pensa e sente:** "Tenho medo de perder o autocarro e chegar atrasado ao trabalho"
- **Vê:** Horários em papel nas paragens, desatualizados; outros passageiros a consultar o telemóvel
- **Ouve:** Colegas a recomendar apps de transporte; anúncios de novas linhas
- **Diz e faz:** "Nunca sei se o autocarro já passou"; sai de casa 20 minutos mais cedo por precaução
- **Dores:** Incerteza sobre horários reais, perda de tempo à espera
- **Necessidades:** Informação em tempo real, previsibilidade, planeamento eficiente

**2. Persona — Dar rosto ao utilizador**
A partir dos insights do Mapa de Empatia, cria-se uma Persona — uma descrição de um indivíduo fictício mas representativo, com nome, idade, perfil, contexto e objetivos.

*Exemplo:*
**Ana Ferreira**, 28 anos, designer gráfica em Lisboa. Usa transportes públicos diariamente (autocarro + metro). Não tem carro. Valoriza pontualidade e planeamento. Usa iPhone. Frustra-se quando não sabe a que horas o próximo autocarro chega. Slogan: "Preciso de saber exatamente quando saio de casa para não perder tempo."

**3. User Journey — Mapear toda a experiência**
Com a Persona definida, constrói-se a User Journey — o percurso completo que a Ana faz ao interagir com o serviço de transportes, mapeando etapas, ações, emoções, touchpoints e dificuldades.

*Exemplo — Jornada da Ana para ir trabalhar:*
| Etapa | Ação | Emoção | Ponto de Fricção |
|-------|------|--------|------------------|
| Planeamento | Consulta a app para ver horários | Expectativa | App demora a carregar |
| Deslocação à paragem | Caminha até à paragem | Neutra | Não sabe se o autocarro está atrasado |
| Espera | Aguarda pelo autocarro | Ansiedade | Sem informação em tempo real na paragem |
| Viagem | Dentro do autocarro | Alívio | Não sabe quando deve preparar-se para sair |
| Transbordo | Troca para o metro | Stresse | Tempo apertado, medo de perder a ligação |
| Chegada | Chega ao trabalho | Satisfação/Frustração | Depende de se correu bem |

Oportunidade identificada: a app deve mostrar atualizações em tempo real e alertas de transbordo.

**4. User Scenario — Narrar uma situação concreta**
O User Scenario transforma a jornada numa narrativa específica, descrevendo quem é o utilizador, o contexto, o objetivo e as ações.

*Exemplo:*
"As a **commuter** (Ana), I want to **check real-time bus arrival** so that **I can leave home at the optimal time and not wait at the bus stop unnecessarily**."

Narrativa expandida: É segunda-feira de manhã, 7h30. A Ana está em casa a tomar o pequeno-almoço. Abre a app de transportes no telemóvel, consulta o tempo estimado de chegada do próximo autocarro à sua paragem (8 minutos). Decide que tem tempo para acabar o café. Recebe uma notificação push: "O seu autocarro 28 chega em 3 minutos". Pega na mala e sai de casa.

**5. Storyboard — Visualizar a narrativa**
O Storyboard traduz o cenário numa sequência visual (estilo banda desenhada), comunicando emoções, contexto e interações com a app.

*Exemplo (quadros):*
- **Quadro 1:** Ana na cozinha a olhar para o telemóvel (expressão neutra)
- **Quadro 2:** Ecrã da app mostrando "Autocarro 28 — 8 min" (Ana sorri)
- **Quadro 3:** Notificação push "3 min" — Ana levanta-se apressada mas confiante
- **Quadro 4:** Ana na paragem, o autocarro chega quase imediatamente (expressão satisfeita)
- **Quadro 5:** Dentro do autocarro, a app mostra "Transbordo para Metro Azul em 2 paragens" (Ana relaxada)

O storyboard permite à equipa de design visualizar o utilizador em ação e empatizar com as suas emoções em cada momento.

**6. User Task Flow — Mapear as ações na interface**
O User Task Flow traduz o cenário e o storyboard num diagrama linear de ações concretas dentro da app, mapeando o caminho funcional do utilizador.

*Exemplo — Task Flow "Consultar próximo autocarro":*
Abrir app → [Ecrã: Mapa com paragens próximas] → Tocar na paragem habitual → [Ecrã: Lista de autocarros com tempos em tempo real] → Identificar "Autocarro 28 — 8 min" → Tocar em "Ativar Alerta" → [Configurar: Avisar 3 min antes] → Confirmar → [Notificação recebida] → Sair de casa

Este Task Flow dá origem diretamente ao fluxo de wireframes — a sequência de ecrãs que o designer irá prototipar.

**Relação encadeada:**
> Mapa de Empatia → fornece insights para criar a **Persona**
> Persona → serve de base para a **User Journey**
> User Journey → identifica pontos de fricção e oportunidades → alimenta o **User Scenario**
> User Scenario → narra o uso concreto → é visualizado no **Storyboard**
> Storyboard → comunica a experiência emocional → é traduzido em ações no **User Task Flow**
> User Task Flow → dá origem aos **wireframes** e protótipos

Esta sequência garante a transição coerente da compreensão narrativa e empática do utilizador para a execução concreta do design da interface.

---

### Pergunta 6 — Leis de UX num redesign (≈3 pontos)

> Imagine que foi contratado para redesenhar o menu de navegação de um website institucional que atualmente tem 25 opções no menu principal, botões pequenos e um layout inconsistente entre páginas. Utilizando as leis de Fitts, Hick, Miller e Jacob, proponha melhorias concretas e justifique cada uma com a lei correspondente.

**Resposta:**

O website descrito apresenta três problemas principais: excesso de opções no menu (25), botões pequenos e layout inconsistente. Cada um destes problemas pode ser resolvido aplicando as leis de UX estudadas.

**1. Lei de Hick — Reduzir o número de opções no menu**

*Problema:* O menu tem 25 opções no nível principal, o que força o utilizador a analisar todas antes de decidir.

*Fundamento:* A Lei de Hick estabelece que quanto mais opções o utilizador tiver, mais tempo demora a tomar uma decisão. O tempo de decisão aumenta logaritmicamente com o número de alternativas.

*Melhoria proposta:* Reorganizar as 25 opções em **5 a 7 categorias principais** no menu de primeiro nível (ex: "Sobre Nós", "Serviços", "Notícias", "Contactos", "Área Reservada"), cada uma com submenus (dropdowns) que agrupam as opções específicas. Exemplo: em vez de listar "Missão", "Visão", "Valores", "Equipa", "História" individualmente, agrupá-las sob "Sobre Nós". Isto reduz drasticamente o tempo de decisão inicial — o utilizador analisa 5–7 categorias em vez de 25 opções.

**2. Lei de Miller — Agrupar conteúdo em chunks**

*Problema:* 25 opções excedem largamente a capacidade de processamento da memória de curto prazo.

*Fundamento:* A Lei de Miller (1956) estabelece que a memória de curto prazo retém aproximadamente **7 ± 2 itens**. Apresentar 25 opções simultâneas sobrecarrega a capacidade cognitiva do utilizador.

*Melhoria proposta:* Organizar as opções em **chunks** (agrupamentos lógicos) de no máximo 5–7 itens. Dentro de cada submenu, as opções devem estar organizadas por relevância ou frequência de uso, e nunca ultrapassar 7 itens. Se uma categoria tiver mais opções, criar sub-agrupamentos com separadores visuais (headings dentro do dropdown). Exemplo: o submenu "Serviços" poderia ter 6 opções agrupadas em 2 blocos de 3 com um separador visual.

**3. Lei de Fitts — Aumentar o tamanho e reduzir a distância dos alvos**

*Problema:* Os botões são pequenos, dificultando o clique/toque preciso.

*Fundamento:* A Lei de Fitts estabelece que o tempo de interação com um alvo depende do seu tamanho e da distância a que se encontra. Alvos maiores e mais próximos são mais rápidos e fáceis de atingir.

*Melhoria proposta:* (1) Aumentar significativamente o tamanho dos botões e áreas clicáveis do menu — cada opção deve ter padding generoso (mínimo 44×44 pixels para touch, conforme recomendação Apple/Google). (2) Agrupar as opções mais frequentes em posições de fácil acesso (cantos e margens do ecrã são mais fáceis de atingir, segundo Fitts). (3) Se houver botões de ação prioritária (ex: "Contacte-nos"), torná-los maiores e mais proeminentes do que os restantes. (4) Reduzir a distância entre itens de menu relacionados para que o utilizador não tenha de percorrer longas distâncias com o cursor.

**4. Lei de Jacob — Seguir convenções de design existentes**

*Problema:* O layout é inconsistente entre páginas, quebrando as expectativas do utilizador.

*Fundamento:* A Lei de Jacob estabelece que os utilizadores desenvolvem expectativas baseadas na experiência com outros websites que já conhecem. Seguir convenções reconhecidas reduz a carga cognitiva porque o utilizador não precisa de reaprender a navegar.

*Melhoria proposta:* (1) Colocar o **logótipo no canto superior esquerdo** (clicável para voltar à homepage — convenção universal). (2) Posicionar a **barra de navegação principal no topo** da página, horizontal, com as categorias principais. (3) Colocar a **caixa de pesquisa no canto superior direito**. (4) Garantir que o **layout, cores, tipografia e posição do menu são idênticos em todas as páginas** do website — consistência total. (5) Utilizar padrões de navegação que os utilizadores reconhecem de websites de referência (ex: mega menus para websites com muitas secções, breadcrumbs para indicar a localização atual). O utilizador deve sentir-se imediatamente familiarizado com a navegação, mesmo na primeira visita.

**Síntese das melhorias:**

| Problema | Lei Aplicada | Melhoria |
|----------|-------------|----------|
| 25 opções no menu | Lei de Hick | Reduzir para 5–7 categorias com submenus |
| 25 opções sobrecarregam memória | Lei de Miller | Agrupar em chunks de 7±2 itens |
| Botões pequenos | Lei de Fitts | Aumentar tamanho (≥44px), reduzir distância entre alvos frequentes |
| Layout inconsistente | Lei de Jacob | Seguir convenções (logo em cima-esquerda, pesquisa em cima-direita, menu no topo, consistência entre páginas) |

**Conclusão:**
A aplicação combinada destas 4 leis de UX resultaria numa navegação significativamente mais eficiente, intuitiva e satisfatória. O menu passaria de uma lista esmagadora de 25 opções com botões pequenos e layout caótico para uma estrutura organizada, previsível e acessível — alinhada com as capacidades cognitivas e os modelos mentais dos utilizadores.
