🎯 Portal de Certificação em Metodologias Ágeis

Projeto em andamento do primeiro semestre do curso em Desenvolvimento de Software Multiplataforma da FATEC-Jacareí, focado no desenvolvimento de um Portal de Certificação em Metodologias
Ágeis

[Logo da Equipe/Projeto]

## [Bit or Byte]

| Desafio | Solução | Backlog do Produto | DoR | DoD | Cronograma de Sprints | Tecnologias | Manual de Instalação | Equipe |

Status do Projeto: Sprint 1 em andamento
Relatório de Testes: [Link/Formato] 
Pasta de Documentação: [Link] 
Video do Projeto: [Link] 

## 🏅 Desafio
É comum que os estudantes tenham dificuldade em fixar conceitos teóricos de metodologias ágeis (como o Scrum) e aplicá-los em cenários reais de desenvolvimento. O sistema proposto visa resolver essa lacuna oferecendo uma trilha de simulados randômicos cronometrados e uma Área de Estudos integrada, validando o conhecimento através de um certificado eletrônico autêntico.

---

## 🔄 Sprint 1 – Fundações, Infraestrutura e Base de Dados

### 📅 Período
- **Início:** 28/09/2026
- **Término:** 22/10/2026

### 🎯 Objetivos Principais
- Estruturar a modelagem inicial e os contêineres Docker do ambiente de desenvolvimento.
- Criar e popular o banco de dados com as questões dos primeiros tópicos de agilidade.
- Desenvolver os protótipos de interface gráfica e telas estáticas do front-end.



| Item | História / Descrição | Prioridade | Critérios de Aceite |
| --- | --- | --- | --- |
| **US01** | **Visualizar informações da certificação**<br>

<br>*Como candidato, quero visualizar as informações da certificação para entender seu funcionamento antes de acessá-la.* | Alta (2) | A descrição da certificação deve estar detalhada, e deve existir uma opção para o usuário prosseguir para o login; |
| **US02** | **Realizar login no portal**<br>

<br>*Como candidato, quero realizar login utilizando meu CPF e senha para acessar as funcionalidades do portal.* | Alta (3) | O login deve exigir CPF e senha válidos para direcionar o candidato ao Menu Principal, exibindo uma mensagem de erro caso as credenciais estejam incorretas. |
| **US03** | **Acessar cadastro de candidato**<br>

<br>*Como candidato, quero realizar login utilizando meu CPF e senha para acessar as funcionalidades do portal.* | Alta (1) | A opção de cadastro na tela de login deve redirecionar o candidato para uma nova tela contendo todos os campos necessários para a criação da conta. |
| **US04** | **Cadastrar candidato**<br>

<br>*Como candidato, quero me cadastrar utilizando meus dados pessoais para criar uma conta no portal.* | Alta (5) | O sistema deve validar os campos obrigatórios e barrar CPFs duplicados, confirmando o sucesso da criação da conta com o CPF como identificador único. |
| **US05** | **Escolher ação após concluir o cadastro**<br>

<br>*Como candidato, quero escolher entre iniciar a certificação ou acessar o menu principal para decidir como prosseguir no portal.* | Alta (2) | O sistema deve exibir uma mensagem de sucesso e oferecer a escolha entre iniciar a certificação — redirecionando para a Página de Exames — ou não iniciá-la naquele momento, direcionando o candidato para o Menu Principal. |
| **US06** | **Acessar o Menu Principal**<br>

<br>*Como candidato, quero acessar um menu principal para navegar pelas funcionalidades disponíveis no portal.* | Alta (2) | Após o login, o Menu Principal deve exibir as opções de acesso à Página de Exames, Área de Estudos, Histórico, Certificados e a funcionalidade para encerrar a sessão. |
| **US07** | **Navegar entre as áreas do portal**<br>

<br>*Como candidato, quero selecionar uma funcionalidade no menu para acessar a área desejada do portal.* | Alta (2) | Como candidato autenticado, ao selecionar uma opção no menu, o sistema deve direcioná-lo para a Página de Exames, Área de Estudos, Histórico ou Certificados, permitindo que ele retorne ao Menu Principal a partir de qualquer uma dessas áreas internas. |
| **US08** | **Visualizar temas da Área de Estudos**<br>

<br>*Como candidato, quero visualizar os temas disponíveis na Área de Estudos para escolher o conteúdo que desejo estudar.* | Alta (2) | A Área de Estudos deve apresentar de forma organizada os 12 temas da certificação, permitindo que o candidato selecione individualmente qualquer um deles para ser direcionado ao respectivo conteúdo. |
| **US09** | **Acessar conteúdo de estudo de um tema**<br>

<br>*Como candidato, quero acessar o material de estudo de um tema para me preparar para a certificação.* | Alta (3) | Ao selecionar um tema na lista, o sistema deve exibir um material didático coerente, enriquecido com imagens e recursos de aprendizagem, permitindo que o candidato retorne à lista de temas a qualquer momento. |
| **US10** | **Navegar entre os conteúdos de estudo**<br>

