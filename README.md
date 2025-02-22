# GAIA Hugging Face Validation

This project presents a web-based application that validates test cases from the **GAIA Dataset** using OpenAI’s language models (LLM). Users can interactively select test cases, send them to OpenAI, and compare the AI-generated responses with predefined answers. If OpenAI’s response doesn’t match the expected outcome, users are given the flexibility to modify the validation steps and re-submit the question for another validation attempt.


## Project Resources:

- **Google Codelabs** [Codelabs Link](https://codelabs-preview.appspot.com/?file_id=1mjSKMWLaBjHpahLFToNlpkTMapciBedKwfLZGAjF07A#0)
- **App (Streamlit Cloud)**: [Streamlit Link](https://gaia-openai-validation-apmepvhff4kwcxfy687eqr.streamlit.app/)

# Technologies

![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![AWS](https://img.shields.io/badge/Amazon%20AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=for-the-badge&logo=pandas)
![S3](https://img.shields.io/badge/-AWS_S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)
![RDS](https://img.shields.io/badge/AWS_RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white)
![Hugging Face](https://img.shields.io/badge/-HuggingFace-FFD54F?style=for-the-badge&logo=huggingface&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

## Architecture Diagram

![flow_diagram](https://github.com/aniket-afk/GAIA-Huggingface-Validation/blob/main/Architecture/streamlit_workflow_architecture.png)

## How to Run the Application

### Prerequisites
- Install [Poetry](https://python-poetry.org/) for dependency management.
- Ensure you have a `.env` file with the following environment variables:

  ```bash
  AWS_ACCESS_KEY_ID=<your-access-key-id>
  AWS_SECRET_ACCESS_KEY=<your-secret-access-key>
  POSTGRES_HOST=<your-rds-host>
  POSTGRES_DB=<your-database>
  POSTGRES_USER=<your-username>
  POSTGRES_PASSWORD=<your-password>
  OPENAI_API_KEY=<your-openai-api-key>
  ```

### Setup and Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/RAG_Model_Eval.git
   cd RAG_Model_Eval
   ```

2. **Install dependencies:**
   ```bash
   poetry install
   ```

3. **Run the Streamlit App:**
   ```bash
   streamlit run Streamlit_app/app.py
   ```

### Usage
1. Launch the app and log in using the required credentials.
2. Choose a test case from the dropdown menu.
3. If a file is associated with the test case, it will be fetched from S3 and processed.
4. Review the ChatGPT-generated response and validate the results.

## Contributing
1. Fork the project.
2. Create a feature branch.
3. Submit a pull request for review.

## License
This project is licensed under the MIT License - see the `LICENSE.md` file for details.

## Contact

For Any questions or support, please contact [Aniket Patole](mailto:aniketpatole6@gmail.com).

