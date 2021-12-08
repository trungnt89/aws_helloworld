# Docker Build
    docker build -t <image_name> ./ 
    docker-compose up --build

    docker-compose down
    docker-compose up -d
    docker-compose --env-file .env up --build

# Run
    docker run -p 80:80 <images_name>


# Remove
    docker rm -vf $(docker ps -aq);
    docker rmi -f $(docker images -aq);
    docker volume rm $(docker volume ls -q)

# Other
    docker-compose restart 
