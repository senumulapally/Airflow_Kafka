# Use an official Kafka image as a base image
FROM confluentinc/cp-kafka:6.2.0

# You might need to add any custom configurations here
# For example, to expose the Kafka port:
EXPOSE 9092

# Copy your Kafka producer/consumer configurations into the container
# COPY config/ /etc/kafka/

# Set environment variables if needed
ENV KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://kafka:9092
ENV KAFKA_ZOOKEEPER_CONNECT=zookeeper:2181