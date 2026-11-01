# 📱 BarberApp: Sistema Mobile para Agendamento e Gestão de Barbearia

---

## 👥 Equipa

- **Renan Nunes de Souza**
- **Daniel Francisco de Maria da Fonseca Rincon**
- **Ryan Victor Carvalho de Oliveira**

---

## 🎯 Objetivo

Desenvolvimento de uma aplicação móvel multiplataforma (Android/iOS) utilizando a framework Flutter e a linguagem Dart. A aplicação atuará como a interface front-end mobile, consumindo a API RESTful desenvolvida previamente em Spring Boot, visando automatizar e centralizar os agendamentos e a gestão operacional da barbearia.

---

## 💈 Público-alvo

- **Clientes:** Utilizadores que procuram agendar, acompanhar o histórico e cancelar cortes de cabelo e barba diretamente pelo smartphone, de forma autónoma.
- **Barbeiros:** Profissionais que necessitam de uma ferramenta prática para visualizar a agenda diária e atualizar o estado dos serviços prestados em tempo real.

---

## ⚙️ Requisitos

**Requisitos Funcionais (RF):**

- **RF01:** O utilizador deve realizar o registo e autenticação (login) na aplicação.
- **RF02:** O utilizador deve visualizar a lista de barbeiros e os serviços disponíveis.
- **RF03:** O utilizador deve selecionar datas e horários livres para confirmar um agendamento.
- **RF04:** O utilizador deve consultar o seu histórico de agendamentos e solicitar cancelamentos.
- **RF05:** O barbeiro deve aceder à sua agenda diária e alterar o estado dos atendimentos (ex: pendente, concluído, cancelado).

**Requisitos Não Funcionais (RNF):**

- **RNF01:** A aplicação será construída na framework Flutter (linguagem Dart).
- **RNF02:** A comunicação de dados ocorrerá via requisições HTTP, consumindo os endpoints da API.
- **RNF03:** A interface utilizará componentes nativos do Material Design, implementando navegação intuitiva por separadores (`BottomNavigationBar`).

---

## 📊 Diagramas

**1. Diagrama de Classes (Modelos Front-end no Flutter)**
Reflete o mapeamento dos DTOs recebidos da API no Dart, contemplando a herança de perfis de utilizador e os enumeradores de estado, garantindo a tipagem forte dos dados recebidos.

*(Insira a imagem do seu Diagrama de Classes aqui usando: `![Diagrama de Classes](nome_da_imagem.png)`)*

**2. Diagrama Entidade-Relacionamento (DER)**
Representação da estrutura da base de dados do back-end que sustenta as operações e os relacionamentos consumidos pela aplicação móvel.

*(Insira a imagem do seu Diagrama DER aqui usando: `![Diagrama DER](nome_da_imagem.png)`)*

---

## 🛠️ Organização da equipa para desenvolvimento

A equipa adotará um fluxo de trabalho modularizado no front-end, com as seguintes atribuições para o desenvolvimento em Flutter:

- **Renan Nunes de Souza** — *Estrutura base do projeto, roteamento de navegação, Ecrã de Login/Registo e integração HTTP da Home do Cliente.*
- **Daniel Francisco de Maria da Fonseca Rincon** — *Módulo de Agendamento do Cliente, desenvolvendo a interface de calendário, o ecrã de confirmação de horários e a lógica da listagem de histórico.*
- **Ryan Victor Carvalho de Oliveira** — *Módulo do Barbeiro, desenvolvendo o painel de agenda diária e o ecrã de gestão para alteração do estado de atendimento.*
