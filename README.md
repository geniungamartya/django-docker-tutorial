# Learn Django

## How to Install Dependencies

1. Create conda environment:

    ```
    conda env create -f environment.yml
    conda activate python39-poetry-env
    ```

2. Create python environment:

    ```
    python -m venv venv
    venv/Scripts/Activate.ps1
    ```

2. Install Depencies using Poetry
    ```
    poetry install
    ```

# Create a project

To create django project:
```
django-admin startproject mysite
```

## Create django app

To create django app:

```
python manage.py startapp polls
```

## How to Define Model

The three-step guide to making model changes:

1. Change your models (in models.py).
2. Run python manage.py makemigrations to create migrations for those changes
3. Run python manage.py migrate to apply those changes to the database.

> A model is the single, definitive source of information about your data. It contains the essential fields and behaviors of the data you’re storing. Django follows the DRY Principle. The goal is to define your data model in one place and automatically derive things from it.

## How to migrate database

To migrate database:

```
python manage.py migrate
```

To make new migration:
```
python manage.py makemigrations polls
```

To see SQL that used to migrate:
```
python manage.py sqlmigrate polls 0001
```

## How to run program

To run program:

```
python manage.py runserver
```