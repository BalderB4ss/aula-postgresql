# 🎓 Sistema de Gerenciamento de Alunos

Aplicação web simples para gerenciar alunos utilizando **Streamlit** como interface e **PostgreSQL** como banco de dados.

## 📋 Funcionalidades

- ➕ Inserir novo aluno
- 📋 Listar alunos cadastrados
- ✏️ Atualizar a idade de um aluno
- 🗑 Deletar um aluno do sistema

---

## 🛠 Tecnologias Utilizadas

- [Python 3.8+](https://www.python.org/)
- [Streamlit](https://streamlit.io/)
- [PostgreSQL](https://www.postgresql.org/)
- [psycopg2](https://www.psycopg.org/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)

---

## 🚀 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
2. Instale as dependências
Utilize um ambiente virtual recomendado (como venv ou virtualenv).

bash
Copiar código
pip install -r requirements.txt
Exemplo de requirements.txt:

txt
Copiar código
streamlit
psycopg2
python-dotenv
3. Configure o arquivo .env
Crie um arquivo .env na raiz do projeto com as credenciais do seu banco de dados PostgreSQL:

env
Copiar código
DB_NAME=seu_banco
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_HOST=localhost
DB_PORT=5432
4. Configure o banco de dados
Certifique-se de ter uma tabela chamada alunos com a seguinte estrutura:

sql
Copiar código
CREATE TABLE alunos (
    id SERIAL PRIMARY KEY,
    nome TEXT NOT NULL,
    idade INTEGER NOT NULL
);
5. Execute a aplicação
bash
Copiar código
streamlit run app.py
📁 Estrutura do Projeto
bash
Copiar código
.
├── app.py                # Interface com Streamlit
├── crud.py               # Funções de CRUD (Create, Read, Update, Delete)
├── db.py                 # Conexão com PostgreSQL
├── .env                  # Variáveis de ambiente (não versionado)
├── requirements.txt      # Bibliotecas necessárias
└── README.md
📸 Interface
A aplicação possui uma interface interativa com menu lateral para:

Inserir alunos com nome e idade

Listar todos os registros do banco

Atualizar a idade de um aluno existente

Deletar um aluno selecionado por ID

⚠️ Requisitos
Python 3.8 ou superior

PostgreSQL instalado e configurado

