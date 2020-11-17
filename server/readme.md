# Book Api​

Create a dynamic library type application that stores books and allows you to add books. It should have a home page add page and books page. You are able to add a title, author, url, rating, and button to add the book.

## Dependencies

- Python
  - [python](https://www.python.org/)
- Flask
  - [flask-pypi](https://pypi.org/project/Flask/)
  - [flask-docs](https://flask.palletsprojects.com/en/1.1.x/)
- Flask-SQLAlchemy
  - [flask-sqlalchemy-pypi](https://pypi.org/project/Flask-SQLAlchemy/)
  - [flask-sqlalchemy-docs](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
- Flask-Marshmallow
  - [flask-marshmallow-pypi](https://pypi.org/project/flask-marshmallow/)
  - [flask-marshmallow-docs](https://flask-marshmallow.readthedocs.io/)
- Marshmallow-SQLAlchemy
  - [marshmallow-sqlalchemy-pypi](https://pypi.org/project/marshmallow-sqlalchemy/)
  - [marshmallow-sqlalchemy-docs](https://marshmallow-sqlalchemy.readthedocs.io/en/latest/)
- Flask-Bcrypt - [flask-bcrypt-pypi](https://pypi.org/project/Flask-Bcrypt/) - [flask-bcrypt-docs](https://flask-bcrypt.readthedocs.io/)
  ​

## Getting Started

- download zip or clone
- Install all dependencies

  ```
  $ pipenv install
  ```

- Create your sqlite database
  ```
  $ pipenv shell
  $ python
  >>> from app import db
  >>> db.create_all()
  ```
  ​
- Start your flask server
  ```
  $ python app.py
  ```
  ​

## Flask Routes (test in postman or build a front-end)

- Create User
  - METHOD: `POST`
  - URL: http://localhost:5000/api/register
  - BODY: `application/json`
    ```json
    {
      "username": "test",
      "password": "test"
    }
    ```
- Login
  - METHOD: `POST`
  - URL: http://localhost:5000/api/login
  - BODY: `application/json`
    ```json
    {
      "username": "test",
      "password": "test"
    }
    ```
- GET All Users (For test purposes)
  - METHOD: `GET`
