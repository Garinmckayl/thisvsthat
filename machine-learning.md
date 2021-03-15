# Machine Learning

Table of Contents
=================

   * [Tenserflow Vs Pytorch](machine-learning.md#Tenserflow-Vs-Pytorch)


## Tenserflow Vs Pytorch

## What is Tenserflow?
TensorFlow is a free and open-source software library for machine learning. It can be used across a range of tasks but has a particular focus on training and inference of deep neural networks.
Google’s TensorFlow is a famous open-source  an end-to-end deep-learning library for dataflow and differentiable programming across a range of tasks. With great documentation and training support, It is also a symbolic math library and machine learning applications such as neural networks also use this library. 
Research and production are the primary uses of the library. 

## What is Pytorch?

relatively new deep learning framework open-sourced on GitHub in 2017, Based on the Torch library,  
Pytorch is known for its simplicity, ease of use, and dynamic computational graphs. PyTorch follows an imperative computation approach, which means computations run immediately, which means the user needs not to wait to write the full code before checking if it works or not. We can efficiently run a part of the code and inspect it in real-time. The library is python based built for providing flexibility as a deep learning development platform.  
It runs on Linux, macOS, and Windows.




## Differences


TensorFlow was developed by Google and is based on Theano (Python library), whereas Facebook developed PyTorch using the Torch library. 



### Computational Graph Construction 

Tensorflow works on a static graph concept that means the user first has to define the computation graph of the model and then run the ML model, whereas PyTorch believes in a dynamic graph that allows defining/manipulating the graph on the go. 

PyTorch offers an advantage with its dynamic nature of creating the graphs. The graphs are built, interpreting the line of code corresponding to that particular aspect of the graph. However, in the case of TensorFlow, as the construction is static and the graph is required to go through compilation and then executed on execution engine. 



### Serialization 

PyTorch serves a simple API that saves all the weights of the model or pickles the entire class. TensorFlow also offers a significant advantage that the entire graph can be saved as a protocol buffer, including parameters and operations as well. Also, other supported languages such as C++ and Java can load the graph; this is critical for deployment stacks where Python is not offered. It is also useful when the user changes the model source code and but wants to run old models. 



### Visualization

Tenserflow offers better visualization, which allows developers to debug better and track the training process effectively.  
TensorBoard visualizes machine learning models in TensorFlow, which helps during the training the model and spot the errors quickly. TensorBoard is the real-time representation of the graphs of a model that depicts the graph representation and shows the accurate graphs in real-time.


### Deployment

TensorFlow is better than Pytorch in deploying trained machine learning models to production,  
thanks to the TensorFlow Serving framework. Pytorch offers no such framework, so developers need to use Django, Flask or other python web development frameworks as a back-end server.

### Conclusion 

If you’re just starting out on machine learning , 
it is recommended that you should learn Pytorch first due to its simplicity and ease of use. However, if you’re familiar with machine learning and deep learning and focused on getting a job in the industry as soon as possible, learn TensorFlow first.
 Both provide machine learning libraries to achieve various tasks and get the job done. TensorFlow is a powerful and deep learning tool with active visualization and debugging capabilities. TensorFlow also offers serialization benefits as the entire graph is saved as a protocol buffer. It also has support for mobile platforms and offers production-ready deployment. PyTorch, on the flip side, is still gaining momentum and attracting Python developers as it’s more Python friendly. In summary, TensorFlow is used to make things faster and build AI-related products, while research-oriented developers prefer PyTorch.





