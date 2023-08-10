# Simple Language Models

Simple language model is a model that predicts the next unit of text. 

For example, the system receives the *characters*, *words*, and *sentences* as inputs, then calculate the probability distribution so as to give the outputs as the predicting *characters*, *words*, and *sentences*. It is easy to understand but it's not easy to build (personally hehe).

- In **Part 1**, the requirement is to build a neural network named **Multi Layered Perception (MLP)** using `JAX Autodiff`. This model follows a concept of updating the parameters by calculating their gradients. The `Autodiff` is calculated by the chain rule when I step-by-step dot-mutiplied the matrices of weights and biases.

- In **Part 2**, the requirement is to build a **Bigram Language Model**. Again, as mentioned, the concept is easy to understand but very challenging to implement. **Bigram Language Model** is counting the frequency of **2** adjacent characters (or words) in the corpus then calculate the probability distribution. After that, we are able to figure out other characters (or words) to create more of them.
