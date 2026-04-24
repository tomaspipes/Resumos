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

💡 **Resposta Exemplo:**

As cinco dimensões do design de interação, propostas por Gillian Crampton Smith, não devem ser entendidas como categorias isoladas, mas como um sistema interdependente em que cada decisão numa dimensão condiciona e é condicionada pelas restantes.

A **1D (Palavras)** define a linguagem da interface — os rótulos, instruções e mensagens de erro que orientam o utilizador. A **2D (Representações Visuais)** reforça ou contradiz esse texto através de ícones, cores e tipografia. Se as duas dimensões estiverem alinhadas, o utilizador forma rapidamente um modelo mental correto e sabe o que fazer. Se não estiverem — por exemplo, um botão com o texto "Confirmar" mas com uma cor vermelha associada a perigo — a ambiguidade gera hesitação.

A **3D (Objetos/Espaço)** organiza fisicamente os elementos na interface: a proximidade entre controlos relacionados reduz a carga cognitiva e guia o olhar. A **4D (Tempo)** comunica causalidade através de animações, transições e feedback sonoro — o utilizador aprende que "a minha ação produziu este resultado" através da sequência temporal. Sem feedback temporal adequado, o utilizador não sabe se o sistema reagiu ou se está bloqueado.

O **5D (Comportamento)** é o resultado emergente de todas as decisões anteriores: é onde a experiência se materializa, onde os modelos mentais são confirmados ou quebrados, e onde a confiança no sistema se constrói ou se perde ao longo do tempo.

**Exemplo — Google Maps:**
As instruções de navegação (1D) são imediatamente reforçadas por setas visuais e pela via destacada no mapa (2D). O espaço do ecrã está organizado de forma a que a informação crítica — distância e próxima manobra — seja sempre a mais proeminente (3D). A animação suave do recálculo de rota, acompanhada de feedback sonoro (4D), sinaliza que o sistema reagiu sem surpreender o utilizador. O resultado comportamental (5D) é uma interação confiante e automática: o utilizador não questiona o sistema, simplesmente segue.

**Problemas de desalinhamento:**
Se a mesma app recalculasse a rota em silêncio e sem animação (4D deficiente), e sem qualquer mensagem textual (1D ausente), o utilizador não saberia se o sistema estava a processar ou bloqueado. O comportamento resultante (5D) seria contraproducente: toques repetidos no ecrã, frustração e, em contexto de condução, risco de segurança. O desalinhamento entre dimensões não gera apenas má experiência — pode gerar consequências reais.

---

**Pergunta 18 — Modelos Mentais**

> Os modelos mentais influenciam fortemente a forma como os utilizadores interagem com interfaces digitais. Explique o que são modelos mentais no contexto do design de interação e analise como a discrepância entre o modelo mental do utilizador e o modelo do sistema pode gerar problemas de usabilidade. Ilustre com um exemplo e proponha estratégias de design que minimizem essa discrepância.

*Pontos-chave: definição (representação interna do funcionamento do sistema, formada por experiência prévia e expectativas); discrepância = rutura de expectativa → frustração, erros, abandono; exemplo (slider de volume horizontal vs. vertical que funciona horizontalmente, ignição de carro física vs. botão); estratégias (seguir convenções — Lei de Jacob, onboarding, feedback imediato, affordances claras).*

💡 **Resposta Exemplo:**

Um modelo mental é a representação interna que um utilizador constrói sobre o funcionamento de um sistema, com base na sua experiência prévia, no conhecimento adquirido e nas expectativas geradas pelo contexto. Não são criados pelo sistema — são construídos pelo utilizador — e determinam como este interpreta a interface e antecipa o resultado das suas ações.

Quando o modelo mental do utilizador está alinhado com o modelo real do sistema, a interação é fluida, previsível e eficiente. Quando existe discrepância, surgem problemas de usabilidade: o utilizador comete erros, fica confuso, perde tempo ou abandona a tarefa.

**Exemplo 1 — Slider de volume (abordado em aula):**
Um slider de volume horizontal, em que mover para a direita aumenta o som, respeita o modelo mental da maioria dos utilizadores — segue a convenção de que "direita = mais". O utilizador age de forma automática, sem pensar. Se o mesmo slider for apresentado verticalmente mas operar horizontalmente (mover para a direita enquanto visualmente aponta para cima), existe uma discrepância entre o modelo mental e o modelo do sistema. O utilizador hesita, testa, erra — e a confiança na interface quebra-se.

