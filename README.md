# My Data Science Helper Library (ds_helper)

This library is a toolkit designed to automate common data science tasks like column type detection, data visualization, and text cleaning.

## Features
* **Column Type Detection**: Automatically identifies numerical, categorical, and text columns.
* **Auto Visualization**: Generates appropriate plots for each column type.
* **Text Cleaning**: A utility to remove punctuation, stopwords, and filler words.

## Usage Example

```python
import pandas as pd
from ds_helper import clean_text

# Create sample data
sample_data = ["This is a test... like, a GREAT test!", "And another sentence."]
text_series = pd.Series(sample_data)

# Use the library to clean the text
cleaned_series = clean_text(text_series)
print(cleaned_series)
