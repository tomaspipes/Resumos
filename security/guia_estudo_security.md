# Guia de Estudo — Segurança de Redes e Sistemas

> **Nota:** Este guia está organizado por tópicos do programa. Foca-se nos conceitos que mais provavelmente aparecerão no teste (baseado nas NOTAS_TESTE e nos PDFs das aulas).

---

## 1. Introdução à Segurança Informática

### 1.1 Tríade CIA (Confidencialidade, Integridade, Disponibilidade)

| Pilar | Definição | Exemplo real |
|-------|-----------|--------------|
| **Confidencialidade** | Garantia de que a informação não é divulgada a entidades não autorizadas | Cifrar e-mails com PGP para que só o destinatário leia |
| **Integridade** | Garantia de que a informação não é modificada/destruída sem autorização | Hash SHA-256 de um ficheiro para verificar que não foi alterado |
| **Disponibilidade** | Garantia de que a informação está acessível quando necessário | Servidores redundantes para resistir a ataques DDoS |

**Extensões da tríade:**
- **Privacidade** = confidencialidade dos dados pessoais
- **Anonimidade** = confidencialidade da identidade
- **Autenticação** = integridade da origem
- **Não-repudiação** = integridade da comunicação (não poder negar que enviou)
- **Autorização** = integridade de direitos/permissões

### 1.2 Modelo AVI (Ataque + Vulnerabilidade = Intrusão)

Um **ataque** explora uma **vulnerabilidade** e se tiver sucesso resulta numa **intrusão**.

- **Ameaça**: potencial de causar dano
- **Vulnerabilidade**: fraqueza no sistema
- **Risco** = Valor da perda estimada × Probabilidade de perda

### 1.3 Tipos de Ameaças

| Tipo | Descrição | Objetivo principal | Exemplo |
|------|-----------|-------------------|---------|
| **Passiva** | Expõe informação sem afetar recursos | Prevenção | Sniffing de rede |
| **Activa** | Afeta os recursos do sistema | Detecção + Recuperação | DoS, Replay |

**Lista de ameaças:**
- Intercepção (sniffing/eavesdropping)
- Reprodução (replay/fabrication)
- Modificação (tampering)
- Personificação (spoofing/masquerading)
- Negação de serviço (DoS)
- Repudiação
- Acesso não autorizado

### 1.4 Controlos de Segurança (⚠️ PROVÁVEL NO TESTE)

| Controlo | O que faz | Exemplo |
|----------|-----------|---------|
| **Dissuasão** | Desencoraja atacantes | Honeypots, políticas de segurança visíveis |
| **Prevenção** | Evita falhas de segurança | Firewall, cifra de dados |
| **Detecção** | Detecta falhas/ataques | IDS (Intrusion Detection System) |
| **Correcção** | Corrige falhas | Patches de segurança |
| **Recuperação** | Restaura após incidente | Backups, plano de disaster recovery |
| **Compensação** | Mecanismos alternativos | Seguro cibernético |

**Tipos de controlos por natureza:**
- **Técnicos/Digitais**: Firewall, IDS
- **Físicos**: Sensores de movimento, detectores de incêndio
- **Formais**: Políticas de segurança, procedimentos
- **Informais**: Formação, awareness (as pessoas são SEMPRE o elo mais fraco)

### 1.5 Princípios de Saltzer e Schroeder (⚠️ PROVÁVEL NO TESTE)

| # | Princípio | Explicação simples | Exemplo |
|---|-----------|-------------------|---------|
| 1 | **Privilégio Mínimo** | Dar apenas os privilégios necessários para a tarefa | Um estagiário só acede às pastas do seu projeto |
| 2 | **Predefinições Seguras (Fail-Safe)** | Falhar de modo seguro; negar acesso por omissão | Porta de cofre que tranca automaticamente se faltar energia |
| 3 | **Economia de Mecanismo** | Manter simples → menos bugs | Sistema com menos linhas de código = menos falhas |
| 4 | **Mediação Completa** | Verificar SEMPRE a autorização (Zero Trust) | Verificar credenciais em cada pedido, não usar cache |
| 5 | **Desenho Aberto** | Segurança não depende do segredo do algoritmo | AES é público e testado por milhares de especialistas |
| 6 | **Separação de Privilégios** | Autorização requer múltiplas condições | Transferência bancária requer password + código SMS |
| 7 | **Mínimo Mecanismo Comum** | Limitar recursos partilhados entre utilizadores | Processos isolados em containers separados |
| 8 | **Aceitação Psicológica** | Não dificultar a vida ao utilizador | Login com impressão digital em vez de passwords de 20 caracteres |

