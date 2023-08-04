# End to End Text-Summarizer-NLP-Project

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py

## Project Description
Project Description
This project demonstrates text summarization using the Hugging Face Pegasus model, a state-of-the-art model for abstractive text summarization. Abstractive summarization generates a concise summary that may contain original sentences not present in the input.

The model is fine-tuned on the SAMSum dataset, which is a dialogue-based dataset for abstractive summarization.

The project provides a FastAPI application that exposes a simple API to summarize text using the Hugging Face Pegasus model.

### Project Structure
- /artifacts: Contains the dataset and data preprocessing and trained machine learning model.
- /src/components: Include all the components like data_ingestion, data_transformation, data_validation, modal_evaluation and modal_trainer.
- /src/pipeline: Predice pipeline steps added
- /config: Contains all the configuration required in project.
- app.py: Includes the Flask web application and API.
- utils.py: Include all the common function used in project.
- requirements.txt: List of dependencies required to run the project.

## Install the required packages:
```
pip install -r requirements.txt
```

## Usage
1. Ensure that the Hugging Face Transformers library is installed:
```
pip install transformers
```
2. Download the SAMSum dataset and place it in the /data directory.
3. Run the FastAPI application:

    - uvicorn app.main:app --host 0.0.0.0 --port 8000

4. Open your web browser and go to http://localhost:8000/docs to access the Swagger UI for the API.
5. Use the /predict endpoint to summarize text by providing the input text in the text parameter.

