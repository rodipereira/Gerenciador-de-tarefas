# Flask-Todolist

[![Licença][license-image]][license-url]  
[![Status de Build][travis-image]][travis-url]

Flask-Todolist é uma aplicação web simples de lista de tarefas, construída com o framework **Flask** em **Python**. A aplicação possui os recursos básicos de autenticação (contas/login), uma API e uma interface de usuário (UI) interativa.

---

### Tecnologias Utilizadas

- **Python (Flask)**: Framework para desenvolvimento web.
- **Docker**: Containerização da aplicação para facilitar o ambiente de desenvolvimento e deploy.

### Dependências

- **Flask-SQLAlchemy**: ORM para interação com banco de dados.
- **Flask-Migrate**: Migrações de banco de dados.
- **Flask-WTF**: Extensão para criação de formulários.
- **Flask-Login**: Gerenciamento de autenticação de usuários.
- **Flask-Testing**: Ferramenta para testes da aplicação.

CSS | [Skeleton](http://getskeleton.com/)  
JS  | [jQuery](https://jquery.com/)

Eu também desenvolvi um aplicativo semelhante usando **Django**:  
https://github.com/rtzll/django-todolist

---

## Explore  
Experimente a aplicação!

### Docker
Com o uso do `docker-compose`, você pode rodar a aplicação facilmente:

```bash
docker-compose build
docker-compose up

A aplicação estará disponível em http://localhost:8000/.

(Ela está rodando com gunicorn, que é utilizado para deploy, ao invés de usar flask run diretamente.)

Manualmente
Se preferir rodar localmente na sua máquina, recomendo o uso do venv.

bash
Copiar código
pip install -r requirements.txt
FLASK_APP=todolist.py flask run
Para adicionar alguns dados de exemplo, rode:

bash
Copiar código
pip install -r test-requirements.txt
flask fill-db
Agora, você pode explorar a API:

http://localhost:5000/api/users

Escolha um usuário, faça login com as credenciais fornecidas. A senha padrão após rodar fill-db é correcthorsebatterystaple.
Dê uma olhada na visão geral de suas listas de tarefas em:
http://localhost:5000/todolists
(Você precisa estar logado para acessar esta página.)

Extensões Utilizadas
Durante o desenvolvimento deste projeto, utilizei algumas extensões para facilitar a criação e manutenção da aplicação:

## Extensões Utilizadas

Durante o desenvolvimento deste projeto, utilizei algumas extensões para facilitar a criação e manutenção da aplicação:

| Uso                  | Extensão Flask  
|----------------------|------------------------  
| Modelo & ORM         | [Flask-SQLAlchemy](http://flask-sqlalchemy.pocoo.org/latest/)  
| Migração             | [Flask-Migrate](http://flask-migrate.readthedocs.io/en/latest/)  
| Formulários          | [Flask-WTF](https://flask-wtf.readthedocs.org/en/latest/)  
| Login                | [Flask-Login](https://flask-login.readthedocs.org/en/latest/)  
| Testes               | [Flask-Testing](https://pythonhosted.org/Flask-Testing/)  

Essas extensões foram suficientes para o escopo do projeto.

Projeto desenvolvido por Rodrigo Pereira de Almeida.