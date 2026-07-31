# 🏦 Miniguia de estudos: Open Finance no Brasil com NotebookLM

![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Bootcamp](https://img.shields.io/badge/Bootcamp-Santander%20%2B%20DIO-red)
![Tema](https://img.shields.io/badge/Tema-Open%20Finance-blue)

## 📑 Índice

- Contexto
- Objetivo
- Curadoria de fontes
- Engenharia de prompts
- Miniguia de estudos
    - Resumos estruturados
    - Glossário
    - Prompts reutilizáveis
- Aprendizados

## 📌 Contexto

Este projeto foi desenvolvido como parte do Bootcamp Santander em parceria com a DIO, explorando o uso do NotebookLM como ferramenta de aprendizagem ativa.

O tema escolhido foi Open Finance, uma iniciativa que vem transformando o sistema financeiro brasileiro por meio do compartilhamento seguro de dados, permitindo novas experiências para consumidores, instituições financeiras e fintechs.

## 🎯 Objetivo

Compreender como o Open Finance está transformando o sistema financeiro brasileiro, explorando seus benefícios, desafios, regulamentação e impactos para consumidores, instituições financeiras e fintechs.

## 📚 Curadoria de fontes

Para garantir a acurácia técnica do NotebookLM, selecionei 8 fontes de alta autoridade e diversidade metodológica, contemplando conteúdos em texto e vídeo de órgãos reguladores, instituições financeiras, especialistas do setor, entidades do consumidor e portais de notícias especializados:

* **Fontes em texto:** 
  1. **[Banco Central do Brasil]** [Visão Geral e Normativa do Open Finance](https://www.bcb.gov.br/estabilidadefinanceira/openfinance)
  2. **[Banco Central do Brasil]** [Diretrizes de Segurança e Proteção de Dados](https://www.bcb.gov.br/estabilidadefinanceira/seguranca-open-finance)
  3. **[Banco Central do Brasil]** [FAQ Oficial do Open Finance](https://bcb.gov.br/meubc/faqs/s/open-finance)
  4. **[Santander Brasil]** [Open Finance na Prática Bancária](https://www.santander.com.br/banco/open-finance/)
  5. **[IDEC]** [Tudo o que você precisa saber sobre Open Banking/Finance](https://idec.org.br/dicas-e-direitos)
  6. **[Finsiders Brasil]** [Brasil lidera Open Finance no mundo e alcança marca histórica](https://finsidersbrasil.com.br/economia-open/brasil-lidera-open-finance-no-mundo-com-100-milhoes-de-clientes/)
  7. **[Valor Investe]** [Open Finance para Empresas: Desafios e Burocracia no Crédito B2B](https://valorinveste.globo.com/produtos/servicos-financeiros/)

* **Fontes em vídeo:**
  1. **[Ministério da Fazenda / Banco Central]** [Live BC: Como funciona o Open Finance e como utilizar o ecossistema](https://www.gov.br/fazenda/pt-br/composicao/orgaos/orgaos-colegiados/crsfn/acesso-a-informacao/noticias/2024/livebc-detalhou-como-funciona-o-open-finance-e-como-utilizar-o-ecossistema)

## 🧠 Engenharia de prompts

Nesta seção, registrei a evolução dos prompts utilizados dentro do NotebookLM para extrair análises estratégicas das fontes.

### Teste 1: Exploração inicial
* **Prompt V1:** *"O que é Open Finance?"*
  
* **Prompt V2:** *"Explique o que é o Open Finance, seus principais objetivos e como ele funciona no sistema financeiro brasileiro."*

    <details>
    <summary><strong>Resposta</strong></summary>

  O Open Finance (anteriormente conhecido como Open Banking) é uma infraestrutura tecnológica e regulatória que permite o compartilhamento padronizado de dados, produtos e serviços financeiros entre instituições autorizadas pelo Banco Central do Brasil (BCB), por meio de plataformas integradas via APIs (Interfaces de Programação de Aplicativos).

  A transição do nome para Open Finance ocorreu para refletir a ampliação do seu escopo, que passou a abranger não apenas serviços bancários tradicionais, mas também o compartilhamento de dados de investimentos, seguros, previdência complementar e operações de câmbio.

  A sua premissa central é que os dados financeiros pertencem ao cliente, e não às instituições. Isso inverte o eixo de poder do mercado, garantindo ao consumidor (pessoa física ou jurídica) a soberania para decidir com quem, como e por quanto tempo deseja compartilhar seu histórico financeiro.

  #### Principais Objetivos

  O desenho regulatório do Open Finance pelo Banco Central foi pautado em quatro pilares fundamentais:

  - **Promover a concorrência:** Ao quebrar o monopólio histórico que as grandes instituições tínhamos sobre as informações de seus clientes, o sistema nivela as condições de disputa no mercado, permitindo que novos entrantes (como fintechs) concorram de forma mais justa.
  - **Incentivar a inovação:** Facilita a criação de novos modelos de negócios e soluções financeiras personalizadas baseadas no comportamento real do usuário.
  - **Aumentar a eficiência:** Otimiza o funcionamento do Sistema Financeiro Nacional (SFN) e do Sistema de Pagamentos Brasileiro (SPB), tornando os processos mais ágeis e menos custosos.
  - **Promover a inclusão e cidadania financeira:** Facilita o acesso a produtos financeiros mais adequados e com taxas menores, além de ajudar a bancarizar e oferecer crédito a parcelas da população e pequenos empreendedores que antes eram penalizados pela falta de um histórico formal.

  #### Como funciona no Sistema Financeiro Brasileiro

  **1. Implementação em Fases**

  O ecossistema foi estruturado de forma gradual em quatro fases:
  - **Fase 1:** Compartilhamento de dados abertos das próprias instituições, como canais de atendimento, produtos oferecidos e suas respectivas taxas.
  - **Fase 2:** Compartilhamento de dados cadastrais e do histórico transacional dos clientes (contas, cartões e crédito).
  - **Fase 3:** Iniciação de transações de pagamento (permitindo realizar um Pix fora do ambiente do banco, por exemplo) e encaminhamento de propostas de crédito.
  - **Fase 4:** Compartilhamento de dados de produtos complexos (investimentos, previdência, seguros e câmbio).

  **2. A Jornada de Compartilhamento**

  Nenhum dado é movido sem a vontade do usuário. O processo exige três etapas estritas que ocorrem nos canais digitais dos bancos envolvidos: consentimento prévio, autenticação da identidade e confirmação do que será compartilhado. O usuário tem o controle para definir o prazo de validade (limitado a 12 meses, mas com regras recentes de simplificação) e pode revogar a permissão a qualquer momento.

  **3. Participantes do Ecossistema**

  O sistema conta com participantes obrigatórios, que englobam os grandes conglomerados bancários (segmentos S1 e S2) e instituições com mais de 5 milhões de clientes ativos, e participantes voluntários, que podem aderir ao sistema respeitando a regra da reciprocidade (quem recebe dados também deve estar apto a enviá-los). As instituições podem exercer os papéis de transmissoras de dados, receptoras de dados, provedoras de contas ou iniciadoras de transação de pagamento (ITPs).

  **4. Governança e Segurança**

  A operação do Open Finance não centraliza dados em um único banco de dados do Banco Central; as informações trafegam diretamente entre a instituição que envia e a que recebe, através de APIs padronizadas com forte criptografia. Todo o modelo obedece rigorosamente à Lei Geral de Proteção de Dados (LGPD) e às exigências de segurança cibernética do BCB. O dia a dia e os padrões técnicos são geridos por uma Estrutura de Governança Definitiva, formada por associações representativas do mercado (bancos, fintechs, meios de pagamento) e supervisionada pelo Banco Central.

  #### Impactos Práticos

  No dia a dia, o Open Finance converte-se em melhorias palpáveis:

  - **Análise de crédito mais justa:** Os bancos passam a analisar o fluxo de caixa real, a renda recorrente e o comportamento atual do cliente, superando a visão restrita do score tradicional de birôs de crédito (que focam muito no histórico de negativações). Com isso, clientes podem conseguir redução nas taxas de juros, aumento de limites e até aprovação de crédito para autônomos.
  - **Portabilidade de crédito 100% digital:** O sistema elimina a burocracia documental para que o consumidor transfira dívidas e empréstimos para o banco que oferecer a taxa mais barata.
  - **Gestão Consolidada:** É possível usar apenas o aplicativo do seu banco favorito para enxergar saldos, investimentos e limites de todas as outras contas que você possui.
  - **Pagamentos Inovadores:** Em conjunto com o Pix, o ecossistema permite "pagamentos agênticos" e transações iniciadas por aplicativos de terceiros ou lojas online, reduzindo etapas na hora de fechar uma compra (Jornada Sem Redirecionamento) e facilitando serviços como o Pix Automático.

  </details>

* **Análise:** A resposta apresentou uma visão ampla sobre o Open Finance, abordando seus principais conceitos, benefícios e aspectos relacionados à segurança. Entretanto, por se tratar de um prompt bastante abrangente, o conteúdo teve um caráter predominantemente introdutório. Para aprofundar o estudo e obter uma compreensão mais estruturada do tema, o próximo prompt buscará explorar seus objetivos e funcionamento no contexto do sistema financeiro brasileiro.
* **Prompt V2:** *"Explique o que é o Open Finance, seus principais objetivos e como ele funciona no sistema financeiro brasileiro."*

<details>
<summary><strong>Resposta</strong></summary>

The Open Finance (anteriormente conhecido como Open Banking) é uma infraestrutura tecnológica e regulatória que permite o compartilhamento padronizado de dados, produtos e serviços financeiros entre instituições autorizadas pelo Banco Central do Brasil (BCB), por meio de plataformas integradas via APIs (Interfaces de Programação de Aplicativos).

A transição do nome para Open Finance ocorreu para refletir a ampliação do seu escopo, que passou a abranger não apenas serviços bancários tradicionais, mas também o compartilhamento de dados de investimentos, seguros, previdência complementar e operações de câmbio.

A sua premissa central é que os dados financeiros pertencem ao cliente, e não às instituições. Isso inverte o eixo de poder do mercado, garantindo ao consumidor (pessoa física ou jurídica) a soberania para decidir com quem, como e por quanto tempo deseja compartilhar seu histórico financeiro.

#### Principais Objetivos

O desenho regulatório do Open Finance pelo Banco Central foi pautado em quatro pilares fundamentais:

- **Promover a concorrência:** Ao quebrar o monopólio histórico que as grandes instituições tinham sobre as informações de seus clientes, o sistema nivela as condições de disputa no mercado, permitindo que novos entrantes (como fintechs) concorram de forma mais justa.
- **Incentivar a inovação:** Facilita a criação de novos modelos de negócios e soluções financeiras personalizadas baseadas no comportamento real do usuário.
- **Aumentar a eficiência:** Otimiza o funcionamento do Sistema Financeiro Nacional (SFN) e do Sistema de Pagamentos Brasileiro (SPB), tornando os processos mais ágeis e menos custosos.
- **Promover a inclusão e cidadania financeira:** Facilita o acesso a produtos financeiros mais adequados e com taxas menores, além de ajudar a bancarizar e oferecer crédito a parcelas da população e pequenos empreendedores que antes eram penalizados pela falta de um histórico formal.

#### Como funciona no Sistema Financeiro Brasileiro

**1. Implementação em Fases**

O ecossistema foi estruturado de forma gradual em quatro fases:
- **Fase 1:** Compartilhamento de dados abertos das próprias instituições, como canais de atendimento, produtos oferecidos e suas respectivas taxas.
- **Fase 2:** Compartilhamento de dados cadastrais e do histórico transacional dos clientes (contas, cartões e crédito).
- **Fase 3:** Iniciação de transações de pagamento (permitindo realizar um Pix fora do ambiente do banco, por exemplo) e encaminhamento de propostas de crédito.
- **Fase 4:** Compartilhamento de dados de produtos complexos (investimentos, previdência, seguros e câmbio).

**2. A Jornada de Compartilhamento**

Nenhum dado é movido sem a vontade do usuário. O processo exige três etapas estritas que ocorrem nos canais digitais dos bancos envolvidos: consentimento prévio, autenticação da identidade e confirmação do que será compartilhado. O usuário tem o controle para definir o prazo de validade (limitado a 12 meses, mas com regras recentes de simplificação) e pode revogar a permissão a qualquer momento.

**3. Participantes do Ecossistema**

O sistema conta com participantes obrigatórios, que englobam os grandes conglomerados bancários (segmentos S1 e S2) e instituições com mais de 5 milhões de clientes ativos, e participantes voluntários, que podem aderir ao sistema respeitando a regra da reciprocidade (quem recebe dados também deve estar apto a enviá-los). As instituições podem exercer os papéis de transmissoras de dados, receptoras de dados, provedoras de contas ou iniciadoras de transação de pagamento (ITPs).

**4. Governança e Segurança**

A operação do Open Finance não centraliza dados em um único banco de dados do Banco Central; as informações trafegam diretamente entre a instituição que envia e a que recebe, através de APIs padronizadas com forte criptografia. Todo o modelo obedece rigorosamente à Lei Geral de Proteção de Dados (LGPD) e às exigências de segurança cibernética do BCB. O dia a dia e os padrões técnicos são geridos por uma Estrutura de Governança Definitiva, formada por associações representativas do mercado (bancos, fintechs, meios de pagamento) e supervisionada pelo Banco Central.

#### Impactos Práticos

No dia a dia, o Open Finance converte-se em melhorias palpáveis:

- **Análise de crédito mais justa:** Os bancos passam a analisar o fluxo de caixa real, a renda recorrente e o comportamento atual do cliente, superando a visão restrita do score tradicional de birôs de crédito (que focam muito no histórico de negativações). Com isso, clientes podem conseguir redução nas taxas de juros, aumento de limites e até aprovação de crédito para autônomos.
- **Portabilidade de crédito 100% digital:** O sistema elimina a burocracia documental para que o consumidor transfira dívidas e empréstimos para o banco que oferecer a taxa mais barata.
- **Gestão Consolidada:** É possível usar apenas o aplicativo do seu banco favorito para enxergar saldos, investimentos e limites de todas as outras contas que você possui.
- **Pagamentos Inovadores:** Em conjunto com o Pix, o ecossistema permite "pagamentos agênticos" e transações iniciadas por aplicativos de terceiros ou lojas online, reduzindo etapas na hora de fechar uma compra (Jornada Sem Redirecionamento) e facilitando serviços como o Pix Automático.

</details>
  
* **Reflexão:** Mudar a abordagem de "o que é" para "análise comparativa com foco em dor de mercado" gerou insights muito mais ricos e aplicáveis a negócios.

### 🔬 Teste 2: Extração para Segurança e Consentimento (LGPD)
* **Prompt Aplicado:** *"Resuma como a segurança dos dados e o consentimento do cliente são tratados no ecossistema, citando as garantias do BACEN e as orientações do IDEC."*
* **Desafio Encontrado (Cicatriz):** A IA tendia a generalizar a LGPD sem citar mecanismos práticos.
* **Solução:** Adicionei a instrução: *"Destaque obrigatoriamente a revogabilidade do consentimento e a responsabilidade das instituições envolvidas."*

---
  
## 📘 Miniguia de estudos

### 📌 Resumos estruturados

#### 1. O que é o Open Finance?
O Open Finance (Sistema Financeiro Aberto) é uma infraestrutura tecnológica e regulatória que permite o compartilhamento padronizado de dados e serviços financeiros entre instituições, por meio de plataformas seguras integradas via APIs (*Interfaces de Programação de Aplicativos*).

Ele é a evolução direta do *Open Banking*: enquanto o modelo anterior focava em produtos bancários tradicionais, o Open Finance engloba também investimentos, seguros, previdência e câmbio. Sua premissa principal é que os dados financeiros pertencem ao cliente, que passa a ter total controle para decidir com quem, quando e o que deseja compartilhar.

---

#### 2. Por que o Open Finance surgiu?
O sistema financeiro brasileiro era historicamente muito concentrado, fazendo com que os grandes bancos detivessem o monopólio das informações financeiras de seus clientes. Esse "empoçamento" de dados dificultava a entrada de concorrentes e impedia que os clientes conseguissem ofertas melhores em outras instituições.

O Banco Central desenhou o Open Finance como uma política pública para:
* **Promover a concorrência:** Quebrar a assimetria de informações para que novos entrantes e *fintechs* possam disputar clientes de forma justa.
* **Aumentar a eficiência e inovação:** Incentivar a criação de novos modelos de negócios e soluções financeiras no Brasil.
* **Impulsionar a cidadania financeira:** Incluir a população e facilitar o acesso a crédito mais adequado e barato.

---

#### 3. Como funciona o compartilhamento de dados?
Não existe um "banco de dados centralizado". Os dados trafegam diretamente entre a instituição que os possui e a que os recebe, através de APIs criptografadas e seguindo normas rigorosas da LGPD (*Lei Geral de Proteção de Dados*).

A jornada digital ocorre nos próprios aplicativos dos bancos e exige três etapas obrigatórias:
1. **Consentimento:** O cliente escolhe livremente quais dados compartilhar, a instituição de destino e o prazo de validade (limitado a 12 meses, revogável a qualquer momento).
2. **Autenticação:** O cliente é redirecionado ao seu banco original para confirmar sua identidade (via senha ou biometria).
3. **Confirmação:** O cliente revisa um resumo do que será compartilhado e finaliza a operação.

---

#### 4. Quem participa do ecossistema?
O ecossistema é regulado pelo Banco Central e gerenciado no dia a dia pela Estrutura de Governança Definitiva (Associação Open Finance). 

A participação no compartilhamento de dados é obrigatória para os grandes bancos (segmentos S1 e S2) e conglomerados com mais de 5 milhões de clientes. Outras instituições podem aderir de forma voluntária, desde que respeitem a *regra da reciprocidade* (se recebem dados, também devem compartilhar).

Os participantes assumem diferentes papéis:
* **Transmissora de Dados:** A instituição que envia as informações.
* **Receptora de Dados:** A instituição que solicita e recebe as informações autorizadas.
* **Detentora de Conta:** Instituição onde o cliente mantém seu dinheiro.
* **Iniciadora de Transação de Pagamento (ITP):** Instituição autorizada a comandar pagamentos (como o Pix) a partir de plataformas de terceiros, sem reter o dinheiro durante o processo.

---

#### 5. Quais são os benefícios do Open Finance?
* **Análise de crédito comportamental:** Ao invés de usar apenas o *score* baseado em dívidas, as instituições podem ver o fluxo de caixa real, os investimentos e a renda recorrente. Isso ajuda a aprovar crédito para autônomos e negativados recuperados, reduzindo taxas de juros.
* **Gestão financeira unificada:** O cliente pode usar seu aplicativo favorito (*agregador*) para visualizar saldos, faturas e limites de todos os seus bancos em uma única tela.
* **Portabilidade de crédito digital:** Transferência de empréstimos e dívidas para o banco que oferecer a melhor taxa, sem precisar lidar com papeladas ou burocracia física.
* **Pagamentos invisíveis e ágeis:** Iniciar pagamentos, como o Pix, direto de um site de compras ou aplicativo de delivery, sem precisar abrir o app do banco (*Jornada Sem Redirecionamento*).

---

#### 6. Quais são os principais desafios?
* **Fricção para Empresas (PJ):** O processo de consentimento para empresas esbarra em burocracia, especialmente quando a empresa possui múltiplos sócios que precisam assinar eletronicamente a autorização, gerando travamentos e afastando o segmento B2B.
* **Custos e tecnologias legadas:** Os grandes bancos enfrentam o desafio técnico e o altíssimo custo de adaptar sistemas antigos para lidar com bilhões de chamadas de APIs em tempo real, mantendo rigorosos níveis de conformidade regulatória e cibersegurança.
* **Educação financeira e confiança:** Embora grande parte da população já tenha ouvido falar do sistema, ainda há hesitação em compartilhar dados. Converter o conhecimento em uso ativo e demonstrar os benefícios práticos são barreiras persistentes.

---

#### 7. Qual é o futuro do Open Finance?
* **Convergência Sistêmica:** O sistema não atuará sozinho; ele se unirá de forma estrutural ao **Pix** (Pix Automático e por aproximação) e ao **Drex** (a moeda digital tokenizada do Brasil). Isso permitirá *smart contracts* (contratos inteligentes) e "pagamentos agênticos" automáticos.
* **Hiperpersonalização com IA:** Dados abertos alimentarão ferramentas de Inteligência Artificial generativa, fornecendo aos assistentes virtuais o contexto real do cliente em tempo real para renegociar dívidas ou fazer ofertas hiperpersonalizadas (NBO).
* **Open Capital Markets (Mercado de Capitais):** Com a atuação da CVM, a plataforma evoluirá para abraçar os investimentos de forma mais profunda, democratizando o mercado de capitais e simplificando cadastros em corretoras.

---

### 📖 Glossário

| Termo | Definição |
| :--- | :--- |
| **API (Interface de Programação de Aplicativos)** | Tecnologia segura que permite a comunicação e a integração padronizada entre os sistemas de diferentes instituições financeiras, sem centralizar as informações. |
| **Associação Open Finance** | Estrutura de governança gerida por instituições participantes e supervisionada pelo Banco Central, responsável por definir os padrões técnicos, operacionais e de segurança, além de monitorar o ecossistema. |
| **Consentimento** | Autorização prévia, livre, informada e inequívoca do cliente (por meios eletrônicos) para compartilhar seus dados ou iniciar um pagamento. Tem prazo de validade (até 12 meses), finalidade específica e pode ser revogado a qualquer momento. |
| **Drex (Real Digital)** | Representação oficial em formato digital (tokenizado) da moeda soberana brasileira, operando em rede segura que permite a criação de *smart contracts* para automação de transações. |
| **Iniciadora de Transação de Pagamento (ITP)** | Instituição autorizada a comandar uma transferência ou pagamento a pedido do cliente a partir de plataformas de terceiros, sem nunca reter ou deter os fundos transacionados. |
| **Instituição Detentora de Conta** | Instituição financeira ou de pagamento na qual o cliente possui e mantém sua conta (depósito, poupança ou pré-paga) de livre movimentação. |
| **Instituição Receptora de Dados** | Instituição participante que, com a prévia autorização do cliente, solicita e recebe os dados financeiros que estavam armazenados em outro banco. |
| **Instituição Transmissora de Dados** | Instituição onde os dados do cliente estão armazenados originalmente e que realiza o envio seguro dessas informações para a instituição receptora. |
| **Jornada Sem Redirecionamento (JSR)** | Modelo de pagamento que remove atritos na hora da compra, permitindo a conclusão de um pagamento sem que o usuário precise ser redirecionado para o aplicativo do seu banco original. |
| **Open Banking** | Termo original do sistema de compartilhamento de dados do Banco Central, focado inicialmente apenas no escopo de serviços e produtos bancários tradicionais. |
| **Open Finance (Sistema Financeiro Aberto)** | Evolução do Open Banking que abrange todo o mercado financeiro. Permite o compartilhamento de dados, produtos e serviços (investimentos, previdência, seguros e câmbio) sob controle total do cliente. |
| **Pix Automático** | Solução para automatizar pagamentos recorrentes (contas de consumo, assinaturas e mensalidades) sobre a infraestrutura do Pix, reduzindo a dependência do débito automático tradicional. |
| **Portabilidade de Crédito** | Funcionalidade 100% digital impulsionada pelo Open Finance que permite a transferência de dívidas e empréstimos para outra instituição que ofereça taxas de juros mais atrativas. |
| **Smart Contracts (Contratos Inteligentes)** | Regras ou protocolos programáveis (como no ecossistema do Drex) que executam transações automaticamente assim que condições preestabelecidas são cumpridas. |

### 🔄 Prompts reutilizáveis

Estes prompts podem ser copiados e colados no NotebookLM para gerar revisões rápidas:

1. **Revisão para Entrevista Técnica:** 
   > *"Simule uma pergunta de entrevista de emprego sobre os desafios de segurança no Open Finance e elabore uma resposta ideal estruturada em formato STAR (Situação, Tarefa, Ação e Resultado) com base nas fontes."*

2. **Geração de Quadro Comparativo:** 
   > *"Crie uma tabela comparativa com os Impactos do Open Finance para 3 atores: Clientes PF, Grandes Bancos e Startups/Fintechs."*

3. **Análise de Tendências:** 
   > *"Quais são as principais tendências citadas nas fontes sobre a convergência do Open Finance com o Pix e a Inteligência Artificial?"*

## 💡 Aprendizados

Durante o desenvolvimento deste projeto, foi possível aprimorar:

- Conhecimentos sobre Open Finance e seu impacto no sistema financeiro brasileiro;
- Curadoria de fontes confiáveis e organização do conhecimento;
- Engenharia de prompts para obter respostas mais precisas;
- Uso do NotebookLM como ferramenta de aprendizagem ativa;
- Pensamento crítico na análise e validação de respostas geradas por IA;
- Documentação de projetos utilizando Markdown e GitHub.

---

> 💡 **Nota:** este README foi escrito originalmente em português. Caso seu navegador utilize tradução automática, alguns termos técnicos, tabelas ou elementos de formatação podem ser alterados. Para a melhor experiência, recomenda-se visualizar a versão original do repositório.
