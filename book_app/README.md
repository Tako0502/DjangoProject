# DjangoProject Backend

## Features
- Django 4.x + Django Rest Framework
- Multi-Tenancy (django-tenants)
- JWT Authentication (djangorestframework-simplejwt)
- OAuth2 & Social Auth (django-allauth)
- Two-Factor Authentication (django-otp)
- PostgreSQL with advanced indexing
- Celery + Redis for async tasks
- WebSockets (Django Channels)
- Elasticsearch for full-text search
- AWS S3 file storage (django-storages)
- Stripe payments
- GraphQL API (Strawberry)
- Monitoring: Prometheus, Sentry
- Dockerized for easy development

## Quickstart

### 1. Clone the repo
```bash
git clone <your-repo-url>
cd DjangoProject/book_app
```

### 2. Set up environment variables
Create a `.env` file with your secrets (see `.env.example`).

### 3. Build and run with Docker Compose
```bash
docker-compose up --build
```

### 4. Run migrations and create superuser
```bash
docker-compose exec web python manage.py migrate
docker-compose exec web python manage.py createsuperuser
```

### 5. Access
- API: http://localhost:8000/api/
- Admin: http://localhost:8000/admin/

## Multi-Tenancy
Uses `django-tenants` for schema-based multi-tenancy. See docs for adding tenants.

## JWT Auth
Uses `djangorestframework-simplejwt` for secure token-based auth.

## Celery & Redis
Async tasks and periodic jobs via Celery. Redis as broker.

## Elasticsearch
Full-text search and autocomplete.

## S3 Storage
Configure AWS credentials in `.env` for file uploads.

## Stripe Payments
Set your Stripe keys in `.env`.

## Monitoring
Prometheus metrics at `/metrics`. Sentry for error logging.

## GraphQL
GraphQL endpoint at `/graphql/`.

---

For more details, see the docs for each package or ask for specific setup help! 