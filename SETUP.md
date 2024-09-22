
# Setup Instructions for Data Resources

## Overview

In this project, we will be working with two important resources that you need to download and set up:

1. [Healthy Heart PDF](https://www.nhlbi.nih.gov/files/docs/public/heart/healthyheart.pdf) - A public document on maintaining heart health.
2. BioMistral-7B.Q4_K_M.gguf - The open-source large language model that powers the chatbot's responses.

Follow the steps below to download and set up these resources for your project.

---

## 1. Healthy Heart PDF

The Healthy Heart PDF is a document provided by the National Heart, Lung, and Blood Institute (NHLBI), containing essential information on maintaining heart health. It serves as one of the key data sources for answering medical queries.

### Steps to Download:

- Open your terminal or download manager.
- Use the following link to download the PDF directly:

    [Healthy Heart PDF](https://www.nhlbi.nih.gov/files/docs/public/heart/healthyheart.pdf)

- Save it to the designated data folder in your project, such as `/BioMistral_RAG_APP/Data/`.

### Example:

```bash
curl -o /BioMistral_RAG_APP/Data/healthyheart.pdf https://www.nhlbi.nih.gov/files/docs/public/heart/healthyheart.pdf
```

---

## 2. BioMistral-7B.Q4_K_M.gguf Model

The BioMistral-7B.Q4_K_M.gguf is a large biomedical language model that enhances the chatbot's ability to understand and generate accurate medical responses.

### Steps to Download:

- You will need to obtain the BioMistral-7B.Q4_K_M.gguf model file and place it in the appropriate folder, such as `/BioMistral_RAG_APP/Models/`.

> **Note**: The model file can be quite large, so make sure you have sufficient storage space available.

Once downloaded, store it in the model directory:

```
/BioMistral_RAG_APP/Models/BioMistral-7B.Q4_K_M.gguf
```

Ensure that the model file path is correctly configured in your code.

### Example:

```bash
# Move the downloaded model file to the Models directory
mv ~/Downloads/BioMistral-7B.Q4_K_M.gguf /BioMistral_RAG_APP/Models/
```

---

## Summary

Once both the Healthy Heart PDF and BioMistral model are downloaded and set up in the correct directories, you can proceed with running the chatbot system.

Feel free to consult the README.md for further instructions on how to execute the chatbot.

