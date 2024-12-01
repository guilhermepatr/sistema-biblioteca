# 📚 Digital Library Management System

Um sistema de gerenciamento de materiais de biblioteca digital, desenvolvido em **TypeScript**, com ênfase nos conceitos de **Programação Orientada a Objetos (POO)**, como herança, polimorfismo, classes abstratas, interfaces e injeção de dependências.

---

## 🚀 **Funcionalidades**
- Adicionar, buscar, listar e remover materiais (Livros, Revistas e Jornais).
- Visualizar detalhes específicos de cada material.
- Estrutura modular e extensível para novos tipos de materiais.
- Interface de menu interativo em linha de comando.

---

## 🛠️ **Tecnologias e Ferramentas**
- **Linguagem:** TypeScript
- **Paradigma:** Programação Orientada a Objetos (POO)
- **Gerenciamento de Dependências:** npm
- **Estruturação do Projeto:** Arquitetura MVC (Model-View-Controller)
- **Banco de Dados:** Simulado com arrays no momento, pronto para expansão com um banco real (PostgreSQL ou outros).

---

## 🧩 **Conceitos de POO Implementados**
1. **Herança**: Subclasses `Book`, `Magazine` e `News` derivadas da superclasse `Material`.
2. **Polimorfismo**: Métodos sobrescritos como `getDetails()` para diferentes tipos de materiais.
3. **Classes Abstratas**: A classe `Material` define a estrutura base para os tipos de materiais.
4. **Injeção de Dependências**: Controladores (`BookController`, `MagazineController`, etc.) são injetados na tela principal (`PrimaryScreen`).
5. **Sobrecarga de Métodos**: Implementada nos métodos de busca (`searchBooks`, `searchNews`, `searchMagazine`).
6. **Interfaces**: Definição de contratos para as telas e controladores.

---

## 🏗️ **Como Executar**
1. **Clone o repositório:**
git clone https://github.com/seu-usuario/digital-library.git
2. **Instale as dependências:**
npm install
3. **Compile o TypeScript para JavaScript:**
tsc
4. **Execute o projeto:**
node dist/index.js

---

## 📂 **Estrutura do Projeto**
```plaintext
src/
├── controllers/        # Controladores para gerenciar lógica de negócio
│   ├── BookController.ts
│   ├── MagazineController.ts
│   └── NewsController.ts
├── db/                 # Simulação de banco de dados
│   └── Database.ts
├── models/             # Classes que representam os dados
│   ├── Material.ts
│   ├── Book.ts
│   ├── Magazine.ts
│   └── News.ts
├── routers/            # Gerenciamento de rotas
│   └── Router.ts
├── views/              # Interface de interação (menu principal)
│   └── PrimaryScreen.ts
├── utils/              # Funções auxiliares
│   └── Helpers.ts
├── index.ts            # Arquivo principal
└── README.md           # Documentação