<br>*Como candidato, quero navegar entre os diferentes temas da Área de Estudos para consultar os conteúdos disponíveis.* | Alta (2) | O candidato deve conseguir navegar livremente entre os 12 temas de estudo sem iniciar uma certificação, podendo alternar entre eles, retornar à lista de temas ou voltar ao Menu Principal a qualquer momento. |
| **US36** | **Implementar banco de dados PostgreSQL**<br>

<br>*Como equipe de desenvolvimento, queremos persistir os dados do portal em PostgreSQL para atender à arquitetura definida para o projeto.* | Alta (8) | O banco de dados PostgreSQL deve ser estruturado com comandos DDL com base nos modelos conceitual e lógico para armazenar dados de usuários, temas, questões, imagens, alternativas, respostas, certificados e histórico, permitindo sua manipulação por comandos DML. |
| **US37** | **Implementar arquitetura Web da aplicação**<br>

<br>*Como equipe de desenvolvimento, queremos implementar a comunicação entre front-end, back-end e banco de dados para permitir o funcionamento integrado do portal.* | Alta (8) | O sistema deve integrar o front-end em HTML, CSS e JavaScript puro com o back-end para gerenciar a comunicação com o banco de dados, garantindo a validação de regras sensíveis no servidor e um tempo de resposta adequado. |

## 📋 Requisitos e Cobertura do Projeto

### Requisitos Funcionais (RF) Contemplados
- **RF01:** Apresentação da tela inicial com objetivos e instruções do simulado.
- **RF03 / RF04:** Cadastro e autenticação exclusiva por meio de CPF e senha criptografada.
- **RF06:** Sorteio randômico de 1 questão a partir de um banco fixo de 4 itens por tema.
- **RF10 / RF11:** Cronômetro dinâmico de 150 segundos com encerramento automático por timeout.
- **RF17 / RF19:** Emissão e validação pública de certificados digitais por QR Code.
- **RF20:** Gravação em tempo real do histórico completo de respostas e horários das tentativas.

### Requisitos Não Funcionais (RNF) & Restrições (RP)
- **RNF01:** Interface responsiva adaptada para dispositivos móveis (Mobile Friendly).
- **RNF04:** Proteção do Back-end contra manipulações indevidas de notas via console do Front-end.
- **RP01:** Interface construída de forma nativa com HTML5, CSS3 e JavaScript (Vanilla ES6), sem frameworks.
- **RP02:** Persistência relacional utilizando banco de dados PostgreSQL estruturado.
- **RP05:** Orquestração completa de microsserviços isolados através de Docker Compose.

---

## 📚 Conteúdo Programático (12 Temas da Certificação)
O escopo do banco de dados abrange os 12 seguintes tópicos da Engenharia de Software Ágil:

1. **Fundamentos da Agilidade:** Crise do software, desenvolvimento tradicional cascata × ágil.
2. **Manifesto Ágil:** Os 4 valores fundamentais e os 12 princípios norteadores.
3. **Introdução ao Scrum:** Pilares do empirismo, transparência, inspeção e adaptação.
4. **Papéis do Scrum:** Product Owner, Scrum Master e time de Developers.
5. **Eventos do Scrum:** Sprint, Sprint Planning, Daily, Sprint Review e Sprint Retrospective.
6. **Artefatos do Scrum:** Product/Sprint Backlog, Incremento, Sprint Goal e Definition of Done.
7. **User Stories:** Critérios de aceitação e aplicação prática do modelo "Como... Quero... Para...".
8. **Gestão do Product Backlog:** Priorização, técnicas de refinamento e evolução contínua.
9. **Kanban:** Fluxo contínuo de trabalho, cartões, gerenciamento de gargalos e limites de WIP.
10. **Planejamento Ágil:** Estimativas com Story Points, dinâmica de Planning Poker e Release Roadmaps.
11. **Métricas Ágeis:** Gráficos de Burndown, Burnup, métricas de Velocity, Lead Time e Cycle Time.
12. **Qualidade em Projetos Ágeis:** Critérios de Pronto (DoD), testes e Integração Contínua (CI).

---

