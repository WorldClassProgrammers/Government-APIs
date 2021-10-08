# Government APIs

## Installation

Create .env file

```.env
DEBUG=True
SQLALCHEMY_DATABASE_URI=postgresql://<USERNAME>:<PASSEORD>@localhost/government
```

## APIs

- /index
- /registration
  - POST: add a person data to database 'citizen'
    ![alt text](static/images/registration.png)
- /citizen
  - GET: check citizen table
  - DELETE: reset citizen table (delete all rows)

## Basic CMD

```zsh
# install dependencies
> pipenv shell
# install pip to pipFile
> pipenv install <PACKAGE_NAME>

# create requirements.txt
> pip freeze > requirements.txt
```

```zsh
# initial database
> from app import db
> db.create_all()
```
