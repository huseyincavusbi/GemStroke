# Gemini Stroke Detection Test

This repository contains a Jupyter notebook (`GemStroke.ipynb`) used to evaluate the vision capabilities of Google's Gemini 2.0 Flash model for binary stroke detection on Non-Contrast Computed Tomography (NCCT) brain scans.

*Note: Attempts to use the `gemini-2.5-pro-exp-03-25` model was often unsuccessful due to consistent security blocks from the API. This evaluation focuses solely on `gemini-2.0-flash`.*

## Dataset

The data used is the **Competition Data Set (Session 1)** from the **STROKE DATA SET, TEKNOFEST 2021**, provided by the Turkish Ministry of Health Open Data Portal:
[https://acikveri.saglik.gov.tr/Home/DataSetDetail/1](https://acikveri.saglik.gov.tr/Home/DataSetDetail/1)

## Objective

The goal of this experiment was to test whether the Gemini 2.0 Flash multimodal model could perform a binary classification task on single NCCT image slices, determining the presence ("1") or absence ("0") of clear visual signs suggestive of stroke based on a specific prompt.

## Results

The notebook evaluates the performance of the `gemini-2.0-flash` model on the validation set. Based on the output provided in the notebook:

*   **Model:** `gemini-2.0-flash`
*   **Accuracy:** Approximately **81.00%** on the 200 valid comparison images.
*   **Evaluation Metrics:** The notebook outputs a detailed confusion matrix and classification report providing precision, recall, and F1-score for both "No Stroke" (0) and "Stroke" (1) classes.

## Disclaimer

This is an experimental evaluation of a general multimodal AI model for a specific medical imaging task. The results and code **are not intended for clinical use or medical diagnosis**. Stroke detection requires specialized medical expertise and validated diagnostic tools. The performance reported here is specific to the dataset, prompt, and model version used.

## License

This project is licensed under the MIT LICENSE - see the [LICENSE](LICENSE) file for details.
