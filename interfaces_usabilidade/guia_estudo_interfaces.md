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

*Boa sorte no teste! 🍀*
