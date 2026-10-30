<div align="center">

# 📱 SMARTFIX
### Sistema de Gerenciamento de Assistência Técnica de Celulares

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0F172A,100:2563EB&height=180&section=header&text=SMARTFIX&fontSize=50&fontColor=FFFFFF&animation=fadeIn&fontAlignY=40&desc=Tecnologia%20%7C%20Organiza%C3%A7%C3%A3o%20%7C%20Efici%C3%AAncia&descAlignY=65&descSize=16" width="100%" alt="SmartFix - Sistema de Assistência Técnica"/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-2563EB?style=for-the-badge)

</div>

---

## 💻 Sobre o projeto

O **SmartFix** é um sistema desenvolvido para auxiliar no gerenciamento de uma assistência técnica de celulares, permitindo organizar informações de clientes e seus respectivos aparelhos.

O projeto tem como objetivo aplicar conhecimentos de desenvolvimento web, programação com Python e Flask, integração com banco de dados MySQL e criação de funcionalidades para gerenciamento de informações.

A aplicação utiliza como referência o sistema de oficina mecânica disponibilizado no material de apoio da atividade, adaptando sua proposta para o contexto de uma assistência técnica de celulares.

## 🎯 Objetivos

- Desenvolver um sistema funcional para uma assistência técnica.
- Implementar autenticação de usuários.
- Integrar a aplicação com um banco de dados MySQL.
- Consultar e apresentar informações dos clientes.
- Associar os clientes aos seus aparelhos celulares.
- Documentar o sistema e elaborar seu Diagrama Entidade-Relacionamento (DER).

## ⚙️ Funcionalidades do sistema

| Funcionalidade | Descrição |
|:---|:---|
| 🔐 Login | Permite que o usuário acesse o sistema por meio de autenticação. |
| 👤 Identificação do usuário | Retorna o nome do usuário autenticado. |
| 👥 Consulta de clientes | Permite buscar e visualizar os clientes cadastrados. |
| 📱 Associação de aparelhos | Relaciona os aparelhos celulares aos seus respectivos clientes. |
| 🚪 Logout | Permite encerrar a sessão por meio do botão "Sair". |
| 🗄️ Banco de dados | Armazena e organiza as informações utilizadas pela aplicação. |
| 📋 Documentação | Descreve os requisitos e o funcionamento do sistema. |
| 🔗 Diagrama DER | Representa as entidades, os atributos e os relacionamentos do banco de dados. |

> **Observação:** as funcionalidades devem ser implementadas e testadas na aplicação antes de serem consideradas concluídas.

## 🛠️ Tecnologias utilizadas

- **Python:** linguagem de programação utilizada no desenvolvimento.
- **Flask:** framework para criação da aplicação web.
- **MySQL:** sistema de gerenciamento do banco de dados.
- **MySQL Workbench:** ferramenta utilizada para modelagem e elaboração do DER.
- **HTML e CSS:** tecnologias para estruturar e estilizar as páginas, caso utilizadas no projeto.
- **Git e GitHub:** ferramentas para versionamento e compartilhamento do código.

## 🗂️ Estrutura do projeto

A organização pode variar conforme os arquivos disponibilizados no material de apoio. Uma estrutura possível é:

```text
sistema-celulares/
│
├── app.py
├── config.py
├── requirements.txt
├── README.md
│
├── templates/
│   ├── login.html
│   ├── index.html
│   └── clientes.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   └── img/
│
├── database/
│   └── banco.sql
│
└── documentacao/
    ├── documentacao-software.docx
    └── der.png
```

*Importante: os nomes acima são apenas um exemplo. Mantenha os nomes e as pastas existentes no projeto original, adaptando esta estrutura ao código realmente desenvolvido.*

## 🚀 Como executar o projeto

### 1. Pré-requisitos

Antes de iniciar, verifique se você possui:

- Python instalado.
- MySQL Server instalado e em execução.
- MySQL Workbench, para administrar o banco de dados.
- Visual Studio Code ou outro editor de código.
- Os arquivos do projeto extraídos do ZIP.

### 2. Extraia o projeto

