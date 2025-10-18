# 💰 Zen Finance

O **Zen Finance** é um aplicativo financeiro moderno desenvolvido com **React** no frontend e **JAX-RS (Jakarta RESTful Web Services)** no backend.  
Seu objetivo é proporcionar uma maneira **simples, rápida e intuitiva** de **gerenciar receitas, despesas e saldo**, ajudando o usuário a manter o **equilíbrio financeiro** no dia a dia.

---

## 📖 Descrição do Projeto

O **Zen Finance** permite que o usuário:

- Cadastre e categorize **receitas** e **despesas**.
- Visualize o **saldo total** e o **histórico de movimentações**.
- Gere **relatórios mensais** e **gráficos personalizados**.
- Filtre transações por **data, categoria ou tipo (entrada/saída)**.

A aplicação adota uma arquitetura **frontend-backend separada**, onde o React consome os endpoints REST expostos pelo JAX-RS.

---

## 🧩 Tecnologias Utilizadas

### **Frontend**
- ⚛️ [React](https://react.dev/) — Criação de interfaces modernas e reativas.
- 📦 [Axios](https://axios-http.com/) — Comunicação com a API REST.
- 🎨 [Material-UI](https://mui.com/) — Interface limpa e responsiva.
- 📊 [Recharts](https://recharts.org/en-US/) — Exibição de gráficos financeiros interativos.

### **Backend**
- ☕ [Java 17+](https://adoptium.net/) — Linguagem principal da API.
- 🌐 [JAX-RS (Jakarta RESTful Web Services)](https://jakarta.ee/specifications/restful-ws/) — Implementação da API REST.
- 🧱 [WildFly / Payara / TomEE](https://wildfly.org/) — Servidor de aplicação Java EE.
- 🗄️ [JPA / Hibernate](https://hibernate.org/) — Persistência e mapeamento objeto-relacional.
- 🧰 [PostgreSQL / MySQL] — Banco de dados relacional.

---

## ⚙️ Estrutura do Projeto

```
zen-finance/
│
├── backend/
│   ├── src/
│   │   ├── main/java/com/zenfinance/api/...
│   │   ├── main/resources/META-INF/persistence.xml
│   └── pom.xml
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── App.js
│   └── package.json
│
└── README.md
```

---

## 🚀 Como Executar o Projeto

### 🔹 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/zen-finance.git
cd zen-finance
```

---

### 🔹 2. Configurar o Backend (JAX-RS)

1. Abra a pasta `backend/` em sua IDE Java (Eclipse, IntelliJ, VS Code com extensões Java).
2. Configure o **servidor de aplicação** (WildFly, Payara ou TomEE).
3. Atualize o arquivo `persistence.xml` com as credenciais do seu banco de dados.
4. Execute o projeto no servidor.

A API estará disponível em:
```
http://localhost:8080/api/
```

**Exemplos de endpoints:**
- `GET /api/transactions` → Lista todas as transações.
- `POST /api/transactions` → Cadastra uma nova transação.
- `GET /api/balance` → Retorna o saldo total.

---

### 🔹 3. Configurar o Frontend (React)

1. Acesse a pasta `frontend/`:
   ```bash
   cd frontend
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Configure o arquivo `.env` com a URL da API:
   ```
   REACT_APP_API_URL=http://localhost:8080/api
   ```
4. Execute o aplicativo:
   ```bash
   npm start
   ```
5. Acesse o app no navegador:
   ```
   http://localhost:3000
   ```

---

## 🧪 Exemplo de Uso

1. Cadastre uma **receita** (ex: salário, freelas).
2. Adicione algumas **despesas** (ex: aluguel, transporte, alimentação).
3. Acompanhe o **saldo total** e visualize **gráficos mensais** com os gastos por categoria.

---

## 📸 Telas (exemplo)

- 💵 **Dashboard** — Resumo de receitas, despesas e saldo.
- 📈 **Gráficos Financeiros** — Desempenho por período e categoria.
- 🧾 **Histórico de Transações** — Filtro por tipo e data.

---

## 👨‍💻 Contribuição

1. Faça um fork do repositório.
2. Crie uma nova branch:
   ```bash
   git checkout -b feature/minha-feature
   ```
3. Faça suas alterações e commit:
   ```bash
   git commit -m "Adiciona nova funcionalidade"
   ```
4. Envie um pull request.

---

## 📝 Licença

Este projeto está sob a licença **MIT**.  
Sinta-se livre para usar, modificar e distribuir, mantendo os créditos ao autor original.

---

## ✉️ Contato

Desenvolvido por **Gabriel Gonçalves**
🌐 Portfólio: [https://github.com/gabrielgpace](https://github.com/gabrielgpace)