**Outros princípios importantes:**
- **Confiabilidade**: Não assumir confiança implícita
- **Segurança por camadas (Defense-in-depth)**: Vários mecanismos autónomos
- **Minimizar superfície de ataque**: Limitar acesso a recursos

### 1.6 Perfil do Atacante

**MOM**: Motivo + Oportunidade + Meios

| Perfil | Características |
|--------|----------------|
| Script Kiddies | Pouco conhecimento, curiosidade, alvos aleatórios |
| Donos de Botnets | Ganhos financeiros, maximizam máquinas comprometidas |
| Grupos Online | Procuram vulnerabilidades 0-day, constroem ferramentas |
| Hacker | Age sozinho, auto-estudo, evita detecção |
| Intruso Contratado | Espionagem industrial |
| Crime Organizado | Lucro ilícito, roubo de identidade, ransomware |
| Terroristas | Negação de serviço massiva |
| Serviços de Inteligência | Guerra de informação |

**Metodologia do atacante:**
1. Recolha de informação (análise passiva)
2. Scanning (verificação activa de serviços/vulnerabilidades)
3. Intrusão (exploits)
4. Manter acesso (rootkits)
5. Apagar rasto (alterar logs)

---

## 2. Criptografia (⚠️ MUITO PROVÁVEL NO TESTE)

### 2.1 Conceitos Base

- **Cifrar (encrypt)**: texto claro → criptograma
- **Decifrar (decrypt)**: criptograma → texto claro
- **Princípio de Kerchoff**: A segurança não deve depender do segredo do algoritmo, apenas da chave

**Tipos de operações**: Substituição, Transposição, ou Combinação de ambas

### 2.2 Cifras Stream vs. Cifras de Bloco (⚠️ PROVÁVEL NO TESTE)

| Característica | Cifra Stream (Fita) | Cifra de Bloco |
|---------------|--------------------:|---------------:|
| Unidade | 1 bit/byte de cada vez | Grupo de bits (ex: 128 bits) |
| Velocidade | Rápida | Mais lenta |
| Propagação erros | Fraca | Alta |
| Difusão | Baixa | Alta |
| Implementação | Hardware | Software |
| Vulnerabilidades | Inserção/eliminação maliciosa | — |
| Exemplo | RC4 | AES, DES |

**Difusão**: Mudar 1 bit no texto claro muda completamente o texto cifrado.
**Confusão**: Não é possível prever o efeito de mudar 1 símbolo.

### 2.3 Modos de Operação de Cifras de Bloco

| Modo | Descrição | Particularidade |
|------|-----------|-----------------|
| **ECB** | Cada bloco cifrado individualmente | Blocos iguais → criptogramas iguais (INSEGURO) |
| **CBC** | XOR com bloco cifrado anterior + vetor de inicialização | Blocos iguais → criptogramas diferentes; auto-sincronizável |
| **PCBC** | Propaga erros | Detecção de erros de transmissão |
| **CFB** | Transforma bloco em stream auto-sincronizável | — |
| **OFB** | Transforma bloco em stream sincronizada | 1 bit errado no cifrado = 1 bit errado no claro |
| **CTR** | Usa nonce + contador | Permite cifra em paralelo |

### 2.4 Criptografia Simétrica vs. Assimétrica (⚠️ PROVÁVEL NO TESTE)

| Característica | Simétrica | Assimétrica |
|---------------|-----------|-------------|
| Chaves | 1 chave partilhada (privada) | 2 chaves: pública + privada |
| Performance | Rápida, eficiente | Mais lenta |
| Tamanho chave | Menor (128-256 bits) | Maior (1024-4096 bits) |
| Escalabilidade | Difícil (distribuição de chave) | Boa (chave pública é... pública) |
| Uso principal | Cifrar grandes volumes de dados | Troca de chaves, assinaturas digitais |
| Exemplos | AES, DES, 3DES, RC4, IDEA | RSA, ECC, Diffie-Hellman |

