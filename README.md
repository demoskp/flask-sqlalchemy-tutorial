## Populating the database with users
- First open a Flask shell session by running `flask shell` in your terminal
- Import the `db` object by running `from app import db`
- Import the sql script by running `sql = open("users.sql", "r")`
- Get the sql statement by running `statement = sql.read()`
- Import the `text` function from sqlalchemy by running `from sqlalchemy import text`
- Run the sql statement by running `db.session.execute(text(statement))`
- Finally, commit the transaction by running `db.session.commit()`