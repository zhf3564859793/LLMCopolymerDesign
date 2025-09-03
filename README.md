# LLMCopolymerDesign
<!-- GETTING STARTED -->
## Getting Started

This is the code for **Accelerating Copolymer Discovery: From Automated Literature Mining to de novo Design Using Large Language Models**.

### Prerequisites

The version of python:

  ```sh
  python==3.8.0
  ```

### Installation
1. Clone this repository to your local machine:

   ```sh
   git clone git@github.com:zhf3564859793/LLMCopolymerDesign.git
   ```
2. Navigate to the project directory:

   ```sh
   cd LLMCopolymerDesign
   ```
3. Install the required packages using pip:

   ```sh
   pip install -r requirements.txt

<!-- USAGE EXAMPLES -->
## Usage

## 1. Copolymer Information Extraction

To extract copolymer information from scientific literature, follow these steps:

1. **Download Literature**: Collect 393 PDF files of relevant literature and place them in the `copolymer_pdf` folder.
2. **Convert PDFs to Markdown**: Use the `pdf2markdown_by_textin.ipynb` notebook to convert the PDF files into markdown format for easier processing.
3. **Extract Copolymer Information**: Run the `gpt_extract_copolymer.ipynb` notebook to automatically extract copolymer names and properties from the markdown files using a large language model.
4. **Evaluate Accuracy**: Use the `gpt4o_evaluation_20250820.ipynb` notebook to assess the accuracy of the information extracted by the LLM.

**Extend to Other Tasks**: To apply the pipeline to other information extraction tasks, place the relevant literature PDFs in the `copolymer_pdf` folder and modify the prompts in the respective notebooks as needed.

## 2. Forward Model

The `QSPR_copolymer.ipynb` notebook contains the implementation of a Random Forest model trained on manually annotated data and LLM-extracted data. This model predicts the glass transition temperature ($T_g$) and melting temperature ($T_m$) of copolymers, enabling quantitative structure-property relationship (QSPR) analysis.

## 3. Inverse Model

The `mingpt_copolymer_real_Tg.ipynb`  notebook provides a method to generate copolymers with specified properties, such as a target $T_g$, using a generative model based on the minGPT framework.