**Na prática**: Usa-se assimétrica para trocar chaves e simétrica para cifrar os dados (sistema híbrido).

### 2.5 Algoritmos de Cifra Simétrica — DES vs AES (⚠️ PROVÁVEL NO TESTE)

| | DES | AES |
|--|-----|-----|
| Ano | 1976 | 2000 (Rijndael) |
| Chave | 56 bits (+8 paridade) | 128, 192 ou 256 bits |
| Bloco | 64 bits | 128 bits |
| Segurança | **INSEGURO** (força bruta viável) | Seguro para uso actual |
| Operação | Transposição + Substituição | — |
| Nota | Primeiro standard criptográfico | Vencedor de concurso NIST |

**Outros algoritmos:**
- **3DES**: 2 ou 3 chaves (112 ou 168 bits), blocos 64 bits — substituiu DES
- **IDEA**: 128 bits, blocos 64 bits (patenteado, expirou 2012)
- **RC4**: Stream, chave variável 1-2048 bits, simples mas usado erradamente (WEP, SSL)

### 2.6 Cifra Assimétrica — Envio de Mensagem Confidencial (⚠️ PROVÁVEL NO TESTE)

**Para garantir CONFIDENCIALIDADE:**
1. Remetente obtém a **chave pública do destinatário**
2. Remetente **cifra** a mensagem com essa chave pública
3. Envia a mensagem cifrada
4. Destinatário **decifra** com a sua **chave privada**

> Só o destinatário pode ler porque só ele tem a chave privada.

**Para garantir AUTENTICAÇÃO (assinatura):**
1. Remetente cifra com a sua **chave privada**
2. Qualquer pessoa decifra com a **chave pública** do remetente
3. Se decifrar correctamente → prova que veio daquele remetente

### 2.7 Diffie-Hellman

- Permite criar uma chave partilhada a partir do zero sem a transmitir em claro
- **Problema**: Não há autenticação → vulnerável a ataques Man-in-the-Middle (MITM)

### 2.8 Checksums Criptográficos (Hash e MAC)

**Propriedades de um hash:**
- **Unidirecional**: impossível obter a mensagem a partir do hash
- **Resistência a colisões**: 2 mensagens diferentes NÃO devem dar o mesmo hash
- **Padding**: adição de bits para tamanho correcto do bloco

| Algoritmo | Bits | Seguro? | Nota |
|-----------|------|---------|------|
| **MD5** | 128 bits (blocos 512) | ❌ NÃO | Colisões demonstradas (2^39) |
| **SHA-1** | 160 bits (blocos 512) | ❌ Depreciado | — |
| **SHA-2** | 224/256/384/512 bits | ✅ Sim | Uso recomendado actual |
| **SHA-3** | 224/256/384/512 bits | ✅ Sim | Algoritmo Keccak |

**MD5** (⚠️ PROVÁVEL NO TESTE): Produz hash de 128 bits. Garante integridade mas é INSEGURO por vulnerabilidade a colisões. Usar SHA-256 em vez disso.

**MAC (Message Authentication Code):**
- Usa uma chave partilhada
- Garante **autenticação** + **integridade**
- Tipos: Cifras de bloco e HMAC

**Paradoxo do Aniversário**: Com N bits de hash, segurança máxima = 2^(N/2) (probabilidade 50% de colisão num grupo de 2^(N/2) hashes)

### 2.9 Assinatura Digital (⚠️ PROVÁVEL NO TESTE)

**Processo de assinar:**
1. Remetente cria um **hash** da mensagem (ex: SHA-256)
2. Remetente **cifra o hash** com a sua **chave privada** → assinatura digital
3. Envia a mensagem original + assinatura digital

**Processo de verificar:**
1. Destinatário decifra a assinatura com a **chave pública** do remetente → obtém hash original
2. Destinatário calcula o hash da mensagem recebida
3. Compara os dois hashes: se iguais → mensagem íntegra e autêntica

