# 🚗🐾 Car-Tech - Sistema de Adoção de Animais

API REST desenvolvida em **Node.js** para gerenciar o processo de adoção de animais, permitindo cadastro de animais, tutores, pedidos de adoção, doações e gerenciamento administrativo.

Contrução de API para ser consumida pelo frontend dos profissionais avaliadores da equipe **VENTURUS**!

---

## 📌 Regras do Projeto
Este projeto foi desenvolvido como parte do **Trabalho de Conclusão do 2°DS-AMS em parceria com VENTURUS**.  
As regras definidas foram:

- Tecnologias obrigatórias:
  - **Node.js**
  - **Express.js**
  - **Sequelize**
  - **SQLite** (ou outro banco relacional suportado pelo Sequelize)
- Todas as tabelas devem conter os campos:
  - `createdAt`
  - `updatedAt`
- Foram usadas APIs externas, desde que documentadas.
- Foi criada uma **seed** para inserir usuários administradores.
- As senhas são criptografadas utilizando a lib [`encryptjs`](https://www.npmjs.com/package/encryptjs).

---

## 🎯 Funcionalidades Principais

- Cadastro de **Animais** (com foto em buffer)
- Cadastro de **Tutores** e **Questionário de adoção**
- Listagem de **Animais disponíveis**
- Registro de **Pedidos de Adoção**
- Atualização de dados do Tutor
- Endpoints administrativos para gerenciar animais e adoções
- Autenticação via **login com email e senha**
- Registro de **Doações** (com Pix e QRCode)

---

## 📂 Estrutura das Rotas da API

| Método | Rota                  | Descrição |
|--------|-----------------------|-----------|
| **POST**   | `/animais`            | Cadastro de animal |
| **GET**    | `/animais`            | Listar animais disponíveis |
| **GET**    | `/animais/:id`        | Buscar animal por ID (admin) |
| **POST**   | `/tutores`            | Cadastro de tutor |
| **PATCH**  | `/tutores/:id`        | Atualizar dados do tutor |
| **GET**    | `/tutores/:id`        | Detalhes do tutor + questionário |
| **POST**   | `/questionario`       | Cadastro do questionário |
| **POST**   | `/adocoes`            | Criar pedido de adoção |
| **GET**    | `/admin/animais`      | Listar animais (admin) |
| **PATCH**  | `/admin/animais/:id`  | Atualizar status de animal (admin) |
| **DELETE** | `/admin/animais/:id`  | Deletar animal (admin) |
| **POST**   | `/autenticacao`       | Login |
| **POST**   | `/doacoes`            | Registrar doação |

---

## ⚙️ Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [Sequelize](https://sequelize.org/)
- [SQLite](https://www.sqlite.org/)  
- [encryptjs](https://www.npmjs.com/package/encryptjs)

---

## 👥 Membros
- **Arthur Dombroski** – Estudante  
- **Murilo Firmo** – Estudante  
- **Mateus Pinheiro** – Estudante  

---

## 📫 Contato
Caso queira saber mais sobre nossos projetos:  
👉 [Página da Organização no GitHub](https://github.com/Car-Tech-Venturus)

---