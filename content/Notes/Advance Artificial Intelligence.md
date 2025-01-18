### Website to [Make Mind Map](https://www.mymap.ai/)

### Why use Pretrained Models?
[Source](https://www.ahead.com/resources/why-pre-trained-models-matter-for-machine-learning/)
Pretrained models are already trained models which have grasped the patterns and representations from the data. Model training require a good performance hardware. If everyone is training a model from the scratch then there is just waste of time and recourses if there is other pretrained model available which is better than we trained. Why go and unnecessary train a model if there is better version available trained from the same data? Pretrained models provide ML engineers a good headstart for their project development. If a pretrained model is good and want to fine tune according to specific requirements you can use transfer learning and modify the model according to your requirements. Also if there is anyone out there having very low knowledge to train AI models. They can use a pretrained model. This provides benefits to Non Experts. They have a generalized architecture that is ready to integrate into applications. Developers do not need to spend time designing complex neural networks from scratch, which streamlines the development process. They offer better accuracy and performance as they have learned meaningful Features from large amounts of data.

### What is Random Forest Algorithm?
[Source](https://careerfoundry.com/en/blog/data-analytics/what-is-random-forest/)
Random Forest is a  **supervised machine learning algorithm** that grows and combines multiple decision trees to create a “forest.” It can be used for both classification and regression problems.
#### What is Supervised Learning?
Supervised machine learning is when the algorithm (or model) is created using labelled data. Where each input and its respective Output is Provided to train.
#### What are regression and classification in machine learning?
For a simple way to distinguish between the two, remember that **classification is about predicting a label** (e.g. “spam” or “not spam”) while **regression is about predicting a quantity**.
#### 1. What are decision Trees?
A decision tree is another type of algorithm used to classify data. In very simple terms, you can think of it like a flowchart that draws a clear pathway to a decision or outcome; it starts at a single point and then branches off into two or more directions, with each branch of the decision tree offering different possible outcomes. As we know, the Random Forest model grows and combines multiple decision trees to create a “forest.”
![](https://cdn.careerfoundry.com/en/wp-content/uploads/old-blog-uploads/decision-tree-example-2-1.jpg)

#### 2. How Random Forest Algorithm Works?
Random Forest grows multiple decision trees which are merged together for a more accurate prediction.

The logic behind the Random Forest model is that multiple uncorrelated models (the individual decision trees) perform much better as a group than they do alone. When using Random Forest for classification, each tree gives a classification or a “vote.” The forest chooses the classification with the majority of the “votes.” When using Random Forest for regression, the forest picks the average of the outputs of all trees.

The key here lies in the fact that there is low (or no) correlation between the individual models—that is, between the decision trees that make up the larger Random Forest model. While individual decision trees may produce errors, the majority of the group will be correct, thus moving the overall outcome in the right direction.

#### Are decision trees in Random Forest different from regular decision trees?
It’s easy to get confused by a single decision tree and a decision forest. It seems like a decision forest would be a bunch of single decision trees, and it is… kind of. It’s a bunch of single decision trees but all of the trees are mixed together randomly instead of separate trees growing individually.

When using a regular decision tree, you would input a training dataset with features and labels and it will formulate some set of rules which it will use to make predictions. If you entered that same information into a Random Forest algorithm, it will randomly select observations and features to build several decision trees and then average the results.

For example, if you wanted to predict how much a bank’s customer will use a specific service a bank provides with a **single decision tree**, you would gather up how often they’ve used the bank in the past and what service they utilized during their visits. You would add some features that describe that customer’s decisions. The decision tree will generate rules to help predict whether the customer will use the bank’s service.

If you inputted that same dataset into a **Random Forest**, the algorithm would build multiple trees out of randomly selected customer visits and service usage. Then it would output the average results of each of those trees.
#### How are the trees in a Random Forest trained (Bagging Explained)?
Decision trees in an ensemble, like the trees within a Random Forest, are usually trained using the “bagging” method.

The “bagging” method is a type of ensemble machine learning algorithm called Bootstrap Aggregation. An ensemble method combines predictions from multiple machine learning algorithms together to make more accurate predictions than an individual model. Random Forest is also an ensemble method.

**Bootstrap** randomly performs row sampling and feature sampling from the dataset to form sample datasets for every model.

**Aggregation** reduces these sample datasets into summary statistics based on the observation and combines them. Bootstrap Aggregation can be used to reduce the variance of high variance algorithms such as decision trees.

**Variance** is an error resulting from sensitivity to small fluctuations in the dataset used for training. High variance will cause an algorithm to model irrelevant data, or noise, in the dataset instead of the intended outputs, called signal. This problem is called **overfitting**. An overfitted model will perform well in training, but won’t be able to distinguish the noise from the signal in an actual test.

**Bagging** is the application of the bootstrap method to a high variance machine learning algorithm.

#### 3. What is Random Forest used for?
Random forest is used on the job by data scientists in many industries including banking, stock trading, medicine, and e-commerce.

It’s used to predict the things which help these industries run efficiently, such as customer activity, patient history, and safety.

Random Forest is used in **banking** to detect customers who are more likely to repay their debt on time. It’s also used to predict who will use a bank’s services more frequently. They even use it to detect fraud. Talk about the robin hood of algorithms!

**Stock traders** use Random Forest to predict a stock’s future behavior. It’s used by **retail companies** to recommend products and predict customer satisfaction as well.

Scientists in China used Random Forest to study the spontaneous combustion patterns of coal to reduce safety risks in **coal mines**!

In **healthcare,** Random Forest can be used to analyze a patient’s medical history to identify diseases. Pharmaceutical scientists use Random Forest to identify the correct combination of components in a medication or predict drug sensitivity. Sometimes Random Forest is even used for computational biology and the study of genetics.