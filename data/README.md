# Data

Datasets used in the sessions. One row is one sample in every file.

| File | Rows | What it is | Source |
| --- | --- | --- | --- |
| `iris.csv` | 150 | Iris flowers: 4 measurements and the species. Column names match OpenML dataset 61. | scikit-learn's bundled copy of Fisher's Iris data |
| `bikes.csv` | 17,379 | Hourly bicycle rentals in Washington D.C., 2011 to 2012, with calendar and weather columns. Same layout as OpenML dataset 42712. | UCI Bike Sharing dataset (`hour.csv`), converted: category names instead of codes, temperatures in °C, wind speed rescaled |
| `spam.csv` | 11,512 | Emails with a `label` (spam or ham) and the `text`. 35 rows have no text. | Enron spam data |
| `weather.csv` | 25,218 | Hourly measurements from 8 Swiss weather stations, 2015 to 2017. The course target, the Luzern wind peak 5 hours later, is created in the notebooks with `shift(-5)`. | MeteoSwiss data |
| `mnist_small.csv` | 1,000 | Handwritten digits: 784 pixel columns (0 to 255) and the `class`. A small sample to keep the repository light. | The first 1,000 images of the MNIST test set |

The full MNIST dataset (70,000 images) can be loaded with `fetch_openml("mnist_784", version=1)`.
