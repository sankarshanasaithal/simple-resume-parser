# Simple Resume Parser

## Overview

This project is a simple Resume Parser that uses the ChatGroq API to extract key details from resumes such as

- **Name**
- **Email**
- **Phone Number**
- **Technical Skills**
- **Soft Skills**
- **Experience**
- **Total Years of Experience**

By leveraging the ChatGroq API, the parser can efficiently process resumes in various formats (PDF, DOCX, etc.) to capture relevant information, helping recruiters and hiring managers to quickly access essential candidate details


## How It Works

   The parser utilizes the ChatGroq API, which uses Meta Llama 3.0 to extract specific details from resume text. Here’s a high-level workflow

  - **Extract Text**: Uses pdfplumber for PDFs, docx for DOCX files, and pytesseract for image-based text extraction
  - **Call ChatGroq API**: Sends the extracted text to the ChatGroq API with a template prompt to identify and extract relevant details
  - **Save Output**: The extracted information is formatted and saved to a CSV file for easy access and analysis


## Installation and Setup

1. **Clone the Repository**

    Navigate to your respective project repository and execute the following code snippet in the command prompt
  
   ```bash
   git clone https://github.com/username/simple-resume-parser.git
   cd simple-resume-parser
   ```

2. **Install Dependencies**

   Use the `requirements.txt` file to install necessary packages

   ```bash
   pip install -r requirements.txt
   ```
      
3. **Setup Tesseract OCR**

   Follow the installation procedure provided on (https://tesseract-ocr.github.io/tessdoc/Installation.html)

4. **Prepare Resumes**

   Place resume files (in PDF, DOCX, or image formats) in the `sample_resumes` folder

5. **Launch Jupyter Notebook**

   Open the Jupyter Notebook interface by running:

    ```bash
    jupyter notebook
    ```

6. **Run the Notebook**

   Open `resume_parser.ipynb` from the Jupyter interface and run the cells sequentially to execute the resume parsing process

7. **Output**

   The extracted details will be saved in a `.csv` file, capturing each candidate's key information for easy reference


## Contributions

   Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.
