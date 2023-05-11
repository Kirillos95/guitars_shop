#####__shop_django_vue__

# Установка django

### 1) Создать виртуальное окружение
    python3 -m venv venv
    source venv/bin/activate

### 2) Установить зависимости

    pip install -r requirements.txt

### 3) Выполнить миграции

    python manage.py migrate    

### 4) Создать суперпользователя

    python manage.py createsuperuser

# Старт

    python manage.py runserver
    
# Установка vue
    npm i
 
    npm run serve
#__________________________________________________#    

My Shop docker run docker:
# Установка: ветка 2; branch 2

    ##
    
    docker-compose build
    docker-compose up 
    open new terminal:
    
    docker-compose run --rm web-app sh -c 'python manage.py makemigrations'
    docker-compose run --rm web-app sh -c 'python manage.py migrate'
    docker-compose run --rm web-app sh -c 'python manage.py createsuperuser'
    
    ##
    vue run docker:
    cd djackets_vue
    docker-compose build
    docker-compose up
