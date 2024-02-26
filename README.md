when restarting this database:

type `pip3 list` to check all currently installed packages

install the following packages and remove those not required:
`pip3 install asgiref==3.7.2 dj-database-url==0.5.0 Django==4.2.1 gunicorn==20.1.0 psycopg2==2.9.9 sqlparse==0.4.4`

create an env.py file and add the following:

import os

os.environ.setdefault(
    "DATABASE_URL", "<copy-this-url-from-elephant-sql-details>")