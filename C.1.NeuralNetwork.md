# But What is a neural network? by 3blue1brown

Machine Learning Neural Network

Structure of neural Network

Convolution neural network -> Good for image recognition

Long short-term memory network -> Good for speech recognition

NN

What are neurons? -> a thing that holds number in a basic sense

Let's say there is a 28x28 image of a handwritten number in it.

each pixel in that image holds a value from 0-9, in this context 0 is black, 9 is white.

when we write a handwritten number on the image, the pixels which have the number written on them have higher value.

Now let's arrange all the pixels in a straight line because for a computer it doesn't care if an image is 1 Dimensional or 2 Dimensional.

Now we have 28x28 = 784 neurons.

What could be the output of these 784 neurons?

It's a handwritten text of 0-9 hence the output is 0-9, 10 neurons (nodes).

Here is the 4th neuron which points to the number 3, has a value of 0.6, and the 9th neuron which points to the number 8 has a value of 0.4 and rest of the neurons have 0.0. So by probability we assume that this number most likely is 3.

How does 784 neurons assign weights to 10 neurons? There are hidden layers between the 784 neurons and 10 neurons. Here 784 neurons are the input, and 10 neurons are the output, while the hidden layers which are made of neurons are the logic. (The thing that does the calculation).

2 hidden layers each one with 16 neurons, which is just arbitrary choice.

Activations in one layer determine the activation in the next layer,

How can these layers be expected to act intelligently

In a perfect world where we know how what these neurons actually mean, the layer before last might have loops, lines, different types of curved lines corresponding to the respected digits like

3 might have 2 curved lines, 8 might have 2 loops, 1 might have a single line.

this is just a example of what might the layers have, just recognizing the curves and loops for a layer is hard enough. in the real world we don't know what these weights actually represent.

These edges and lines are the ones which help we distinguish different numbers to distinguish everything we see.

This can also corelate to audio's when we

pick out a raw audio, pick out different sounds, putting the sounds together to make certain syllables, which combine to make words, which combine to make sentences and more abstract thoughts and etc.

so a neuron

Lets take a neuron in the 2nd layer, now we assign a weight to each one of the connections to our neuron and the neurons from the first layer, Then take all those activations from the first layer and compute their weighted sum according to these weights (connections).

Sigmoid ->

we add a bias which means that this connection has some knowledge in it, this bias determines if this bias is at a specific threshold we can make use of this specific neuron's knowledge.

every other neuron has these connections and their knowledge, and each one have their own bias.

This NN has 784x 16+ 16 x 16+ 16 x 10 weights 16+16+10 biases 13,002 weights and biases, which means 13,002 knobs and diodes that could be tweaked and turned to make this network behave in different ways.

So when we talk about learning -> we mean finding the right weights and biases a(1) sigmoid (Wa(0) + b)

Matrix vector product of first layer and each neuron in the second layer, Learning rate.

Neuron is a function one that takes in the outputs of all the layers in the previous layer and spits of a number between 0 and 1.

really the entire network is a function.

ReLU vs Sigmoid

Rectified linear unit, sigmoid is old

ReLU is easier to train,

How does one layer influence the next layer?

How does training work?




Gradient Descent, how neural networks learn


