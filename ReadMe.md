### Django, Postgres, PgAdmin, Gunicorn, Nginx

Docker-Compose

    $ docker system prune -a # delete all

    $ docker-compose down -v

    $ docker-compose up -d --build

    $ docker-compose logs -f

    $ docker-compose -f docker-compose.prod.yml down -v

    $ docker-compose -f docker-compose.prod.yml up -d --build

    $ docker-compose -f docker-compose.prod.yml exec web python manage.py migrate --noinput

    $ docker-compose -f docker-compose.prod.yml exec web python manage.py collectstatic --no-input --clear


References:

    https://github.com/khezen/compose-postgres
    
    https://testdriven.io/blog/dockerizing-django-with-postgres-gunicorn-and-nginx/
    
