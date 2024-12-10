# Career Assessment and Mentorship Platform - README

## Overview

The **Career Assessment and Mentorship Platform** is an interactive web-based tool designed to help users evaluate their aptitudes, explore career paths, and connect with mentors. The platform enables students to take aptitude tests, view career suggestions, and directly contact mentors via email for personalized guidance.

---

## Features

1. **Aptitude Test**  
   - Evaluate logical reasoning, verbal ability, quantitative skills, and more using a curated set of questions.

2. **Career Suggestions**  
   - Provides tailored career recommendations based on the user's test performance and skills.

3. **Mentorship Connection**  
   - A dedicated mentorship page where students can select mentors and automatically generate an email request for guidance.

4. **Dynamic Web Interface**  
   - User-friendly pages for test-taking, mentorship selection, and career exploration.

5. **Customizable Content**  
   - Easily update question sets, skill mappings, and mentor details.

---

## File Structure

| File/Folder Name          | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| **LICENSE**               | Specifies the license for the repository.                                 |
| **README.md**             | Detailed documentation of the project.                                    |
| **app.py**                | Backend script to process test results and handle mentorship redirection.  |
| **aptitude_questions.csv** | Dataset containing aptitude test questions.                              |
| **aptitude_result.html**  | Template to display aptitude test results.                                |
| **aptitude_test.html**    | Template for users to take the aptitude test.                             |
| **career_template.html**  | Template for exploring career suggestions.                                |
| **index.html**            | Main landing page for the platform.                                       |
| **mentor.html**           | Mentorship page where students can select mentors and request guidance.   |
| **results.html**          | Displays detailed aptitude test results and career suggestions.           |
| **script.js**             | Contains JavaScript for interactive features like email redirection.      |
| **skills.csv**            | Dataset mapping skills to career suggestions.                             |
| **style.css**             | CSS file for styling the web pages.                                       |

---

## Requirements

### Prerequisites
- Python 3.8 or higher
- Libraries (listed in `requirements.txt`, if provided):
  - Flask
  - pandas
  - Jinja2 (integrated with Flask)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/career-mentorship-platform.git
   cd career-mentorship-platform
   ```
2. Install the required Python libraries:
   ```bash
   pip install Flask pandas
   ```

---

## Usage

### Running the Application
1. Start the Flask application:
   ```bash
   python app.py
   ```
2. Open the platform in your browser at `http://127.0.0.1:5000`.

### Navigating the Platform
1. **Aptitude Test**  
   - Navigate to `aptitude_test.html` to take the test and receive career suggestions.
   
2. **Career Suggestions**  
   - Explore recommended career paths on the career page (`career_template.html`).

3. **Mentorship Request**  
   - Visit `mentor.html` to choose a mentor. Clicking on a mentor will redirect to Gmail with a pre-written email template asking for mentorship.

### Mentorship Redirection
The platform uses a `mailto` link to automatically open Gmail with the following template:
```plaintext
Subject: Request for Mentorship

Dear [Mentor's Name],

I hope this message finds you well. I am [Your Name], a student exploring career paths and seeking guidance in [Field/Area]. I would greatly appreciate the opportunity to learn from your expertise and experiences. Kindly let me know if you would be available for mentorship.

Looking forward to your response.

Best regards,  
[Your Name]  
[Your Contact Information]  
```

---

## Customization

### Updating Mentor Information
- Add or edit mentor details (name, email, area of expertise) in `mentor.html`.

### Modifying Email Template
- Update the `mailto` link or JavaScript logic in `mentor.html` or `script.js`.

### Enhancing the Interface
- Use `style.css` to change the design and layout.
- Update `script.js` to add more dynamic interactions.

---

## Sample Input and Output

### Input
- Answers to aptitude test questions.
- Selected mentor for mentorship request.

### Output
- Aptitude test results with career suggestions.
- Redirection to Gmail with a pre-written mentorship email.

---

## License

This project is licensed under [LICENSE](LICENSE). Refer to the file for terms and conditions.

---

## Contributions

Contributions are welcome! Please fork the repository and submit a pull request for feature enhancements, bug fixes, or additional mentorship features.

---

