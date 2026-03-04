# Imperial College London COMP70016 Coursework

Natural Language Processing Coursework by Henry Yu (tsy22).

## Repository Structure

| File/Directory | Description                                                                                                           |
|:---------------|:----------------------------------------------------------------------------------------------------------------------|
| `BestModel/`   | The final best model with highest F1. `BestModel/BestModel/` contains the model weights, trained by `training.ipynb`. |
| `data/`        | Raw datasets with official train/dev split and hidden test set.                                                       |
| `Experiments/` | Experimental training using different methods (augmentation, oversampling, removing stopwords).                       |
| `eda.ipynb`    | Exploratory data analysis notebook.                                                                                   |
| `dev.txt`      | Predictions of the official dev dataset by the best model.                                                            |
| `test.txt`     | Predictions of the official (hidden) test dataset by the best model.                                                  |

## Setup

I am using PyCharm and `uv` for development. All training is performed on an Apple M4 Pro GPU using PyTorch `mps`
backend. Random seed is set to 42 for reproducibility where possible. To run the notebooks:

```shell
uv sync
jupyter lab
```
