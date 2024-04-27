# Chauvenet’s Criterion

Chauvenet's criterion is a specific method for detecting outliers in data. It is based on the idea that, for a given dataset, the probability of an outlier occurring is relatively low. Chauvenet's criterion can be useful in certain situations, such as when you want to identify outliers in data that follows a normal distribution. However, it is not necessarily the best method for detecting outliers in all cases, and there are other methods that may be more appropriate in certain situations.

According to Chauvenet’s criterion we reject a measurement (outlier) from a dataset of size N when it’s probability of observation is less than 1/2N. A generalization is to replace the value 2 with a parameter C.

Source — Hoogendoorn, M., & Funk, B. (2018). Machine learning for the quantified self. On the art of learning from sensory data.

## Normal distribution
It's important to note that Chauvenet's criterion is only applicable to datasets that are normally distributed. If your dataset is not normally distributed, this method may not be suitable for identifying outliers.

- Histogram — Do you see a bell shaped curve?

- Boxplot — Is the box symmetrical?