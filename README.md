when restarting this database:

type `pip3 list` to check all currently installed packages

install all the packages listed in the requirements.txt

create an env.py file and add the following:
{
    import os

    os.environ.setdefault(
        "DATABASE_URL", "<copy-this-url-from-elephant-sql-details>")

    os.environ.setdefault(
        "SECRET_KEY", "<your_choice_of_secret_key>")
}

create a fixture folder in the blog app:
    create a posts.json file in the fixtures folder. import data through terminal command : `python3 manage.py loaddata blog/fixtures/posts.json`


