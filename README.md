# Facial Sobriety Analysis

## Problem
Modern breathalyzers require bulky hardware to be transported to events people go to everyday. People who are intoxicated don't carry breathalyzers themselves and end up in troubled situations, sometimes resulting in losing our loved ones.
The following are some of the statistics on drunk driving:

**Statistics**
* Every day, 28 people in the United States die from drunk driving
  * That's one person dead every 52 minutes
* In 2019, 10,142 people lost their lives due to drunk driving
* Approximately one third of all car crashes involve drunk drivers

**How alcohol affects driving**
* When you drink alcohol, it is absorbed through the walls of the stomach and small intestine
* It enters into the bloodstream where it accumulates until broken down by the liver
* While in the bloodstream, it reduces the function of the brain
  * Impairs thinking, mental functioning and decision making
* BAC > 0.08 is illegal in the United States

## Solution

### How It Works
We are building an iOS application that takes live facial data and predicts whether one is intoxicated.

**Convolutional Neural Network**
* 2D CNN Layers - 4
  * Pooling: (2, 2)
  * Dropout: 0.1-0.3
  * Activation: RELU
* Dense Layers - 5
  * Activation: RELU
* Compilation
  * Optimizer: Adam
  * Loss: Binary Crossentropy

## Limitations and the Future
### Limitations
Our data was sourced from a PhD study with a limited dataset. Using image augmentation, we were able to multiply our image set significantly for this proof of concept. To finish the project, we will need to source a large dataset of intoxicated individuals at different levels of intoxication.

### The Future
Developing voice recognition feature to identify irregularities/anomalies in speech to gauge state of being.
