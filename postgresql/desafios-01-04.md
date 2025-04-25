Maravilha! Vamos transformar esses níveis em **desafios práticos**, como se fossem *quests* de um jogo. Cada um testa e reforça o aprendizado do nível anterior. Você pode executar tudo no seu container PostgreSQL via DBeaver e me mandar os resultados ou dúvidas!

---

## 🧩 **Nível 1 – Desafio: A Tabela da Guilda**

### 🧪 Objetivo:
Criar e manipular uma tabela básica de membros da guilda.

### 🔧 Tarefa:
1. Crie a tabela `guerreiros` com os campos:
   - `id`: `SERIAL PRIMARY KEY`
   - `nome`: `VARCHAR(50)`
   - `nivel`: `INTEGER`
2. Insira pelo menos **3 guerreiros** com nomes e níveis diferentes.
3. Liste todos os guerreiros de nível maior que 5, ordenados pelo nome.

---

## 🔗 **Nível 2 – Desafio: A Cidade dos Guerreiros**

### 🧪 Objetivo:
Relacionar guerreiros a cidades com chaves estrangeiras.

### 🔧 Tarefa:
1. Crie a tabela `cidades`:
   - `id`: `SERIAL PRIMARY KEY`
   - `nome`: `VARCHAR(100)`
2. Insira pelo menos **2 cidades**.
3. Crie a tabela `moradias` que liga guerreiros a cidades:
   - `id`: `SERIAL PRIMARY KEY`
   - `guerreiro_id`: `INTEGER` (chave estrangeira para `guerreiros`)
   - `cidade_id`: `INTEGER` (chave estrangeira para `cidades`)
4. Relacione os guerreiros às cidades.
5. Faça uma consulta que traga: nome do guerreiro + nome da cidade.

---

## 📊 **Nível 3 – Desafio: Estatísticas da Guilda**

### 🧪 Objetivo:
Gerar estatísticas dos guerreiros.

### 🔧 Tarefa:
1. Descubra quantos guerreiros existem.
2. Qual a **média de nível** dos guerreiros?
3. Agrupe os guerreiros por cidade e diga **quantos vivem em cada uma**.

---

## ⚙️ **Nível 4 – Desafio: Otimizando a Guilda**

### 🧪 Objetivo:
Criar Views e Indexes.

### 🔧 Tarefa:
1. Crie uma **View** chamada `vw_guerreiros_cidades` que mostre:
   - `nome do guerreiro`, `nível` e `cidade onde mora`.
2. Crie um **índice** no campo `nivel` da tabela `guerreiros`.

---

Esses desafios simulam o uso prático de bancos relacionais em um sistema de RPG.  
