# Scaling, Depth, and Epochs: A Model Comparison Study


![Model Comparison Study](https://github.com/ArdaKaymaz/Concrete_Work/assets/146623362/ff80cc74-2815-4e6c-82ba-0dad265bc7af)

In this study, four models with different structures were evaluated using one dataset. The goal was to demonstrate the importance of scaling, depth of the model, and the number of epochs in relation to accuracy and training durations.

To evaluate the stability and variability of the model's performance, a method was employed where each model was trained 50 times with different random splits of the dataset into training and testing sets. This method involved repeating the process of building and training the model, computing the mean squared error (MSE) between the predicted and actual target values on the testing set, and calculating the mean of the absolute weights of the neural network layers across multiple runs. These results provided insights into the robustness of the model and the stability of its learned parameters.

The first model (Model A), which served as a baseline, included 50 epochs and 1 hidden layer without scaling. The second model (Model B), with the same configuration but including scaling, highlighted the impact of normalization on model performance. The third model (Model C), with 100 epochs and 1 hidden layer, explored the effect of increasing the number of epochs on accuracy and training durations. Finally, the fourth model (Model D), featuring 50 epochs and 3 hidden layers with scaling, examined the influence of model depth on performance.

![output](https://github.com/ArdaKaymaz/Concrete_Work/assets/146623362/21e2a8cb-e117-4ee3-b049-d0ad3585b07d)

The results of the study revealed several key findings. Firstly, scaling played a crucial role in improving accuracy and reducing variation in mean weights across all models. Secondly, increasing the depth of the model resulted in lower training durations and decreased variation in mean weights compared to models with fewer layers. Lastly, while increasing the number of epochs generally led to higher accuracy, it also prolonged training durations.

Overall, the study underscores the importance of scaling for model performance, the benefits of deeper architectures in reducing training durations and enhancing stability, and the trade-offs associated with increasing the number of epochs in terms of computational resources and time. These insights can inform future model development and optimization strategies for similar datasets and tasks.
