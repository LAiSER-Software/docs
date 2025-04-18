# LAiSER Documentation for developers and end-users

This repository contains the documentation for the LAiSER project. The documentation is written in Markdown and is built using [MkDocs](https://www.mkdocs.org/).


### Contents
LAiSER is a tool that helps learners, educators and employers share trusted and mutually intelligible information about skills​.

- [About](#about)
- [Installation](#installation)
- [Usage](#usage)
- [Funding](#funding)
- [Authors](#authors)
- [Partners](#partners)

## About
LAiSER is an innovative tool that harnesses the power of artificial intelligence to simplify the extraction and analysis of skills. It is designed for learners, educators, and employers who want to gain reliable insights into skill sets, ensuring that the information shared is both trusted and mutually intelligible across various sectors.

By leveraging state-of-the-art AI models, LAiSER automates the process of identifying and classifying skills from diverse data sources. This not only saves time but also enhances accuracy, making it easier for users to discover emerging trends and in-demand skills.

The tool emphasizes standardization and transparency, offering a common framework that bridges the communication gap between different stakeholders. With LAiSER, educators can better align their teaching methods with industry requirements, and employers can more effectively identify the competencies required for their teams. The result is a more efficient and strategic approach to skill development, benefiting the entire ecosystem.

This service uses the ESCO classification of the European Commission.

## Installation

- Install LAiSER using pip:

  ```shell
  pip install laiser
  ```
**NOTE**: Python 3.9 or later, *preferably 3.12*, is expected to be installed on your system. If you don't have Python installed, you can download it from [here](https://www.python.org/downloads/).

## Usage

As of now LAiSER can be used a python package in Google Colab or a local machine with GPU access. The steps to setup the tool are as follows:

### Google Colab Setup (preferred)
LAiSER's Jupyter notebook is, currently, the fastest way to get started with the tool. You can access the notebook [here](https://github.com/LAiSER-Software/extract-module/blob/development/dev_space/Extract%20Function%20Colab%20Execution.ipynb).

- Once the notebook is imported in google colaboratory, connect to a GPU-accelerated runtime(T4 GPU) and run the cells in the notebook.

- Sample code to import and verify laiser module
  ```shell
  from laiser.skill_extractor import Skill_Extractor
  print('\n\nInitializing the Skill Extractor...')
  # Replace 'your_model_id' and 'your_hf_token' with your actual credentials.
  AI_MODEL_ID = "your_model_id"  # e.g., "bert-base-uncased"
  HF_TOKEN = "your_hf_token"
  use_gpu = True  # Change to False if you are not using a GPU
  se = Skill_Extractor(AI_MODEL_ID=AI_MODEL_ID, HF_TOKEN=HF_TOKEN, use_gpu=use_gpu)
  print('The Skill Extractor has been initialized successfully!\n')
  print("LAiSER package loaded successfully!")
  ```
  
**NOTE**: Python 3.9 or later, *preferably 3.12*, is expected to be installed on your system. If you don't have Python installed, you can download it from [here](https://www.python.org/downloads/).


### Command Line Setup
To use LAiSER as a command line tool, follow the steps below:

- Navigate to the root directory of the repository and run the command below:
  ```shell
  python main.py
  ```

> [!CAUTION]
> - If you encounter any `*.dll` file missing errors, make sure you downgrade the pytorch version to `2.2.2`.
```shell
pip install pytorch=2.2.2
```


<!-- ## Examples -->


## Funding
<div align="center">
<img src="https://i.imgur.com/XtgngBz.png" width="100px"/>
<img src="https://i.imgur.com/a2SNYma.jpeg" width="130px"/>
</div>

## Authors
<div align='center'>
<a href="https://github.com/LAiSER-Software/extract-module/graphs/contributors">
        <img src="https://github.com/phanindra-max.png" width="100" height="100" style="object-fit: cover;"/>
        <img src="https://github.com/PrudhvirajuChekuri.png" width="100" height="100" style="object-fit: cover;"/>
        <img src="https://github.com/bharat21999.png" width="100" height="100" style="object-fit: cover;"/>
</a>
</div>


## Partners
<div align="center">
<img src="https://i.imgur.com/hMb5n6T.png" width="120px"/>
<img src="https://i.imgur.com/dxz2Udo.png" width="70px"/>
<img src="https://i.imgur.com/5O1EuFU.png" width="100px"/>
</div>



</br>
<p align='center'> <b> Made with Passion💖, Data Science📊, and a little magic!🪄 </b></p>
