# 🗄️ Atividades Práticas - Banco de Dados MySQL

Este repositório contém as atividades práticas de Banco de Dados Relacional desenvolvidas durante o bootcamp da **Generation Brasil**.

## 📋 Sobre o Projeto

Conjunto de scripts SQL desenvolvidos para praticar conceitos fundamentais de banco de dados relacionais, incluindo criação de tabelas, relacionamentos, consultas e manipulação de dados.

## 🛠️ Tecnologias Utilizadas

- **MySQL** - Sistema de Gerenciamento de Banco de Dados
- **MySQL Workbench** - Ferramenta para desenvolvimento e administração
- **SQL** - Linguagem de consulta estruturada

## 📂 Estrutura do Repositório

### Atividades Básicas - Tabela Única

- **exe01.sql** - `DB_RH` - Sistema de Recursos Humanos
- **exe02.sql** - `DB_ECOMMERCE` - Sistema de E-commerce
- **exe03.sql** - `DB_ESCOLA` - Sistema de Registro Escolar

### Atividades Avançadas - Relacionamento entre Tabelas

- **exe01.sql** - `DB_GENERATION_GAME_ONLINE` - Sistema de Game Online
- **exe02.sql** - `DB_PIZZARIA_LEGAL` - Sistema de Pizzaria
- **exe03.sql** - `DB_FARMACIA_BEM_ESTAR` - Sistema de Farmácia
- **exe04.sql** - `DB_CIDADE_DAS_CARNES` - Sistema de Açougue
- **exe05.sql** - `DB_CONSTRUINDO_VIDAS` - Sistema de Material de Construção
- **exe06.sql** - `DB_CURSO_DA_MINHA_VIDA` - Sistema de Cursos Online (EAD)

## 🎯 Objetivos de Aprendizagem

### Atividades Básicas (Tabela Única)
- ✅ Criação de banco de dados
- ✅ Criação de tabelas com atributos relevantes
- ✅ Inserção de dados (INSERT)
- ✅ Consultas básicas (SELECT)
- ✅ Filtros com WHERE
- ✅ Atualização de registros (UPDATE)

### Atividades Avançadas (Relacionamentos)
- ✅ Criação de tabelas relacionadas
- ✅ Definição de Chaves Primárias (PRIMARY KEY)
- ✅ Definição de Chaves Estrangeiras (FOREIGN KEY)
- ✅ Consultas com INNER JOIN
- ✅ Operadores BETWEEN e LIKE
- ✅ Filtros em consultas relacionadas

## 📊 Descrição das Atividades

### 📋 Atividades Básicas

#### 👥 Sistema de RH (exe01.sql)
**Banco de Dados:** `DB_RH`

Sistema para gerenciar colaboradores de uma empresa.
- **Tabela:** COLABORADORES
- **Funcionalidades:** Consultas por salário, atualização de dados

#### 🛒 Sistema de E-commerce (exe02.sql)
**Banco de Dados:** `DB_ECOMMERCE`

Sistema para gerenciar produtos de loja virtual.
- **Tabela:** PRODUTOS
- **Funcionalidades:** Consultas por preço, controle de estoque

#### 🎓 Sistema Escolar (exe03.sql)
**Banco de Dados:** `DB_ESCOLA`

Sistema para gerenciar estudantes e notas.
- **Tabela:** ESTUDANTES
- **Funcionalidades:** Consultas por nota, controle de turmas

---

### 🔗 Atividades Avançadas (Relacionamentos)

#### 🎮 Sistema de Game Online (exe01.sql)
**Banco de Dados:** `DB_GENERATION_GAME_ONLINE`

Sistema para gerenciar personagens e classes de um jogo online.
- **Tabelas:** TB_CLASSES, TB_PERSONAGENS
- **Funcionalidades:** Consultas de poder de ataque, poder de defesa, busca por nome

#### 🍕 Sistema de Pizzaria (exe02.sql)
**Banco de Dados:** `DB_PIZZARIA_LEGAL`

Sistema para gerenciar cardápio de pizzaria.
- **Tabelas:** TB_CATEGORIAS, TB_PIZZAS
- **Funcionalidades:** Consultas por valor, categorias (salgada, doce, vegana, premium)

