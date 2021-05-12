# Data-Purifier-Dataset
Data repository for [Data-Purifier](https://pypi.org/project/data-purifier/) examples

This repository exists only to provide a convenient target for the datapurifier.load_dataset function to download sample datasets from. Its existence makes it easy to document datapurifier without confusing things by spending time loading and munging data. The datasets may change or be removed at any time if they are no longer useful for the datapurifier documentation. Some of the datasets have also been modifed from their canonical sources.

Data is sourced from kaggle 

## Get Started

Install the packages

```bash
pip install data-purifier
```

```bash
python -m spacy download en_core_web_sm
```

Load the module
```python
import datapurifier as dp
from datapurifier import Mleda, Nleda, Nlpurifier

print(dp.__version__)
```

Get the list of the example dataset  
```python
print(dp.get_dataset_names()) # to get all dataset names
print(dp.get_text_dataset_names()) # to get all text dataset names
```

Load an example dataset, pass one of the dataset names from the example list as an argument.
```python
df = dp.load_dataset("womens_clothing_e-commerce_reviews")
```


## Example: 
[Colab Notebook](https://colab.research.google.com/drive/1J932G1uzqxUHCMwk2gtbuMQohYZsze8U?usp=sharing)

Official Documentation: https://cutt.ly/CbFT5Dw

Python Package: https://pypi.org/project/data-purifier/