## 💻 Tecnologias e Badges
![HTML5](https://shields.io)
![CSS3](https://shields.io)
![JavaScript](https://shields.io)
![PostgreSQL](https://shields.io)
![Docker](https://shields.io)
![Figma](https://shields.io)

---

## 🎨 Design System & UX
- **Tipografia:** Uso de fontes sans-serif corporativas limpas (`Arial`, `Helvetica`) com foco em legibilidade de avaliações.
- **Diferenciais de UX:** 
  - Bloqueio preventivo de navegação pelas abas do simulado para coibir evasão e fraudes na prova.
  - Tooltips flutuantes explicativos na Área de Estudos e skeletons durante a requisição de imagens pesadas das questões.

---

## 📋 Diagramas e Modelagem

### 📊 Modelo Lógico de Dados (PostgreSQL)
```text
  [USUARIOS] 1 ─────── N [HISTORICO_AVALIACOES]
                                │ N
                                │
                                1
    [TEMAS] 1 ─────── N [QUESTOES] 1 ─────── N [ALTERNATIVAS]
```

---

## 🧰 Manual de Instalação e Execução

### 🛠️ Pré-requisitos
- Ter o [Git](https://git-scm.com) instalado.
Use o código com cuidado.
• Ter o Docker Desktop rodando localmente na máquina.
1. Clonar o Repositório Principal
bash git clone https://github.com cd Portal-Certificacao-Agiles 
2. Executar via Docker Compose
Para subir os contêineres independentes do banco PostgreSQL, do back-end Node.js e do servidor front-end integrados:
bash docker-compose up -d --build 
Após o build concluído, a aplicação estará disponível localmente em seu navegador no endereço: http://localhost:3000.
👥 Nossa Equipe
Membro	Função / Papel Scrum	GitHub	LinkedIn
Matheus Oliveira Dantas de Souza	Product Owner		
Sarah Cristiny de Souza Mendes	Scrum Master		
João Vitor Maximiano de Carvalho	Desenvolvedor Core		
Luiz Felipe Nogueira	Desenvolvedor Banco		
Nikolas Gabriel Alves de Araujo	Desenvolvedor Front		
Pedro Lucas Matias	Desenvolvedor Back		
Ryan Cesar Candido Alves	Desenvolvedor Back		
Willian de Paula Barreto	Desenvolvedor Front		
👨‍🏫 Coordenação e Orientação
• Prof. Marcelo Augusto Sudo (Focal Point do Semestre)
Faculdade de Tecnologia Professor Francisco de Moura (FATEC Jacareí) — Curso de DSM (1º Semestre / 2026-2)

***

<FollowUp>
Se você quiser, posso ajudar com os próximos passos:
* Escrever o script SQL com a **criação de tabelas (DDL)** baseada na modelagem acima.
* Desenvolver os códigos de **configuração do Docker Compose** para rodar o banco e a API.

Diga-me qual item você gostaria de adiantar agora!
</FollowUp>


## 🏅 Solução
[Descrição detalhada de como a aplicação resolve o desafio proposto]

## 📋 Backlog do Produto

| Rank | Prioridade | User Story | Story Points | Sprint | Requisito do Cliente | Status |
| :--- | :--------- | :--------- | :----------- | :----- | :------------------- | :----- |
| 1    | [Grau]     | Como...    | [Pontos]     | [Nº]   | [Código]             | [Ícone]|

## 🏃 DoR - Definition of Ready
- [Item de critério de prontidão 1]
- [Item de critério de prontidão 2]

## 🏆 DoD - Definition of Done
- [Item de critério de conclusão 1]
- [Item de critério de conclusão 2]

## 📅 Cronograma de Sprints

| Sprint | Período | Documentação |
| :----- | :------ | :----------- |
| 🔖 **SPRINT 1** | 28/09/26 - 22/10/26 | [Link Docs] |
| 🔖 **SPRINT 2** | 23/10/26 - 05/11/26 | [Link Docs] |
| 🔖 **SPRINT 3** | 06/11/26 - 25/11/26 | [Link Docs] |



## 💻 Tecnologias
![GitHub](https://shields.io)
![VS Code](https://shields.io)
![Figma](https://shields.io)

## 📖 Manual de Instalação

### 🛠 Pré-requisitos
- [Requisito 1]
- [Requisito 2]

### 1. Clonar o Repositório Principal
```bash
[Comandos de clone]
```

### 2. Configuração do Backend
1° [Passo de ambiente]
2° [Passo de banco de dados]

**Opção A: [Método de Instalação 1]**
```bash
[Comandos]
```

**Opção B: [Método de Instalação 2]**
```bash
[Comandos]
```

**Saída Esperada:**
[Endereço local e informações de sucesso do Backend]

### 3. Configuração do Frontend
```bash
[Comandos de instalação e execução]
```

**Saída Esperada:**
[Endereço local e informações de sucesso do Frontend]

## 🎓 Equipe

| Membro | Função | Github | Linkedin |
| :----- | :----- | :----- | :------- |
| Matheus Oliveira Dantas de Souza | Product Owner | [Link] | [Link]   |
| Sarah Cristiny de Souza Mendes | Scrum Master | [Link] | [Link]   |
| João Vitor Maximiano de Carvalho | Desenvolvedor | [Link] | [Link]   |
| Luiz Felipe Nogueira | Desenvolvedor | [Link] | [Link]   |
| Nikolas Gabriel Alves de Araujo | Desenvolvedor | [Link] | [Link]   |
| Pedro Lucas Matias | Desenvolvedor | [Link] | [Link]   |
| Ryan Cesar Candido Alves  | Desenvolvedor | [Link] | [Link]   |
| Willian de Paula Barreto | Desenvolvedor | [Link] | [Link]   |