**Garante**: Integridade + Autenticação + Não-repudiação

### 2.10 Steganografia

- Arte de esconder mensagens dentro de outras mensagens (ex: dentro de imagens)
- **NÃO É criptografia** — o objetivo é esconder a existência da mensagem, não cifrá-la
- Uso: provar direitos de autor (watermark)

---

## 3. Autenticação e Autorização (⚠️ MUITO PROVÁVEL NO TESTE)

### 3.1 Sistemas AAA

| Componente | Função | Exemplo |
|------------|--------|---------|
| **Authentication** (Autenticação) | Provar identidade | Login com username/password |
| **Authorization** (Autorização) | Permissões associadas à identidade | Utilizador X pode ler mas não escrever |
| **Accounting** (Contabilidade) | Rastreabilidade e auditoria | Logs de quem acedeu o quê e quando |

### 3.2 Factores de Autenticação (⚠️ PROVÁVEL NO TESTE)

| Factor | Descrição | Exemplo |
|--------|-----------|---------|
| **Algo que se sabe** | Conhecimento | Password, PIN |
| **Algo que se tem** | Posse | Smartcard, token, telemóvel |
| **Algo que se é** | Inerência/Biometria | Impressão digital, retina, face |
| Algo que se faz | Comportamento | Padrão de escrita, teclas |
| Onde se está | Localização | GPS |

**Autenticação forte/multifator (MFA)**: Pelo menos 2 factores diferentes combinados.

### 3.3 Biometria

- Impressão digital, retina, íris, geometria da mão, reconhecimento facial, voz, escrita
- **FAR** (False Acceptance Rate): Aceitar um impostor
- **FRR** (False Rejection Rate): Rejeitar o utilizador legítimo
- **CER/EER** (Cross/Equal Error Rate): Ponto ideal onde FAR = FRR

**Fases**: Registo (enrollment) → Verificação → Identificação

### 3.4 Ataques a Passwords (⚠️ PROVÁVEL NO TESTE)

| Ataque | Descrição | Contramedida |
|--------|-----------|--------------|
| **Força Bruta** | Tenta TODAS as combinações | Bloqueio após N tentativas, passwords longas |
| **Dicionário** | Testa palavras comuns/previsíveis | Passwords com caracteres especiais e números |
| **Rainbow Tables** | Tabelas pré-computadas de hashes | Usar **salt** (valor aleatório adicionado antes do hash) |
| **Phishing** | Enganar utilizador para revelar credenciais | Educação + MFA |

### 3.5 Protocolos de Autenticação

| Protocolo | Como funciona |
|-----------|---------------|
| **PAP** | Password enviada em CLARO (inseguro!) |
| **CHAP** | Challenge-Response: servidor envia desafio, cliente responde com desafio cifrado |
| **RADIUS** | Sistema AAA centralizado: múltiplos dispositivos autenticam num ponto central |
| **OTP** | Password usada 1 vez só, depois inválida |
| **Kerberos** | KDC + tickets com expiração temporal |

### 3.6 OTP (One Time Password)

- S/Key (Lamport): Gera hashes consecutivos; usa lista em ordem inversa
- Time-based token: Sincronização temporal, expiração curta (~1 min)
- Chave partilhada no servidor e no token

### 3.7 Single Sign-On (SSO)

- Autenticar-se 1 vez → acesso a múltiplos sistemas sem re-autenticar
- **Vantagem**: Facilita usabilidade e gestão
- **Risco**: Se comprometido, atacante acede a TUDO
- **Mitigação**: Usar MFA + re-autenticação periódica
- **Exemplo**: Kerberos

### 3.8 Políticas de Controlo de Acesso (⚠️ PROVÁVEL NO TESTE)

| Política | Descrição | Prós/Contras |
|----------|-----------|--------------|
| **DAC** (Discretionary) | Dono do recurso controla acesso | Flexível MAS utilizadores podem ser negligentes |
| **MAC** (Mandatory) | Rótulos de segurança estáticos, política global | Rígido e seguro, usado em militares (Bell-LaPadula, Biba) |
| **RBAC** (Role-Based) | Acesso baseado na função/cargo na organização | **MAIS USADO** nas empresas: escalável, hierárquico, fácil de gerir |

