Short URL API with additional feature delete all short URLs

# How to run locally
1. Clone the repository
2. cd into current directory
3. Run the following command, replacing `<your-image-name>` with your desired image name:
    ```bash 
    docker build -t <your-image-name> .
    ```
4. Run the following command, replacing `<your-image-name>` with your desired image name:
    ```bash
    docker run -d -p 8001:80 -v shorturl_data:/app/data <your-image-name>
    ```
5. Open your browser and navigate to `http://localhost:8001/docs` to test the API

# How to run from Docker Hub
1. Run the following command:
    ```bash
    docker run -d -p 8001:80 -v shorturl_data:/app/data kovshichek/shorturl-service:latest
    ```