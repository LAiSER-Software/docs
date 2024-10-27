

As of now LAiSER can be used a command line tool or from the Jupyter notebook(Google Colab). The steps to setup the tool are as follows:

### Google Colab Setup (preferred)
LAiSER's Jupyter notebook is, currently, the fastest way to get started with the tool. You can access the notebook [here](https://github.com/LAiSER-Software/extract-module/blob/main/notebooks/Extract%20Function%20Colab%20Execution.ipynb)

- Once the notebook is imported in google colaboratory, connect to a GPU-accelerated runtime(T4 GPU) and run the cells in the notebook.

### Command Line Setup
To use LAiSER as a command line tool, follow the steps below:

- Navigate to the root directory of the repository and run the command below:

```py
  python main.py
```

> [!CAUTION]
> - If you encounter any `*.dll` file missing errors, make sure you downgrade the pytorch version to `2.2.2`.
```shell
  pip install pytorch=2.2.2
```