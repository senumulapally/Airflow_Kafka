# Use an official Airflow image as a base image
FROM apache/airflow:2.7.3

# Install any additional dependencies if needed
# For example, to install the PostgreSQL driver:
USER airflow
RUN pip install apache-airflow[postgres]

User root
# Copy your DAGs and other configurations into the container
COPY dags/ /opt/airflow/dags/
# COPY config/ /opt/airflow/config/

# Set environment variables if needed
ENV AIRFLOW__CORE__SQL_ALCHEMY_CONN=postgresql+psycopg2://postgres_user:postgres_pwd@postgres_host:5432/user_db

