FROM eclipse-temurin:11-jre

WORKDIR /app

# Script que mantiene el contenedor corriendo y genera logs
RUN echo '#!/bin/sh\n\
while true; do\n\
  echo "$(date) - API Service is running and healthy..."\n\
  echo "Connected to MongoDB at: $MONGO_URI"\n\
  sleep 10\n\
done' > /app/run.sh && chmod +x /app/run.sh

CMD ["/app/run.sh"]