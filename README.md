# CorrSpell

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

4. **clientApp.py:** This file serves as the entry point of the application and includes the Flask web server.

## Testing
To test the spell correction tool locally, follow these steps:

1. Run `clientApp.py`.
2. Access the web server at `http://0.0.0.0:5000/`.
3. Enter a sentence with misspelled words and click "Predict."

## Conclusion
The Spell Corrector project successfully addresses the issue of spelling errors in text. It provides a reliable tool for correcting various types of spelling mistakes, enhancing the overall quality of text content.

## Comparison
While the project achieves its objectives, future enhancements may include the integration of pre-trained language models like BERT or GPT-2 for even higher correction accuracy. Additionally, expanding language support and actively seeking user feedback will contribute to continuous improvement.

## Contributors
- [List of Contributors]

## License
This project is licensed under the [License Name] - see the [LICENSE](LICENSE) file for details.
