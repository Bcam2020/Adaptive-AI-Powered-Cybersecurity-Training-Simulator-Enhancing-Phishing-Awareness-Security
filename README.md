# Adaptive AI-Powered Phishing Training Simulator


## Overview

The **Adaptive AI-Powered Phishing Training Simulator** is a cross-platform application designed to help users learn how to identify phishing emails. The system leverages a combination of deep learning and adaptive difficulty adjustments to simulate realistic phishing scenarios and improve user awareness. It includes features for generating AI-based phishing and legitimate emails, tracking user performance, and providing educational feedback.

This project is open source and available on GitHub. It consists of multiple modules for model management, email generation, user management, statistical analysis, and ethical guidelines.

## Features

- **Adaptive Training:**  
  Adjusts the difficulty level based on your performance.
  
- **AI-Based Email Generation:**  
  Generates both phishing and legitimate emails using trained LSTM models.
  
- **User Authentication and Profile Management:**  
  Secure registration and login with bcrypt password hashing.
  
- **Performance Analytics:**  
  Tracks metrics such as response time, accuracy, and overall performance.
  
- **Ethical Considerations:**  
  Incorporates an ethical consent process and provides educational feedback.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Docker Setup](#docker-setup)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Installation

### Requirements

- **Python 3.7 or later**
- **TensorFlow** (compatible with your hardware)
- **Other Python Dependencies:** Listed in `requirements.txt`
- **Git LFS:** If you wish to work with large files tracked in the repository
- **(Optional) Docker:** For containerized deployment

### Steps to Install Locally

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Set Up a Virtual Environment (Recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use: venv\Scripts\activate
    ```

3. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Download Required Assets:**

   - If your project uses Git LFS, ensure that Git LFS is installed and initialized:
  
     ```bash
     git lfs install
     ```
  
   - Alternatively, download large assets from the [GitHub Release](https://github.com/yourusername/your-repo-name/releases) page.

5. **Configure the Application:**

    - Edit the `config.py` file as needed. This file contains paths, model parameters, and various constants.
    
    - Ensure that you have a dataset CSV file as specified by `CONFIG['DATASET_FILE']`.

## Usage

After installation, you can run the simulator by executing the main entry point:

#bash
python main.py
Upon startup, you will be prompted to either register or login. The simulator then guides you through a series of training rounds where you are shown emails and asked to identify phishing attempts. The system adapts the difficulty level based on your accuracy and response time.

Additional Options
Advanced Settings:
Access performance reports, export data, reset statistics, or adjust the difficulty manually.

Ethical Consent:
Users must provide ethical consent before proceeding with training sessions.

## Docker Setup
If you prefer a containerized environment, follow these steps:

Build the Docker Image:

bash
Copy
docker build -t phishing-trainer .
Run the Container:

bash
Copy
docker run -it --rm -p 8080:8080 phishing-trainer
Users on Windows, macOS, or Linux can run Docker to avoid local dependency issues.

## License
This project is licensed under the MIT License. Feel free to use, modify, and distribute the project as specified by the license.

## Contributing
Contributions are welcome! If you encounter any issues or have ideas for improvements:

Fork this repository.

Create a new branch for your feature or fix.

Commit your changes and open a pull request.

Ensure that your code adheres to the project’s style guidelines and includes appropriate tests and documentation.

## Contact
For any questions or further assistance, please contact:

Name: Your Name

Email: your.email@example.com

GitHub: @yourusername