**Exemplo 2 — Ignição de automóvel:**
A chave física giratória cria um modelo mental claro e integrado na memória motora: girar = ligar. A transição para um botão de arranque digital pode criar discrepância inicial — especialmente para utilizadores que migram de carros convencionais. O modelo antigo não encaixa no novo sistema.

**Estratégias para minimizar a discrepância:**
- **Seguir convenções estabelecidas** (Lei de Jacob): os utilizadores chegam com modelos mentais formados noutros sistemas — aproveitar isso reduz a carga de aprendizagem.
- **Affordances claras**: o design visual deve sugerir a ação correta (botão com aspeto clicável, campo de texto com cursor piscante).
- **Feedback imediato**: confirmar ao utilizador que a ação produziu o efeito esperado reforça e corrige o modelo mental ao longo do tempo.
- **Onboarding progressivo**: para interfaces inovadoras onde a rutura com convenções é inevitável, guiar o utilizador nas primeiras interações acelera a construção de um novo modelo mental correto.

---

**Pergunta 19 — Contexto de Uso no Design**

> De que forma o contexto em que um produto ou serviço será utilizado influencia o processo de design de interfaces e a experiência do utilizador? Explique como fatores como ambiente, cultura, necessidades do utilizador e objetivos específicos podem moldar as decisões de design, e discuta exemplos em que essas variáveis impactam significativamente o sucesso ou fracasso de uma interface.

*Pontos-chave: contexto físico (luz intensa → contraste, mobilidade → botões grandes, ruído → alternativa visual ao som); contexto cultural (cores com significados diferentes, direção de leitura RTL vs LTR); necessidades e objetivos (utilizador novato vs. expert, uso pontual vs. diário); exemplos de sucesso/fracasso (app de mapas que não funciona offline em zonas sem rede, quiosque de aeroporto em vários idiomas).*

💡 **Resposta Exemplo:**

O contexto de utilização é um dos fatores mais determinantes no design de interfaces, porque uma solução tecnicamente correta pode falhar completamente se não estiver adaptada ao ambiente, à cultura e às necessidades reais do utilizador no momento de uso.

**Contexto físico e ambiental:**
Uma app de navegação usada em mobilidade — a pé ou de carro — tem restrições físicas que uma app de desktop não tem: luz solar intensa reduz a legibilidade, logo o contraste tem de ser elevado; o utilizador tem uma mão ocupada, logo os alvos tácteis têm de ser grandes (Lei de Fitts); o ambiente é ruidoso, logo o feedback sonoro não chega sozinho e é necessário complemento visual. Uma interface que ignore estas condições — botões pequenos, texto cinzento sobre fundo branco, alertas apenas sonoros — falha não por razões técnicas, mas por desconhecimento do contexto.

**Contexto cultural:**
As decisões de design têm significados culturalmente variáveis. A cor vermelha significa perigo em Portugal, mas prosperidade na China. A direção de leitura da direita para a esquerda (RTL) em árabe ou hebraico implica um layout espelhado. Um ícone de "casa" pode não ser reconhecido como "página inicial" em culturas onde as habitações têm formas diferentes. Ignorar estas variáveis resulta em interfaces que funcionam para um contexto cultural mas alienam outros.

**Necessidades e objetivos do utilizador:**
Um utilizador que usa uma app bancária diariamente desenvolve eficiência e conhece os atalhos — um design minimalista e direto serve-o melhor. Um utilizador que usa a mesma app uma vez por ano precisa de maior visibilidade das opções e linguagem mais explícita. A mesma interface não pode otimizar igualmente para os dois perfis sem adaptação contextual.

**Exemplo de sucesso e de fracasso:**
O quiosque de check-in do aeroporto de Lisboa, disponível em vários idiomas e com instruções visuais claras independentes da língua, é um exemplo de design sensível ao contexto cultural e à diversidade de utilizadores. Em contraste, uma app de transportes públicos que não funciona offline — quando o utilizador está precisamente no metro sem rede — falha no momento mais crítico de uso, por ignorar o contexto físico de utilização real.


