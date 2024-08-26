
# Fine-Tuning GPT-2 on Diseases and Symptoms

This project fine-tunes a GPT-2 model on a dataset of diseases and symptoms to generate disease-related information based on symptoms. The dataset used is from Hugging Face's `QuyenAnhDE/Diseases_Symptoms` repository.

## Project Structure

- `symptomChatBot.ipynb`: Contains the main code for loading the dataset, fine-tuning the GPT-2 model, and evaluating the performance.
- `requirements.txt`: Lists all the Python dependencies needed to run the project.
- `README.md`: Documentation and setup instructions for the project.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/yourproject.git
   cd yourproject
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have the required libraries installed:

   ```bash
   pip install datasets transformers torch tqdm pandas
   ```

## Dataset

The dataset used for training is the `QuyenAnhDE/Diseases_Symptoms` dataset from Hugging Face. It contains information on diseases, symptoms, and treatments.

## Model

This project uses the `distilgpt2` model from Hugging Face's Transformers library. The model is fine-tuned using the diseases and symptoms dataset.

## Training

To train the model, run the following command:

```bash
python symptomChatBot.ipynb
```

The script performs the following steps:
- Loads the dataset from Hugging Face.
- Prepares the dataset by converting it into a pandas DataFrame and processing it into the required format.
- Fine-tunes the `distilgpt2` model on the dataset.
- Evaluates the model on a validation set.

## Results

During training, the script logs the training and validation loss for each epoch. These metrics help monitor the model's performance and prevent overfitting.

## Usage

After training, the model can generate disease-related information based on input symptoms. For example, you can use the model to suggest possible diseases based on a list of symptoms.
