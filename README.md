# LLMCopolymerDesign
<!-- GETTING STARTED -->
## Getting Started

This is the code for [** **].

### Prerequisites

The version of python:

  ```sh
  python==3.9.19
  ```

### Installation

You can use pip to install the required packagess.

  ```sh
  pip install requirements.txt -r
  ```
<!-- USAGE EXAMPLES -->
## Usage

## 1. Copolymer Information Extraction

To extract copolymer information from scientific literature, follow these steps:

1. **Download Literature**: Collect 393 PDF files of relevant literature and place them in the `copolymer_pdf` folder.
2. **Convert PDFs to Markdown**: Use the `pdf2markdown_by_textin.ipynb` notebook to convert the PDF files into markdown format for easier processing.
3. **Extract Copolymer Information**: Run the `gpt_extract_copolymer.ipynb` notebook to automatically extract copolymer names and properties from the markdown files using a large language model.
4. **Evaluate Accuracy**: Use the `gpt4o_evaluation_20250820.ipynb` notebook to assess the accuracy of the information extracted by the LLM.
5. **Extend to Other Tasks**: To apply the pipeline to other information extraction tasks, place the relevant literature PDFs in the `copolymer_pdf` folder and modify the prompts in the respective notebooks as needed.
