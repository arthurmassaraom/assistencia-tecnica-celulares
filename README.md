# 📱 Assistência Técnica de Celulares



Sistema web full-stack desenvolvido para gestão de clientes, aparelhos e agendamentos de serviços de reparação em uma assistência técnica de dispositivos móveis.



---



## 🛠️ Tecnologias Utilizadas



* **Backend:** Python 3.10+, Flask, `mysql-connector-python`, `bcrypt`

* **Frontend:** HTML5, CSS3, JavaScript (Vanilla ES6+)

* **Banco de Dados:** MySQL 8.0+



---



## ✨ Funcionalidades



* 🔐 **Autenticação e Segurança:** Login seguro com hash de senha via `bcrypt` e gestão de sessão com tempo de expiração automático.

* 👤 **Gestão de Clientes:** Cadastro e pesquisa de clientes com armazenamento criptografado do CPF (`bcrypt`) em conformidade com a LGPD.

* 📱 **Gestão de Aparelhos:** Vinculação de celulares a clientes cadastrados com validação de IMEI (15 dígitos) e descrição de defeitos relatados.

* 📆 **Agendamento de Reparos:** Marcação e reagendamento de serviços técnicos com ordenação cronológica automática por data e hora.



---



## 📁 Estrutura do Projeto



Arthur-Massarao-Marcomini/

├── documentacao.pdf        # Documentação do software (Anexo 1)

├── der.png                 # Diagrama Entidade-Relacionamento

├── assistencia_db.sql      # Script de criação e população do banco de dados

└── sistema/

    ├── app.py              # Ponto de entrada da aplicação Flask

    ├── autenticacao.py     # Regras de login, hash e sessão

    ├── clientes.py         # CRUD e validações de clientes

    ├── aparelhos.py        # CRUD e validações de aparelhos/IMEI

    ├── agendamento.py      # CRUD e regras de agendamento

    ├── rotas.py            # Rotas da API e renderização de páginas

    ├── db.py               # Conexão e execução de queries no MySQL

    ├── requirements.txt    # Dependências do projeto Python

    ├── static/

    │   ├── app.js         # Funções JavaScript utilitárias e rotas de API

    │   └── style.css      # Estilização visual da interface

    └── templates/

        ├── login.html     # Tela de autenticação

        ├── principal.html # Painel inicial

        ├── clientes.html  # Interface de gestão de clientes

        ├── aparelhos.html # Interface de gestão de aparelhos

        └── agendamentos.html # Interface de agendamento de serviços



---