**RBAC é o mais frequente nas organizações** porque:
- É escalável
- Permite hierarquia e herança de permissões
- Facilita gestão (alterações aplicadas a grupos)
- Reduz risco de acesso não autorizado

**DAC** — problemas: utilizadores sem noções de segurança + malware pode enganar para receber privilégios

**MAC** — sem transferência de permissões, "need to know"

### 3.9 Matrizes de Controlo de Acesso

- **Matriz**: Sujeitos × Objectos × Privilégios (Own, Read, Write, eXecute)
- **ACL** (Access Control List): Visão a partir do OBJECTO (quem pode aceder a este ficheiro?)
- **Lista de Capacidades**: Visão a partir do SUJEITO (a que objectos pode este utilizador aceder?)

---

## 4. Gestão de Chaves

### 4.1 Problemas da Gestão de Chaves

- **Simétrica**: Não é escalável, risco de intercepção da chave secreta
- **Assimétrica**: Risco de personificação (o receptor pode não ser quem diz ser)
- **Geração**: Dispositivos electrónicos têm dificuldade em gerar aleatoriedade
- **Confinamento**: Chaves devem ser geradas/guardadas em dispositivos seguros (smartcard, token, TCB)

### 4.2 Tipos de Chaves por Duração

- **Chaves de longa duração (mestras)**: Usadas para gerar/proteger chaves de sessão
- **Chaves de curta duração (sessão)**: Temporárias, renegociação periódica

> Demasiada utilização de uma chave facilita a sua descoberta.

### 4.3 KDC (Key Distribution Center)

- Distribuição centralizada de chaves
- Cada nó partilha uma chave simétrica com o KDC
- Quando A quer falar com B → KDC cria chave partilhada e envia cifrada a ambos
- **Problema**: Ponto único de confiança E de falha

### 4.4 Kerberos

- Baseado no protocolo Needham-Schroeder (simétrico)
- Composto por: **Authentication Server** + **Ticket Granting Service**
- Trusted third party com sincronização temporal (tickets expiram)

### 4.5 PKI (Public Key Infrastructure)

- Funções: Registo, assinatura, validação e revogação de certificados
- **Certificado Digital**: Liga chave pública a uma entidade (validada por CA)
- **CA** (Certificate Authority): Autoridade certificadora que assina certificados
- **RA** (Registration Authority): Autoridade de registo separada

**Cadeia de certificados**: Hierarquia de confiança — verifica-se desde o certificado até encontrar uma CA de confiança.

### 4.6 Formato X.509

- Framework de formato para certificados
- Liga certificado a: endereço web, email, username
- Define propósito: assinatura, autenticação, cifrar, ou combinações

### 4.7 Revogação de Certificados (CRL)

- **CRL** (Certificate Revocation List): Lista periódica de certificados revogados, assinada pela CA
- Verificação: no processo de validação, consultar CRL para confirmar validade

### 4.8 PGP (Pretty Good Privacy)

- Cifra assimétrica para email e ficheiros
- Sem hierarquia predefinida → **Web of Trust** (confiança transitiva)
- Cada nó nomeia o nível de confiança em outros nós
- Usa cifra assimétrica para trocar chave de sessão (simétrica)

### 4.9 Key Escrow (Recuperação de Chaves)

- Informação para recuperar chave privada guardada na CA ou terceiro confiável
- Útil para disputas legais e chaves associadas a funções empresariais
- **Problema**: Vai contra o princípio de não-repudiação

---

## 5. Firewalls (⚠️ PROVÁVEL NO TESTE)

### 5.1 Objetivo

- Monitorizar e validar acessos entre redes
- Usa regras pré-definidas: autoriza o que está permitido, **NEGA tudo o resto**
- **Ponto único de controlo** — não pode haver tráfego que circunde a firewall
- Não pode haver intrusão na própria firewall

### 5.2 Tipos de Firewall

