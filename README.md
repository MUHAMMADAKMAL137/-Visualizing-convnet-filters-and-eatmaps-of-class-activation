# Visualizing-convnet-filters-and-heatmaps-of-class-activation
In this project, we started by defining the loss tensor for filter visualization, which helps us understand what specific patterns each filter in a neural network is learning. We then obtained the gradient of the loss with respect to the input, using a gradient-normalization trick to ensure smooth visualization.

Using this information, we implemented a function to fetch Numpy output values given Numpy input values. With this utility, we performed loss maximization via stochastic gradient descent to generate the filter visualizations.

Next, we created a utility function to convert a tensor into a valid image, enabling us to visualize the learned patterns in a visually interpretable manner. We then developed a function to generate a grid of all filter response patterns in a layer, giving us a comprehensive view of each filter's activations.

Moving on, we explored visualizing heatmaps of class activation, which helps us identify the regions in an image that contribute most to the model's predictions. Finally, we set up the Grad-CAM algorithm, a powerful technique for localizing important regions in an image for classification, which complements the information obtained from class activation heatmaps.

In summary, this project involved understanding and visualizing the learned patterns in a pre-trained VGG16 model using various techniques like filter visualization, class activation heatmaps, and the Grad-CAM algorithm.