Baixe o arquivo ZIP disponibilizado na atividade e extraia seu conteúdo em uma pasta do computador.

Abra a pasta correspondente à versão desenvolvida em Flask no Visual Studio Code.

### 3. Crie o ambiente virtual

No terminal do VS Code, execute:

```bash
python -m venv venv
```

No Windows, ative o ambiente virtual com:

```bash
venv\Scripts\activate
```

### 4. Instale as dependências

Caso exista um arquivo `requirements.txt`, execute:

```bash
pip install -r requirements.txt
```

Se o projeto não possuir esse arquivo, verifique as dependências utilizadas no código antes de instalá-las.

### 5. Configure o banco de dados

Abra o MySQL Workbench, conecte-se ao servidor e execute o script SQL fornecido ou desenvolvido para o projeto.

Confira se o banco de dados foi criado corretamente e se as tabelas necessárias existem.

Configure os dados de conexão da aplicação conforme a estrutura do projeto:

- Host do servidor MySQL.
- Porta de conexão.
- Nome do banco de dados.
- Usuário do banco.
- Senha do banco.

**Atenção:** não compartilhe senhas reais no GitHub. Utilize variáveis de ambiente ou um arquivo de configuração local que não seja enviado ao repositório.

### 6. Execute a aplicação

Se o arquivo principal for `app.py`, execute:

```bash
python app.py
```

Caso o projeto utilize outra configuração de inicialização, siga as instruções correspondentes ao código existente.

Abra no navegador o endereço local indicado pelo Flask no terminal.

### 7. Teste o sistema

Verifique se as principais funcionalidades estão operando corretamente:

- Login com usuário válido.
- Tratamento de credenciais inválidas.
- Exibição do nome do usuário autenticado.
- Busca de clientes cadastrados.
- Associação entre clientes e aparelhos celulares.
- Encerramento da sessão pelo botão "Sair".
- Persistência dos dados no banco de dados.

## 🗄️ Banco de dados e DER

O banco de dados é responsável por armazenar as informações necessárias para o funcionamento do sistema.

O modelo deve representar as entidades identificadas durante a análise dos requisitos, incluindo os usuários, os clientes e os aparelhos celulares, conforme a implementação definida para o projeto.

O **Diagrama Entidade-Relacionamento (DER)** deve apresentar:

- Entidades e seus atributos.
- Chaves primárias (PK).
- Chaves estrangeiras (FK), quando aplicáveis.
- Relacionamentos entre as entidades.
- Cardinalidades dos relacionamentos.

O DER deve ser elaborado no MySQL Workbench e entregue junto com o sistema.

## 📚 Documentação de software

A documentação deve apresentar as informações necessárias para compreender o projeto, incluindo:

- Descrição geral do sistema.
- Objetivos e justificativa.
- Requisitos funcionais e não funcionais.
- Regras de negócio.
- Tecnologias utilizadas.
- Modelagem do banco de dados.
- Diagrama Entidade-Relacionamento.
- Descrição das funcionalidades implementadas.
- Procedimentos de instalação e execução.
- Testes realizados.

## 📦 Entregáveis

Ao finalizar a atividade, devem ser entregues:

- [x] Código-fonte do sistema.
- [x] Documentação de software.
- [x] Diagrama Entidade-Relacionamento (DER).
- [ ] Testes das funcionalidades principais.
- [ ] Verificação da conexão com o banco de dados.

*Os itens marcados como concluídos representam os materiais previstos para entrega, não a confirmação de que já foram implementados ou testados.*

## 🎓 Objetivo acadêmico

Este projeto faz parte de uma atividade prática de desenvolvimento de sistemas, com foco na aplicação dos conceitos de programação web, banco de dados relacionais, autenticação de usuários, consultas e documentação de software.

A proposta é desenvolver uma aplicação organizada, funcional e documentada, colocando em prática os conhecimentos adquiridos durante as aulas.

---

<div align="center">

### 📱 SMARTFIX
**Organizando serviços. Conectando pessoas.**

Desenvolvido como atividade acadêmica de Desenvolvimento de Sistemas.

`Python` • `Flask` • `MySQL`

</div>
