# Creating Customer Segments

### Project in progress (3/14/16)

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

## Questions:

####Question 1: In this section you will be using PCA and ICA to start to understand the structure of the data. Before doing any computations, what do you think will show up in your computations? List one or two ideas for what might show up as the first PCA dimensions, or what type of vectors will show up as ICA dimensions.


#### Question 2: How quickly does the variance drop off by dimension? If you were to use PCA on this dataset, how many dimensions would you choose for your analysis? Why?


#### Question 3: What do the dimensions seem to represent? How can you use this information?


#### Question 4: For each vector in the ICA decomposition, write a sentence or two explaining what sort of object or property it corresponds to. What could these components be used for?


#### Question 5: What are the advantages of using K Means clustering or Gaussian Mixture Models?



#### Question 6:  What are the central objects in each cluster? Describe them as customers.

###Conclusions

#### Question 7:  Which of these techniques did you feel gave you the most insight into the data?


#### Question 8: How would you use that technique to help the company design new experiments?


#### Question 9: How would you use that data to help you predict future customer needs?


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