| Tipo | Camada | Funcionalidade | Prós | Contras |
|------|--------|---------------|------|---------|
| **Packet Filter** | Rede (cabeçalho) | Filtra por IP origem/destino, port, protocolo | Simples e rápido | Sem estado, sem conhecimento aplicacional, logging limitado |
| **Stateful Inspection** | Rede + Estado | Packet filter + tabela de estados de ligações | Conhece protocolos comuns, suporta FTP activo | — |
| **Proxy** | Aplicação | Intermediário que analisa TODO o pacote | Analisa conteúdo, autenticação adicional, caching | Mais complexo, pode não suportar protocolos novos |

**Subtipos de Proxy:**
- **Circuit Gateway (SOCKS)**: Camada de sessão, vários protocolos
- **Application Gateway**: Específico por protocolo (SMTP relay, web proxy)

### 5.3 Para filtrar conteúdo web → Proxy Firewall (⚠️ PROVÁVEL NO TESTE)

**Justificação**: O proxy atua como intermediário na camada de aplicação, inspecionando o conteúdo HTTP/HTTPS. Pode:
- Bloquear sites por categoria/reputação
- Identificar malware e phishing
- Controlar acesso granular por políticas da organização
- Fornecer autenticação adicional

### 5.4 DMZ (Zona Desmilitarizada)

- Segmento neutro: NÃO é rede interna, NÃO é rede externa
- Fica entre 2 firewalls (ou num interface diferente de 1 firewall)
- Hospeda serviços expostos: HTTP, DNS, SMTP
- Conceito militar: zona segura entre faixas de conflito

### 5.5 NAT (Network Address Translation)

- Mapeamento de IPs e ports entre diferentes redes
- Limita exposição do endereçamento interno e serviços
- Mantém lista centralizada dos mapeamentos

### 5.6 Arquitectura Multi-Firewall

- **Defense-in-depth**: Várias firewalls de fabricantes diferentes
- Se uma vulnerabilidade afecta uma, não afecta a outra
- **Redundância**:
  - Load Balancing: Tráfego dividido, todas online
  - Activa/Passiva: Uma online, outra em standby

---

## 6. IDS/IPS (Detecção e Prevenção de Intrusões) (⚠️ PROVÁVEL NO TESTE)

### 6.1 Objetivo do IDS

- Detectar ataques conhecidos E desconhecidos
- Alertar atempadamente
- Minimizar **falsos positivos** (alerta falso) e **falsos negativos** (ataque não detectado)
- Manter-se escondido/não detectável
- Não comprometer o normal uso de recursos

### 6.2 Tipos de IDS por Método de Detecção

| Tipo | Como funciona | Prós | Contras |
|------|---------------|------|---------|
| **Baseado em assinaturas** | Compara com padrões de ataques conhecidos (regras) | Detecção precisa de ataques conhecidos | Precisa actualizações constantes; não detecta 0-days |
| **Baseado em anomalias** | Análise estatística + machine learning; detecta desvios do comportamento normal | Detecta ataques novos/desconhecidos | Precisa baseline; anomalia ≠ ataque; requer tuning |

### 6.3 Network IDS vs Host IDS (⚠️ PROVÁVEL NO TESTE)

| | Network IDS (NIDS) | Host IDS (HIDS) |
|--|--------------------:|:-----------------|
| **Localização** | Ponto estratégico da rede (router, switch, port mirroring) | Instalado no host individual |
| **Monitoriza** | Tráfego de rede entre múltiplos destinos | Logs, ficheiros, processos, memória do host |
| **Tráfego cifrado** | ❌ NÃO consegue analisar | ✅ Sim (reside onde é decifrado) |
| **Detecção** | Vê o ataque mas não sabe se teve sucesso | Sabe se a intrusão teve sucesso |
| **Impacto** | Não afecta hosts (fail-open) | Pode afectar performance do host |
| **Vantagem** | Visão global do tráfego | Conhecimento aplicacional detalhado |
| **Desvantagem** | Não vê resultado do ataque | Atacante pode desligá-lo |

### 6.4 IPS (Intrusion Prevention System)

- IDS + capacidade de **actuar automaticamente**
- Quando detecta ataque: bloqueia na firewall, desconecta máquina
- **Risco**: Se for falso positivo → nega acesso a utilizadores legítimos

