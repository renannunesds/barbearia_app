# 📱 BarberApp: Sistema Mobile para Agendamento e Gestão de Barbearia

---

## 👥 Equipe

- **Renan Nunes de Souza**
- **Daniel Francisco de Maria da Fonseca Rincon**
- **Ryan Victor Carvalho de Oliveira**

---

## 🎯 Objetivo

Desenvolvimento de um aplicativo móvel multiplataforma (Android/iOS) utilizando a framework Flutter e a linguagem Dart. O aplicativo atuará como a interface front-end mobile, consumindo a API RESTful desenvolvida previamente em Spring Boot, visando automatizar e centralizar os agendamentos e a gestão operacional da barbearia.

---

## 💈 Público-alvo

- **Clientes:** Usuários que buscam agendar, acompanhar o histórico e cancelar cortes de cabelo e barba diretamente pelo smartphone, de forma autônoma.
- **Barbeiros:** Profissionais que necessitam de uma ferramenta prática para visualizar a agenda diária e atualizar o status dos serviços prestados em tempo real.

---

## ⚙️ Requisitos

**Requisitos Funcionais (RF):**

- **RF01 (Usuários):** O aplicativo deve suportar o cadastro segregado entre `Clientes` e `Barbeiros`, compartilhando atributos comuns de acesso para o sistema de login.
- **RF02 (Catálogo):** O aplicativo deve permitir a visualização e gestão do catálogo de `Serviços` (medidos por tempo de duração) e `Produtos` (medidos por quantidade em estoque).
- **RF03 (Agendamentos):** O aplicativo deve permitir a criação de reservas vinculando o Cliente, o Barbeiro e o Serviço escolhido em datas e horários específicos.
- **RF04 (Validação):** O aplicativo deve refletir o bloqueio automático de agendamentos caso o Barbeiro solicitado já possua um atendimento registrado no mesmo dia e horário.
- **RF05 (Financeiro):** O aplicativo deve processar os pagamentos vinculados; ao confirmar um pagamento, o agendamento correspondente deve atualizar automaticamente para o status `CONCLUIDO`.
- **RF06 (Segurança):** O aplicativo deve bloquear qualquer tentativa de processar pagamento para serviços que estejam com o status `CANCELADO`.

**Requisitos Não Funcionais (RNF):**

- **RNF01 (Tecnologia Front-end):** O aplicativo será construído na framework Flutter utilizando a linguagem Dart.
- **RNF02 (Comunicação HTTP):** O aplicativo realizará a comunicação assíncrona com o back-end em Spring Boot através de requisições HTTP enviando e recebendo dados em formato JSON.
- **RNF03 (Interface e UX):** A interface utilizará componentes nativos do Material Design, implementando navegação intuitiva por abas (`BottomNavigationBar`).

---

## 📊 Diagramas

**1. Diagrama de Classes (Modelos Front-end no Flutter)**
Reflete o mapeamento dos DTOs recebidos da API no Dart, contemplando a herança de perfis de usuário e os enumeradores de status, garantindo a tipagem forte dos dados recebidos.

*(Insira a imagem do seu Diagrama de Classes aqui usando: `![Diagrama de Classes](nome_da_imagem.png)`)*

**2. Diagrama Entidade-Relacionamento (DER)**
Representação da estrutura de dados e das entidades de domínio que o aplicativo móvel irá consumir, mapear e gerenciar para o funcionamento das interfaces.

<img width="354" height="1491" alt="Diagrama sem nome drawio (5)" src="https://github.com/user-attachments/assets/532d437c-4114-4825-b825-50a46b367496" />

---

## 🛠️ Organização da equipe para desenvolvimento

A equipe adotará um fluxo de trabalho modularizado no front-end, com as seguintes atribuições para o desenvolvimento em Flutter:

- **Renan Nunes de Souza** — *Estrutura base do projeto, roteamento de navegação, Tela de Login/Cadastro e integração HTTP da Home do Cliente.*
- **Daniel Francisco de Maria da Fonseca Rincon** — *Módulo de Agendamento do Cliente, desenvolvendo a interface de calendário, a tela de confirmação de horários e a lógica da listagem de histórico.*
- **Ryan Victor Carvalho de Oliveira** — *Módulo do Barbeiro, desenvolvendo o painel de agenda diária e a tela de gestão para alteração do status de atendimento.*
