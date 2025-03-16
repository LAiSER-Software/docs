## Requirements
- Python version >= Python 3.12. 
- A GPU with atelast 15GB video memory is essential for running this tool on large datasets.

!!! note "NOTE"
   > Google Colab is the preferred mode of execution

## Installation

### i. Install LAiSER package using pip
Installing the package all the dependencies will be installed and downloaded: 
```shell
  pip install laiser
```

### ii. Importing Skill Extractor from LAiSER package
!!! note "NOTE"
    > You need to also intall pandas and torch libraries to handle data and GPU-accelerated computations.
Install the required packages:
```shell
  from laiser.skill_extractor import Skill_Extractor
  import pandas as pd
  import torch
```

**NOTE**: Python 3.9 or later, *preferably 3.12*, is expected to be installed on your system. If you don't have Python installed, you can download it from [here](https://www.python.org/downloads/).
