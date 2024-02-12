# Testing
GPT
Sure, here's a README template for your GitHub project that outlines the project's purpose, how to set it up, and how to use it. You can adjust the content as necessary to better fit your project's specifics.

Resume and Job Description Matching Project
This project automates the comparison of skills and experiences between resumes and job descriptions using text extraction from PDF and DOCX files and analysis through OpenAI's GPT-3.5 Turbo. It aims to streamline the process of identifying matching skills and qualifications, enhancing the efficiency of recruitment and job application processes.

Features
Text Extraction: Extracts text from PDF (resumes) and DOCX (job descriptions) files.
Skills Matching: Utilizes OpenAI's GPT-3.5 Turbo model to compare extracted texts and identify matching skills.
Batch Processing: Supports analyzing a single resume against multiple job descriptions stored in a specified directory.
Flexible Document Formats: Handles both PDF and DOCX formats for job descriptions.
Getting Started
Prerequisites
Python 3.8+
Pip for Python package installation
An active OpenAI API key for accessing GPT-3.5 Turbo
Installation
Clone the repository:
bash
Copy code
git clone https://github.com/your-github-username/your-repo-name.git
cd your-repo-name
Install required Python packages:
bash
Copy code
pip install PyMuPDF python-docx openai
Set up your OpenAI API key:
Securely store your OpenAI API key in an environment variable:

bash
Copy code
export OPENAI_API_KEY='your-openai-api-key'
Usage
Place your resume and job descriptions in the specified directories. Update the resume_path and job_descriptions_dir variables in the script to reflect the paths to your files.

Run the script:

bash
Copy code
python main.py
The script will extract text from the resume and each job description, then analyze the content to identify matching skills. Results will be printed to the console.

How It Works
The project uses PyMuPDF and python-docx to extract text from documents.
It then constructs a prompt for the OpenAI API, leveraging the GPT-3.5 Turbo model to identify skills mentioned in both the resume and job descriptions.
Finally, the script outputs a list of matched skills for each job description compared against the resume.
Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any enhancements, bug fixes, or improvements.
