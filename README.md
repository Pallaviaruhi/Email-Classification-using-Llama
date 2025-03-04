# Email Classification using Llama

## Overview

This project builds an email classification system using the **Llama** language model. The system automatically categorizes emails into three categories:

- **Priority**
- **Updates**
- **Promotions**

The model is initialized using a pre-trained Llama model (`model.gguf`), and it processes emails stored in the dataset `data/email_categories_data.csv`. The classification results are tested on the first two emails in the dataset.

## Prerequisites

Before running this project, ensure you have the following installed:

- Python 3.x
- Required Python libraries:
  - `pandas`
  - `llama_cpp`

You can install the dependencies using:

```bash
pip install pandas llama-cpp-python
```

## Dataset

The dataset `data/email_categories_data.csv` contains email content and their expected categories. The classification model uses this dataset to test its accuracy.

## Project Structure

```
📂 Email-Classification-Llama
├── 📂 data
│   └── email_categories_data.csv
├── model.gguf
├── email_classification.py
├── README.md
```

- `data/email_categories_data.csv`: Dataset containing email samples and their expected categories.
- `model.gguf`: Pre-trained Llama model used for classification.
- `email_classification.py`: Main script that loads the model, classifies emails, and prints results.
- `README.md`: Documentation for the project.

## How to Run the Project

1. Ensure the dataset and model file are in the correct locations.
2. Run the script:
   ```bash
   python email_classification.py
   ```
3. The script will:
   - Load the email dataset
   - Initialize the Llama model
   - Classify the first two emails in the dataset
   - Display the classification results

## Expected Output

The script will output the classified categories for the first two emails, for example:

```
Classification Results:
 email 1: Priority
 email 2: Promotions
```

## Contributions

Feel free to contribute to this project by submitting pull requests or reporting issues.


