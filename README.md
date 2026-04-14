# 💰 Finance API

API REST desenvolvida com **Spring Boot** para gerenciamento de transações financeiras (receitas e despesas).

---

## 🚀 Tecnologias utilizadas

* Java 17
* Spring Boot
* Spring Web
* Spring Data JPA
* H2 Database (banco em memória)
* Maven

---

## 📌 Funcionalidades

* ✅ Criar transação
* ✅ Listar todas as transações
* ✅ Buscar transação por ID
* ✅ Atualizar transação
* ✅ Deletar transação

---

## 📁 Estrutura do projeto

```
src/main/java/com/gabriel/financeapi
│
├── controller   → Camada de API (endpoints)
├── entity       → Modelo da entidade (Transaction)
├── repository   → Acesso ao banco de dados
└── config       → Configurações da aplicação
```

---

## ▶️ Como rodar o projeto

### 1. Clone o repositório

```
git clone https://github.com/SEU-USUARIO/finance-api.git
```

### 2. Acesse a pasta

```
cd finance-api
```

### 3. Execute o projeto

Windows:

```
.\mvnw spring-boot:run
```

Linux/Mac:

```
./mvnw spring-boot:run
```

---

## 🌐 Acesso à API

Após iniciar, a API estará disponível em:

```
http://localhost:8080/transactions
```

---

## 🧪 Exemplos de requisições

### 📌 Criar transação

```
POST /transactions
```

```json
{
  "description": "Salário",
  "amount": 3000.00,
  "type": "INCOME",
  "date": "2026-04-14"
}
```

---

### 📌 Listar todas

```
GET /transactions
```

---

### 📌 Buscar por ID

```
GET /transactions/{id}
```

---

### 📌 Atualizar

```
PUT /transactions/{id}
```

```json
{
  "description": "Salário atualizado",
  "amount": 3500.00,
  "type": "INCOME",
  "date": "2026-04-14"
}
```

---

### 📌 Deletar

```
DELETE /transactions/{id}
```

---

## ⚠️ Observações

* O projeto utiliza **H2 Database**, então os dados são perdidos ao reiniciar a aplicação.
* Ideal para estudos e testes de API REST.

---

## 📈 Próximas melhorias

* 🔹 Integração com PostgreSQL
* 🔹 Validação de dados
* 🔹 Autenticação com JWT
* 🔹 Documentação com Swagger

---

## 👨‍💻 Autor

Desenvolvido por **Gabriel** 🚀
