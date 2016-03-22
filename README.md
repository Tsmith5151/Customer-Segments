# Creating Customer Segments

## Project Description:

- A wholesale grocery distributor wants determine which changes will benefit their business. They recently tested out a change to their delivery method, from a regular morning delivery to a cheaper, bulk evening delivery. Initial tests didn’t discover any significant effect, so they implemented the cheaper option. Almost immediately, they began getting complaints about the change and losing customers. As it turns out, the highest volume customers had an easy time adapting to the change, whereas smaller family run shops had serious issues with it, but these issues were washed out statistically by noise from the larger customers.

- For the future, they want to have a sense of what sorts of different customers they have. Then, when implementing changes, they can look at the effects on these different groups independently. The objective is to use unsupervised learning techniques to see what sort of patterns exist among existing customers, and what exactly makes them different.

## Source Code

- In this directory (`customer_segments/`), run `ipython notebook`, open `customer_segments.ipynb`.

## Software & Libraries:

 - Python 2.7
 - NumPy
 - pandas
 - matplotlib
 - scikit-learn

## Dataset

- The dataset refers to clients of a wholesale distributor. It includes the annual spending in monetary units (m.u.) on diverse product categories. It is part of a larger database published with the following paper:

`Abreu, N. (2011). Analise do perfil do cliente Recheio e desenvolvimento de um sistema promocional. Mestrado em Marketing, ISCTE-IUL, Lisbon.`

## Principal Component Analysis:

- [`Principal Component Analysis`](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) is an unsupervised linear transformation technique which transforms possibly correlated variables into a smaller number of uncorrelated variables which are referred to as the principal components. The objective of PCA is to identify patterns in data based on the correlation between features. PCA attempts to find the direction with the maximum variance in a high-dimensional dataset and then project it onto a new subspace with equal or fewer dimensions that the original one. 

- The principal components are the underlying structure of the data and the are defined by the directions that maximizes the variance (the direction where the data is most spread out); this minimizes the information loss when projecting onto the new axis. The perpendicular axes (orthogonal) are known principal components of the new subspace can be interpreted as the directions of maximum variance. The first step consists of placing the first axis in the direction of greatest variance of the points to maximize the variance along the corresponding axis. The second axis is orthogonal to it. In higher dimensions (greater than 2) the second axis could lie anywhere in the plane perpendicular to the first axis. As a constraint, the second axis always perpendicular (orthogonal) to the first axis to maximizes the variance along the axis.(The figure shown below source: Python Machine Learning)

- Calculate the covariance matrix of the original coordinates of the points and diagonalize it to find the eigenvectors. These are the axes of the transformed space, sorted in order of eigenvalue—because each eigenvalue gives the variance along its axis.

## Attributes

- Fresh: annual spending (m.u.) on fresh products (Continuous)
- Milk: annual spending (m.u.) on milk products (Continuous)
- Grocery: annual spending (m.u.)on grocery products (Continuous)
- Frozen: annual spending (m.u.)on frozen products (Continuous)
- Detergents_Paper: annual spending (m.u.) on detergents and paper products (Continuous)
- Delicatessen: annual spending (m.u.)on and delicatessen products (Continuous)

## Descriptive statistics

**Attribute: (Minimum, Maximum, Mean, Std. Deviation)**

- Fresh: ( 3, 112151, 12000.30, 12647.329)
- Milk: (55, 73498, 5796.27, 7380.377)
- Grocery: (3, 92780, 7951.28, 9503.163)
- Frozen: (25, 60869, 3071.93, 4854.673)
- Detergents_Paper: (3, 40827, 2881.49, 4767.854)
- Delicatessen: (3, 47943, 1524.87, 2820.106)
