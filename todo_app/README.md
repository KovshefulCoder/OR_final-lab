TODO API with additional feature delete all todos
# How to run locally
1. Clone the repository
2. cd into current directory
3. Run the following command, replacing `<your-image-name>` with your desired image name:
    ```bash 
    docker build -t <your-image-name> .
    ```
4. Run the following command, replacing `<your-image-name>` with your desired image name:
    ```bash
    docker run -d -p 8000:80 -v todo_data:/app/data <your-image-name>
    ```
5. Open your browser and navigate to `http://localhost:8000/docs` to test the API

# How to run from Docker Hub
1. Run the following command:
    ```bash
    docker run -d -p 8000:80 -v todo_data:/app/data kovshichek/todo-service:latest
    ```