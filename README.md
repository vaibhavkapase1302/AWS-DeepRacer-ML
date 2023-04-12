# AWS-DeepRacer-ML
# ML:
What is machine learning?
Common techniques in machine learning:
1) Supervised learning: Labeled Data
2) Unsupervised learning: Unlabeled Data
3) Reinforcement learning: Learns from experience and experimentation

Machine learning (ML) is a modern software development technique, and a type of artificial intelligence (AI), that enables computers to solve problems by using examples of real-world data. 

It allows computers to automatically learn and improve from experience without being explicitly programmed to do so.

<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/ML%20Understand.png" alt="Image Description" width = 50% height=50%>

## Nearly all tasks solved with machine learning involve three primary components:
- A machine learning model
- A model training algorithm
- A model inference algorithm

<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/Components%20of%20machine%20learning.png" alt="Image Description" height=200>

## Model training
In the preceding section, we talked about two key pieces of information: a model and data. In this section, we show you how those two pieces of information are used to create a trained model. This process is called model training.

Clustering: Clustering is an unsupervised learning task that helps to determine if there are any naturally occurring groupings in the data.

Labeled Data

Unlabled data

## Defining a problem in Machine Learning
<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/Define%20the%20problem.png" alt="Example Image">

### Clusteringg: 
It is an unsupervised learning task that helps to determine if there are any naturally occurring groupings in the data.

#  # The Four Aspects of Working with Data

<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/The%20Four%20Aspects%20of%20Working%20with%20Data.png" width="700" height="150" alt="Example Image">
To build a good dataset, there are four key aspects to be considered when working with your data. First, you need to collect the data. Second, you should inspect your data to check for outliers, missing or incomplete values, and to see if any kind of data reformatting is required. Third, you should use summary statistics to understand the scope, scale, and shape of the dataset. Finally, you should use data visualizations to check for outliers, and to see trends in your data.


- Impute: 
Impute is a common term referring to different statistical tools that can be used to calculate missing values from your dataset.

- Outliers:
Outliers  are data points that are significantly different from other date in the same sample.

### Splitting your dataset gives you two sets of data:
* Training dataset: The data on which the model will be trained. Most of your data will be here. Many developers estimate about 80%.
* Test dataset: The data withheld from the model during training, which is used to test how well your model will generalize to new data.

## Key terms:
Hyperparameters:
- Hyperparameters are settings on the model that are not changed during training but can affect how quickly or how reliably the model trains, such as the number of clusters the model should identify.

loss function:
- A loss function is used to codify the model’s distance from this goal.

Training dataset: *Before Training* 
- The data on which the model will be trained. Most of your data will be here.

Test dataset: *After Training*
- The data withheld from the model during training, which is used to test how well your model will generalize to new data.

Model parameters: 
- Model parameters are settings or configurations the training algorithm can update to change how the model behaves.

### Supervised learning:
Using machine learning to predict housing prices in a neighborhood, based on lot size and the number of bedrooms.

### Unsupervised learning
Using machine learning to isolate micro-genres of books by analyzing the wording on the back cover description.

### Deep neural network
While this type of task is beyond the scope of this lesson, we wanted to show you the power and versatility of modern machine learning. You will see how it can be used to analyze raw images from lab video footage from security cameras, trying to detect chemical spills.

## Terminology
- Regression: 
  A common task in supervised machine learning used to understand the relationship between multiple variables from a dataset.
- Continuous:
  Floating-point values with an infinite range of possible values. This is the opposite of categorical or discrete values, which take on a limited number of possible values.
- Hyperplane: 
  A mathematical term for a surface that contains more than two planes.
- Plane: 
  A mathematical term for a flat surface (like a piece of paper) on which two points can be joined by drawing a straight line.
## Here's a list of common metrics:
- Accuracy
- Confusion matrix
- F1 score
- False positive rate
- False negative rate
- Log loss
- Negative predictive value
- Precession
- Rec all
- ROC Curve
- Specificity
   
## Introduction to Reinforcement learning
AWS DeepRacer offers two training algorithms:
- Proximal Policy Optimization (PPO)
- Soft Actor Critic (SAC)

In reinforcement learning, an agent interacts with an environment with an objective to maximize its total reward.

## AWS DeepRacer
<a href="https://us-east-1.console.aws.amazon.com/deepracer/home?region=us-east-1#getStarted">AWS DeepRacer Documantation link</a>

## How does AWS DeepRacer learn to drive by itself?
- Agent: The agent simulates the AWS DeepRacer vehicle in the simulation for training. 
- Environment: The environment contains a track that defines where the agent can go and what state it can be in.
- State: A state represents a snapshot of the environment the agent is in at a point in time.
- Action: An action is a move made by the agent in the current state. 
- Reward: The reward is the **score** given as feedback to the agent when it takes an action in a given state.
 
<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/DeepRacer%20concept%20.png" width="300" height="300" alt="Example Image">

## Training an AWS DeepRacer model
1. Name your model
2. Choose track
3. Choose algorithm type: 
 * Proximal Policy Optimization (PPO)
 * Soft Actor Critic (SAC)
4. Customize reward function
 - Follow the centerline
 - Stay within borders
 - Prevent zig-zag
5. Choose duration
6. Training

## Reward Function:
<img src="https://github.com/vaibhavkapase1302/AWS-DeepRacer-ML/blob/main/Reward%20Function.png" width="500" height="300" alt="Example Image">
<a href="https://youtu.be/pov0afxAvlo">Reward Function Explained </a
  
* Reward function is simply peace of code which uses the input parameters to do some calculation and then output the number which is reward.
* It is return in python as a standard function
