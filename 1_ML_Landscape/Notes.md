<h3>Types of Machine Learning Systems</h3>
<h4>Training Supervision </h4>
<b>Supervised Learning </b>
In supervised learning, the training set fed to the algorithms includes the desired solutions, called labels.
e.g.: Classification, Regression

<b>Unsupervised Learning</b>
- Clustering algorithm, 
- Dimensionality Reduction: simplify the data without losing too much information. Merge correlated features into one (feature extraction)
- Visualization algorithms
- Anomaly Detection: fraudulent transactions or Novelty Detection

<b>Semi-supervised Learning</b>

<b>Self-supervised Learning</b>

<b>Reinforcement Learning</b>
agent in this context, can observe the environment, select and perform actions, and get rewards in return( or penalties in the form of negative rewards)

<h4>Batch vs. Online Learning</h4>
<b>Batch Learning:</b> the system is incapable of learning incrementally: it mush be trained using all the available data. This will generally take a lot of time and computing resources.
<i>Offline learning</i> First the system is trained, and then it is launched into production and runs without learning anymore; it just applied what it has learned.
Unfortunately, a model's performance tends to decay slowly over time, simply because the world continues to evolve while the model remains unchanged. this phenomenon is often called <i>model rot</i> or <i>data drift</i>

<b>Online Learning:</b> Train the system sequentially by feed it individual instances or in small groups called <i>mini-batches</i>. Online learning is useful for systems that need to adapt to change extremely rapidly.
<i>out-of-core</i> learning (offline) or incremental learning.

<h4>Instance-Based vs. Model-Based Learning</h4>
<b>Instance-Based Learning:</b> The system learns the examples by heart, and then generalizes the new cases by using a similarity measure to compare them to the learned examples.

<b>Model-Based Learning</b>: Generalize from a set of examples is to build a model of these examples and then use that model to make predictions.
	utility function: measure how good a model is
	cost function: measures how bad a model is

<h3>Main Challenges of Machine Learning</h3>
<b>Insufficient Quantity of Training Data</b>

<b>Nonrepresentative Training data</b>
	Sampling Noise
	Sampling Bias

<b>Poor-Quality Data</b>

<b>Irrelevant Features</b>

<b>Overfitting the Training Data</b>
Model performs well on the training data, but it does not generalize well.
Overfitting happens when the model is too complex relative to the amount and noisiness of the training data. Here are possible solutions:
	Simplify the model by selecting one with fewer parameters, by reducing the number of attributes in the training data, or by constraining the model.
	Gather more training data.
	Reduce the noise in the training data (e.g., fix data errors and remove outliers).
Constraining a model to make it simpler and reduce the risk of overfitting is called <b>regularization</b>

<b>Underfitting the Training Data</b>
Model is too simple to learn the underlying data structure of the data. Here are possible solutions:
	Select a more powerful model, with more parameters.
	Feed better features to the learning algorithm (feature engineering)
	Reduce the constraints on the model

<h3>Testing and Validating</h3>
<h3>Hyperparameter Tuning and Model Selection</h3>
Generalization error: Error on test set.
Measuring the generalization error multiple times on the test set while hyper-parameter tuning and model selection may result in selecting a model that provided best score for that particular test set. 
Holdout validation.
<i>cross-validation</i>: to avoid issues with large(if there are not many instances, larger set might be expensive as it would need system to gather more data points) vs small (imprecise evaluation) validation set. However, the training time is multiplied by the number of validation sets.

<h4>Data Mismatch</h4>




