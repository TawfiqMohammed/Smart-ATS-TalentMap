# Smart ATS - TalentMap
![alt text](image.png)

Smart ATS is a resume evaluation tool designed to help job seekers enhance their resumes for better compatibility with Applicant Tracking Systems (ATS). The app compares a resume with a job description, calculates the match percentage, identifies missing keywords, and provides a profile summary to help candidates tailor their resumes for specific job roles.

## Features

- **Job Description Matching**: Calculates a match percentage based on the provided job description and resume content.
- **Keyword Analysis**: Identifies and lists essential keywords missing from the resume.
- **Profile Summary Generation**: Generates a profile summary based on the job description, highlighting the candidate's strengths and areas for improvement.
- **Simple PDF Upload**: Allows easy uploading of a resume in PDF format for analysis.

## Requirements

- Python 3.8+
- Streamlit
- Google Generative AI (Gemini)
- PyPDF2
- dotenv

## Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/smart-ats.git
   cd smart-ats
   ```

2. **Install Dependencies:**

   Install the required Python packages by running:

   ```bash
   pip install -r requirements.txt
   ```

3. **Environment Variables:**

   Create a `.env` file in the project directory and add your Google API key:

   ```plaintext
   GOOGLE_API_KEY=your_google_api_key
   ```

## Usage

1. **Run the Application:**

   Start the Streamlit app by executing:

   ```bash
   streamlit run app.py
   ```

2. **Upload Resume and Job Description:**

   - Paste the job description in the provided text area.
   - Upload your resume in PDF format.
   - Click the "Submit" button to see the match percentage, missing keywords, and profile summary.

## Example Response Format

Each response will be in the following JSON structure:

```json
{
  "JD Match": "85%",
  "MissingKeywords": ["keyword1", "keyword2"],
  "Profile Summary": "Summary of candidate strengths and improvements."
}
```

## Future Enhancements

- Adding support for additional file formats (e.g., .docx).
- Enhanced natural language processing for better keyword extraction.
- Support for multiple AI providers.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.

