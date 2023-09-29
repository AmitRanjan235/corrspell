# CorrSpell
![Frontend](https://github.com/AmitRanjan235/corrspell/blob/7528c5c3cd6f184fe894e67093687dc8035bd971/frontend.png)

## Table of Contents
- [Project Overview](#project-overview)
- [Project Description](#project-description)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Workflow Diagram](#workflow-diagram)
- [Project Structure](#project-structure)
- [Testing](#testing)
- [Conclusion](#conclusion)
- [Comparison](#comparison)
- [Contributors](#contributors)
- [License](#license)

## Project Overview
This project aims to develop a spelling correction tool using deep learning techniques. The tool can identify and correct spelling errors in text, making it valuable for various applications where accurate text is essential.

## Project Description
A word often needs to be checked for spelling correctness, especially in the context of surrounding words. The spell correction tool can detect spelling errors and suggest corrections. It covers various types of errors, including non-word errors, real-word errors, cognitive errors, and short forms/slang/lingo.

## Technology Stack
- Python 3.6
- Keras 2.2.4
- TensorFlow GPU 1.14.0 backend
- CUDA 10 with CuDNN 10

## Installation
To set up the project environment, follow these steps:

**Using Pycharm:**
1. Create a new project.
2. Navigate to the project directory.
3. Create a new virtual environment using conda with Python 3.6.
4. Install the necessary packages from `requirements.txt` using `pip install -r requirements.txt`.

**Using Conda:**
1. Create a new virtual environment using the command: `conda create -n your_env_name python=3.6`
2. Navigate to the project directory.
3. Install the necessary packages from `requirements.txt` using `pip install -r requirements.txt`.

## Workflow Diagram
![Workflow Diagram](https://github.com/AmitRanjan235/corrspell/blob/d06fdb999128f873d5155cade78b449f2b2fb6ba/architecture.drawio.png)


## Project Structure
1. **Project Directory:** This directory contains various project files, including the spell correction logic, Flask server, etc.

2. **requirements.txt:** This file lists the dependencies and package versions used in the project.

3. **spellingcorrector.py:** This file contains the core spell correction logic.

4. **App.py:** This file serves as the entry point of the application and includes the Flask web server.

## Testing
To test the spell correction tool locally, follow these steps:

1. Run `App.py`.
2. Access the web server at `http://0.0.0.0:5000/`.
3. Enter a sentence with misspelled words and click "Predict."

## Deployment on Render
[Your Live Web App](https://spelling-corrector.onrender.com/)

You can easily deploy this Flask application on the Render platform. Follow these steps to get your project up and running:

### Prerequisites

- An account on Render (https://render.com/)
- A GitHub repository with your project code

### Deployment Steps

1. [Sign in to Render](https://render.com/).

2. Create a new web service on Render:
   - Click the "New +" button on your Render dashboard.
   - Select "Web Service" from the options.
   - Choose the GitHub repository where your Flask application is hosted.

3. Configure your deployment settings:
   - Choose the appropriate branch (e.g., "main") to deploy.
   - Set the build command to create a virtual environment, install dependencies, and start your Flask app. For example:
     ```bash
     python -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
     gunicorn -w 4 -b 0.0.0.0:8000 application:app
     ```

4. Define environment variables:
   - If your Flask app relies on environment variables, set them in the Render dashboard under the "Environment" section.

5. Click the "Create Web Service" button to initiate the deployment process.

6. Render will automatically build and deploy your Flask application. You can monitor the deployment progress in the Render dashboard.

7. Once the deployment is successful, you will receive a URL where your application is accessible.

That's it! Your Flask application is now live on Render. You can access it using the provided URL.

### Custom Domain (Optional)

If you have a custom domain, you can configure it in the Render dashboard to point to your deployed application.

For more detailed information and advanced configuration options, refer to the [Render documentation](https://render.com/docs/deploy-flask).


## Conclusion
The Spell Corrector project successfully addresses the issue of spelling errors in text. It provides a reliable tool for correcting various types of spelling mistakes, enhancing the overall quality of text content.

## Comparison
While the project achieves its objectives, future enhancements may include the integration of pre-trained language models like BERT or GPT-2 for even higher correction accuracy. Additionally, expanding language support and actively seeking user feedback will contribute to continuous improvement.

## Contributors
- Amit Ranjan

## License
This project is licensed under the [License Name] - see the [LICENSE](LICENSE) file for details.
