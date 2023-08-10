# Simple Language Models

**Simple language model** is a model that predicts the next unit of text. A statistical model known as a language model is employed to estimate **the likelihood of a word sequence** appearing in a particular language. This model is trained on extensive text collections and serves the purpose of generating fresh text or assessing the probability of a specified word sequence.

For example, the system receives the *characters*, *words*, and *sentences* as inputs, then calculate the probability distribution so as to give the outputs as the predicting *characters*, *words*, and *sentences*. It is easy to understand but it's not easy to build (personally hehe).

Below are some general stages for training a language model:

- Process and sanitize the text data.
- Convert the textual content into a numerical representation.
- Establish the model's structure: pick the neural network type, and set parameters like layer count, hidden units, and activation functions.
- Specify the loss function: options include max-margin, negative log-likelihood, cross-entropy loss, RMSE, etc.
- Train the model: initialize model parameters, define the optimizer, and execute the training loop for a specific number of epochs to minimize the loss function.
- Adjust parameters: fine-tune hyperparameters or the model itself based on gradients derived from the loss function.
- Assess the model's performance.
- Generate novel text.

## Project's Details:

- In **Part 1**, the requirement is to build a neural network named **Multi Layered Perception (MLP)** using `JAX Autodiff`. This model follows a concept of updating the parameters by calculating their gradients. The `Autodiff` is calculated by the chain rule when I step-by-step dot-mutiplied the matrices of weights and biases.

- In **Part 2**, the requirement is to build a **Bigram Language Model**. Again, as mentioned, the concept is easy to understand but very challenging to implement. **Bigram Language Model** is counting the frequency of **2** adjacent characters (or words) in the corpus then calculate the probability distribution. After that, we are able to figure out other characters (or words) to create more of them.
