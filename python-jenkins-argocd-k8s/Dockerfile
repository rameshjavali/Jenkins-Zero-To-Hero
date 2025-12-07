FROM python:3.9-slim

WORKDIR /app

# Install Django directly
RUN pip install django==3.2

# Copy project files
COPY . .

EXPOSE 8000

# Run migrations and start server at container startup
CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