### 6.5 Técnicas de Evasão de IDS

- Sobrecarga (DoS) para esgotar recursos do IDS
- Ataques espaçados no tempo (abaixo do threshold)
- Fragmentação de pacotes para dar visão diferente ao IDS
- Pacotes com baixo TTL (chegam ao IDS mas não ao alvo)

### 6.6 Resposta a Intrusões

1. **Preparação**: Planeamento, instalação e configuração de IDS
2. **Identificação**: Detectar a intrusão
3. **Contenção**: Isolar o sistema vítima
4. **Erradicação**: Eliminar a ameaça
5. **Recuperação**: Restaurar o sistema
6. **Reajustamento**: Lições aprendidas, follow-up, possíveis acções legais

### 6.7 Honeypots (⚠️ PROVÁVEL NO TESTE)

**O que é**: Sistema/recurso de rede propositadamente vulnerável para ATRAIR e ENGANAR atacantes.

**Para que serve** (APRENDER!):
- Conhecer métodos e técnicas dos atacantes
- Identificar fragilidades reais
- Avaliar nível de risco
- Desviar atenção dos sistemas reais
- Limita falsos positivos (nenhum tráfego legítimo deve chegar a um honeypot)

**Taxonomia:**

| Eixo | Opções |
|------|--------|
| Objetivo | Investigação / Produção |
| Interacção | Baixa / Média / Alta |
| Instalação | Física / Virtual |
| Comportamento | Estático / Dinâmico |

**Honeytoken**: Item monitorizado em localização sensível (ex: ficheiro falso com credenciais falsas)

---

## 7. Comunicação Segura

### 7.1 VPN (Virtual Private Network)

- Estabelece comunicação isolada/privada criando um **túnel** dentro de outra rede (overlay network)
- Usos: Acesso individual externo à rede interna; cifrar tráfego entre localizações

### 7.2 VLAN (Virtual LAN)

- Cria redes segmentadas dentro de uma rede local
- Actua na camada de data link com labels
- Dados só circulam dentro da mesma VLAN
- **SEM** integridade nem confidencialidade

### 7.3 IPSec

**O que faz**: Cifra e autentica TODO o tráfego na camada de rede IP.

**Garante**: Confidencialidade + Integridade + Não-repudiação

**Extension Headers:**

| Header | Garante | Algoritmos |
|--------|---------|-----------|
| **AH** (Authentication Header) | Integridade + Autenticidade (MAC) | HMAC-MD5, HMAC-SHA1 |
| **ESP** (Encapsulating Security Payload) | Confidencialidade (+ opcionalmente integridade) | 3DES, RC5, IDEA, Blowfish + HMAC |

**Modos de Operação:**

| Modo | Descrição | Uso |
|------|-----------|-----|
| **Transporte** | Protege camadas acima de IP | Host-to-Host (end-to-end) |
| **Túnel** | Pacote IP dentro de novo pacote IP | Host-to-Gateway, Gateway-to-Gateway |

**Security Associations (SA):**
- Relação 1 sentido (tráfego bidirecional = 2 SAs)
- **IKE** (Internet Key Exchange): protocolo de troca de chaves
- **SPD** (Security Policy Database): decide o que fazer com pacotes
- Parâmetros: IP destino, AH ou ESP, SPI (identifica a SA)

**Problemas com NAT:**
- NAT altera header IP (mas AH autentica o header!)
- NAT altera checksum TCP/UDP (que está cifrado por ESP!)
- Solução: **NAT-Traversal** — encapsular ESP em UDP

### 7.4 SSL/TLS

- **SSL 1.0/2.0**: Netscape 1994 (vulneráveis)
- **SSL 3.0**: Última versão SSL
- **TLS 1.0**: Primeira alternativa padronizada (= SSL 3.1)
- **TLS 1.2/1.3**: Usados actualmente

**4 Sub-protocolos:**
1. **Handshake Protocol**: Negocia e estabelece comunicação segura
2. **Record Protocol**: Fragmentação, compressão, integridade, confidencialidade
3. **Change Cipher Protocol**: Mudar algoritmos em uso
4. **Alert Protocol**: Gestão de anomalias