#### 💊 Sistema de Farmácia (exe03.sql)
**Banco de Dados:** `DB_FARMACIA_BEM_ESTAR`

Sistema para gerenciar produtos farmacêuticos.
- **Tabelas:** TB_CATEGORIAS, TB_PRODUTOS
- **Funcionalidades:** Controle de estoque, receita médica, categorias de produtos

#### 🥩 Sistema de Açougue (exe04.sql)
**Banco de Dados:** `DB_CIDADE_DAS_CARNES`

Sistema para gerenciar produtos de açougue.
- **Tabelas:** TB_CATEGORIAS, TB_PRODUTOS
- **Funcionalidades:** Consultas por valor, peso, categorias (bovinos, suínos, aves)

#### 🏗️ Sistema de Material de Construção (exe05.sql)
**Banco de Dados:** `DB_CONSTRUINDO_VIDAS`

Sistema para gerenciar produtos de construção.
- **Tabelas:** TB_CATEGORIAS, TB_PRODUTOS
- **Funcionalidades:** Controle de estoque, categorias (hidráulica, elétrica, acabamento)

#### 📚 Sistema de Cursos Online (exe06.sql)
**Banco de Dados:** `DB_CURSO_DA_MINHA_VIDA`

Sistema para gerenciar cursos EAD.
- **Tabelas:** TB_CATEGORIAS, TB_CURSOS
- **Funcionalidades:** Consultas por valor, carga horária, categorias (programação, design, negócios)

## 🚀 Como Executar

### Pré-requisitos
- MySQL Server instalado
- MySQL Workbench ou qualquer cliente MySQL

### Passos
1. Clone este repositório: 
```bash
(https://github.com/AlexandreJulioDev/MY-SQL.git).
```

2. Abra o MySQL Workbench

3. Abra cada arquivo `.sql` desejado

4. Execute o script completo (Ctrl + Shift + Enter)

5. Visualize os resultados das consultas

## 📝 Exemplos de Consultas

### SELECT Básico
```sql
SELECT * FROM TB_COLABORADORES WHERE SALARIO > 2000;
```

### SELECT com BETWEEN
```sql
SELECT * FROM TB_PRODUTOS WHERE VALOR BETWEEN 50.00 AND 100.00;
```

### SELECT com LIKE
```sql
SELECT * FROM TB_PERSONAGENS WHERE NOME LIKE '%C%';
```

### SELECT com INNER JOIN
```sql
SELECT 
    TB_PIZZAS.NOME,
    TB_PIZZAS.VALOR,
    TB_CATEGORIAS.TIPO AS CATEGORIA
FROM TB_PIZZAS
INNER JOIN TB_CATEGORIAS ON TB_PIZZAS.CATEGORIA_ID = TB_CATEGORIAS.ID;
```

## 🎓 Conceitos Aplicados

- **DDL (Data Definition Language):** CREATE DATABASE, CREATE TABLE
- **DML (Data Manipulation Language):** INSERT, UPDATE, SELECT
- **Constraints:** PRIMARY KEY, FOREIGN KEY, NOT NULL
- **Relacionamentos:** 1:N (Um para Muitos)
- **Operadores:** =, >, <, BETWEEN, LIKE
- **Joins:** INNER JOIN
- **Tipos de Dados:** BIGINT, VARCHAR, DECIMAL, INT, BOOLEAN, DATE

## 👨‍💻 Autor

**ALEXANDRE JULIO**
- GitHub: [@AlexandreJulioDev](https://github.com/AlexandreJulioDev)
- LinkedIn: [Alexandre julio](https://www.linkedin.com/in/alexandre-julio-0b007a211?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais como parte do bootcamp da Generation Brasil.

## 🙏 Agradecimentos

- **Generation Brasil** - Pelo bootcamp e oportunidade de aprendizado
- **Instrutores** - Pela orientação e suporte
- **Colegas de turma** - Pela colaboração e troca de conhecimentos

---

⭐ **Se este repositório foi útil para você, deixe uma estrela!**

📚 **Desenvolvido com dedicação durante o bootcamp Generation Brasil**
