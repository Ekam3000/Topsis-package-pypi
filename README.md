## TOPSIS Package discription

TOPSIS stands for Technique for Oder Preference by Similarity to Ideal Solution. It is a method of compensatory aggregation that compares a set of alternatives by identifying weights for each criterion, normalising scores for each criterion and calculating the geometric distance between each alternative and the ideal alternative, which is the best score in each criterion. An assumption of TOPSIS is that the criteria are monotonically increasing or decreasing. In this Python package Vector Normalization has been implemented.

This package has been created based on class assignment of course UCS654. Ekam COE-7 102003322

## In Command Prompt

> 102003322.py 102003322-data.csv "1,1,1,2" "+,+,-,+" 102003322-result.csv

## Installation

You can install this package using following command
pip install Topsis-Ekam-102003333

## Example

#### sample.csv

A csv file showing data for different mobile handsets having varying features.

| Model | Storage space(in gb) | Camera(in MP) | Price(in $) | Looks(out of 5) |
| :---: | :------------------: | :-----------: | :---------: | :-------------: |
| Model |     Correlation      |      R2       |    RMSE     |    Accuracy     |
|  ---  |         ---          |      ---      |     ---     |       ---       |
|  M1   |         0.79         |     0.62      |    1.25     |      60.89      |
|  M2   |         0.66         |     0.44      |    2.89     |      63.07      |
|  M3   |         0.56         |     0.31      |    1.57     |      62.87      |
|  M4   |         0.82         |     0.67      |    2.68     |      70.19      |
|  M5   |         0.75         |     0.56      |     1.3     |      80.39      |

weights vector = [ 1,1,1,1 ]

impacts vector = [ + , + , - , + ]

### input:

```python
topsis sample.csv "1,1,1,1" "+,+,-,+"
```

### output:

```
      TOPSIS RESULTS
-----------------------------

|Model|Correlation|R2|RMSE|Accuracy|TOPSIS Score|Rank|
|---|---|---|---|---|---|---|
|M1|0.79|0.62|1.25|60.89|0.7722097345612788|2.0|
|M2|0.66|0.44|2.89|63.07|0.22559875426413367|5.0|
|M3|0.56|0.31|1.57|62.87|0.43889731728018605|4.0|
|M4|0.82|0.67|2.68|70.19|0.5238778712729114|3.0|
|M5|0.75|0.56|1.3|80.39|0.8113887082429979|1.0|

```

## License

https://github.com/Ekam3000/Topsis-package-pypi/blob/master/LICENSE.unknown