**Handshake simplificado:**
1. Client_hello: versão, random, cipher suites suportadas
2. Server_hello: escolhe cipher suite + envia certificado
3. Troca de chaves (RSA ou DH)
4. Change_cipher + Finished (ambos os lados)

**Ataques a SSL:**
- Mudar https → http nos links
- Favicon como cadeado falso
- Homograph attack (caracteres Unicode parecidos)
- Certificados wildcard fraudulentos
- Colisões MD5 para forjar certificados
- Heartbleed (vulnerabilidade de implementação no OpenSSL)

### 7.5 SSH (Secure Shell)

- Comunicação segura sobre TCP
- Funcionalidades: shell remota, cópia de ficheiros, túneis (VPN dos pobres)
- Versão 1 tem vulnerabilidades → usar Versão 2

### 7.6 Segurança Wireless

#### WEP (Wired Equivalent Privacy) — INSEGURO

- Chaves estáticas partilhadas (40 ou 104 bits) criadas manualmente
- Integridade: CRC (NÃO é criptográfico!)
- Confidencialidade: RC4
- IV (Initialization Vector): apenas 24 bits (público)

**Problemas do WEP:**
- Replay possível
- CRC não garante integridade real
- IV repete-se (24 bits é pouco)
- Chaves não expiram nem são redistribuídas
- Sem autenticação mútua

#### WPA (TKIP)

- Gestão de chaves: múltiplas chaves mestras + renegociação periódica
- Usa RC4 MAS gera chave única por frame (128 bits)
- Contador de sequência (previne replay)
- MIC (Message Integrity Check) com algoritmo Michael (64 bits)
- Reage a falhas de integridade: desliga cliente e renegocia

#### WPA2 (CCMP) — Recomendado

- Usa **AES** (128, 192, 256 bits)
- Modo Counter: confidencialidade
- Modo CBC-MAC: integridade + autenticidade
- Mantém medidas do TKIP: contador sequência, renegociação, chaves únicas
- Blocos de 128 bits

#### Ataques Wireless (WPA2)

- Maioria são falhas de **implementação** dos fabricantes
- **WPS** (PIN): Brute-force do PIN
- Geração de chave a partir de MAC/SSID (segurança por obscuridade)
- **PMKID**: Permite ataque offline

---

## 8. Resumo das Perguntas Mais Prováveis no Teste

Com base nas NOTAS_TESTE, estas são as perguntas que provavelmente aparecerão:

| # | Tema | Secção |
|---|------|--------|
| 1 | Definir CIA (Confidencialidade, Integridade, Disponibilidade) | 1.1 |
| 2 | 4 tipos de controlos de segurança + exemplos | 1.4 |
| 3 | 4 princípios de Saltzer & Schroeder + explicação | 1.5 |
| 4 | Comparar cifra simétrica de bloco vs fita (stream) | 2.2 |
| 5 | Comparar cifra simétrica vs assimétrica | 2.4 |
| 6 | Comparar DES vs AES | 2.5 |
| 7 | Processo de envio com cifra assimétrica (confidencialidade) | 2.6 |
| 8 | O que é MD5 | 2.8 |
| 9 | Processo de assinatura digital + verificação | 2.9 |
| 10 | Sistemas AAA | 3.1 |
| 11 | 3 factores de autenticação + exemplos | 3.2 |
| 12 | Política de controlo de acesso mais frequente (RBAC) | 3.8 |
| 13 | Ataque para descobrir password | 3.4 |
| 14 | Firewall para filtrar conteúdo web (Proxy) | 5.3 |
| 15 | Comparar Host IDS vs Network IDS | 6.3 |
| 16 | O que é um Honeypot e para que serve | 6.7 |

---

## 9. Dicas para o Teste

- **6 perguntas teóricas + 2 práticas** (ferramentas das aulas)
- **JUSTIFICAR TUDO** — o professor é rigoroso
- Nada de romances: ser conciso mas completo
- Parte prática: saber para que servem as ferramentas usadas nas aulas e como se utilizam
- Compreender os conceitos ao máximo, não decorar
- Ver qual é a parte da matéria com mais fragilidades e focar aí

---

*Bom estudo! 💪*
