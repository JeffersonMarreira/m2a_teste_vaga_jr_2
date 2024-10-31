<h1 align="center">Teste de Programação - Nível Júnior</h1>

<p align="center"><i>Aplicação: Controle de Ponto Eletrônico</i></p>

![Static Badge](https://img.shields.io/badge/python-blue)
![Static Badge](https://img.shields.io/badge/orm-django-3fb950)
![Static Badge](https://img.shields.io/badge/report-PyMuPDF-DAA520)

## Objetivo
Desenvolver um sistema simples de ponto eletrônico que permita registrar e consultar batidas de entrada e saída de funcionários de diferentes empresas. O sistema deve ser construído usando Django e deve incluir funcionalidades básicas, com foco em qualidade de código e boas práticas.

## Requisitos do Sistema

### 1. Modelagem de Dados
- **Model `Empresa`**:
  - Campos: `nome`, `endereco`
  
- **Model `Funcionario`**:
  - Campos: `nome`, `email`, `empresa` (chave estrangeira para o modelo Empresa)

- **Model `Ponto`**:
  - Campos: `funcionario` (chave estrangeira para o modelo Funcionario), `data`, `entrada`, `saida`
  - Métodos para calcular horas trabalhadas.

### 2. Funcionalidades
- **Página Inicial**:
  - Permitir que o usuário selecione uma empresa existente ou cadastre uma nova.
  
- **Gerenciamento de Empresas**:
  - Cadastrar informações de empresas.

- **Gerenciamento de Funcionários**:
  - Cadastrar informações de funcionários associados a uma empresa.
  
- **Registro de Batidas**:
  - Página para registrar batidas de ponto (entrada e saída) para funcionários.
  
- **Consulta de Batidas**:
  - Página para visualizar as batidas registradas, com a possibilidade de filtrar por data.

### 3. Interface de Usuário
- Usar Django Templates para criar as páginas. A aparência deve ser simples e funcional, podendo utilizar CSS básico para melhorar a usabilidade.
- Fornecer feedback ao usuário após ações (como mensagens de sucesso ou erro).

### 4. Autenticação
- Implementar um sistema básico de autenticação para usuários (funcionários), permitindo registro e login.

### 5. Documentação
- Incluir um `README.md` com instruções sobre como configurar o ambiente, instalar dependências e rodar o projeto.
- Documentar funções e classes usando docstrings.
