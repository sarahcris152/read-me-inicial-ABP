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

📌 Histórias Selecionadas para a Sprint 1

US01 - Visualizar informações da certificação #1
**Como candidato,**  
Quero visualizar as informações da certificação para entender seu funcionamento antes de acessá-la.
- **Tarefas:**
-A tela inicial deve apresentar uma descrição da certificação.
-Deve apresentar os objetivos da certificação.
-Deve apresentar instruções para realização da avaliação.
-Deve existir uma opção para o usuário prosseguir para o login.
- **Prioridade:** Alta (2)
- **Critérios de Aceite:** A descrição da certificação deve estar detalhada, e deve existir uma opção para o usuário prosseguir para o login;
---

US02 - Realizar login no portal #2
**Como candidato,**  
Quero realizar login utilizando meu CPF e senha para acessar as funcionalidades do portal.
- **Tarefas:**
-O login deve solicitar CPF e senha.
-O sistema deve validar as credenciais informadas.
-O acesso deve ser permitido somente quando CPF e senha forem válidos.
-Em caso de credenciais inválidas, o sistema deve informar que não foi possível realizar o login.
-Após o login realizado com sucesso, o candidato deve ser direcionado ao Menu Principal.
- **Prioridade:** Alta (3)
- **Critérios de Aceite:** O login deve exigir CPF e senha válidos para direcionar o candidato ao Menu Principal, exibindo uma mensagem de erro caso as credenciais estejam incorretas.
---

US03 - Acessar cadastro de candidato #3
**Como candidato,**  
Quero realizar login utilizando meu CPF e senha para acessar as funcionalidades do portal.
- **Tarefas:**
-A tela de login deve possuir uma opção para cadastro.
-Ao selecionar a opção de cadastro, o usuário deve ser direcionado para a tela de cadastro.
-A tela de cadastro deve disponibilizar os campos necessários para criação da conta.
- **Prioridade:** Alta (1)
- **Critérios de Aceite:** A opção de cadastro na tela de login deve redirecionar o candidato para uma nova tela contendo todos os campos necessários para a criação da conta.
---

US04 - Cadastrar candidato #4
**Como candidato,**  
Quero me cadastrar utilizando meus dados pessoais para criar uma conta no portal.
- **Tarefas:**
-O cadastro deve solicitar CPF, nome completo, e-mail e senha.
-O CPF deve ser utilizado como identificador único do candidato.
-O sistema não deve permitir dois candidatos com o mesmo CPF.
-Os campos obrigatórios devem ser validados antes da conclusão do cadastro.
-Após um cadastro válido, o sistema deve informar que a conta foi criada com sucesso.

- **Prioridade:** Alta (5)
- **Critérios de Aceite:** O sistema deve validar os campos obrigatórios e barrar CPFs duplicados, confirmando o sucesso da criação da conta com o CPF como identificador único.
---



---------------------------------------------------------------------CONTINUAR
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
O escopo do banco de dados abrange os 12 primeiros tópicos da Engenharia de Software Ágil:

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

