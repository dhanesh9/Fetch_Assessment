# Fetch_Assessment

This repository contains a multi-task sentence transformer for both sentiment classification and named entity recognition (NER). The model uses pre-trained language models to perform these tasks on sample text, leveraging separate layers for fine-tuning each task. 

## Project Structure

- `Sentence_transformer.ipynb` - The Jupyter Notebook containing the main code for sentiment analysis and NER tasks.
- `requirements.txt` - Lists all Python dependencies needed to run the project.
- `.gitignore` - Specifies files and folders that should be ignored by Git.
- `README.md` - Project documentation.

## Requirements

To install the dependencies, use the following command:

```bash
pip install -r requirements.txt

# Running the Project

### Using Python Environment

1. **Activate Environment**: If you are using a virtual environment, activate it first.

   ```bash
   source env/bin/activate  # For Linux/Mac
   .\env\Scripts\activate   # For Windows

### Using Docker

You can also run the project in a Docker container. The Docker image includes the necessary environment setup for the code.

#### Steps:

1. **Build the Docker Image**:

   ```bash
   docker build -t fetch_assessment .

2. **Run the Docker Container**: 

    ```bash
    docker run -p 8888:8888 fetch_assessment

    Access Jupyter Notebook: Open http://localhost:8888 in your browser, using the token provided in the terminal output.

### Running the Docker Container with Custom Port Mapping
By default, the application runs on port 8888 inside the container. You can map this to any port on your local machine. For example:
docker run -p <host_port>:8888 fetch_assessment


