FROM python:3.11-slim

# Install pg_dump / PostgreSQL client
RUN apt-get update && apt-get install -y postgresql-client

COPY elt_script.py .

# Set env variable for password
ENV PGPASSWORD=secret

CMD ["python", "elt_script.py"]
