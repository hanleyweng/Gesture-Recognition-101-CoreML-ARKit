# Gesture-Recognition-101-CoreML-ARKit
Simple prototype demonstrating how to train your own Object Recognizer (Classifier) and run it live on iOS. Part of a tutorial (🚧 WIP 🚧). Here, we recognise (from the user’s perspective) a spread hand 🖐 , an upwards fist 👊, and when there’s no hands ❎ .

![gif showing fist and spread hand appearing and dissappearing from screen, and it being recognized on an iPhone](post-media/giphy.gif)
[Demo Video - on Youtube](https://youtu.be/P3Q8awgT9Lk)

Technologies: iOS 11, ARKit, CoreML, .mlmodel, Vision Framework, Xcode 9.1 beta

## Notes: 

This is a demonstration of basic Object Recognition. Object Detection (2D or 3D Localization), nor temporal recognition is not covered here.

ARKit is used as it offers a simple way to pass the camera image onto CoreML / Vision. This also sets us up nicely if we want to use ARKit’s 3D features with CoreML in future.

⚠︎ Disclaimer: 

The example model created here is imperfect, not robust, and has many biases (it was created in an hour after all). Its purpose is to simply show the process for creating your own custom Image Recognizer on iOS using CoreML. In other words, it’s a placeholder for the cool (and more accurate) models you’re going to create.

⚠︎ The Example Model:

As noted above, the machine-learning model provided here was generated in a quick 1 hour sketch. Notable biases include: Only trained on right hands, only trained on one skintone 👋🏼 , no jewelry or accessories, fairly plain non-noisey backgrounds. You should replace this model your own. See tutorial (WIP) on building your own model.

## Steps Taken (Draft)

Placeholder: Currently writing a more detailed tutorial. For the time-being, here’s an overview of the steps taken. (You can also view my commit history to see steps involved.)

( Assumes basic iOS knowledge. Basic ML/DNN/CNN knowledge a bonus. )

1. Decide on a few datasets to try. Pick one and continue with the following steps. (If it doesn’t work well, try another.)
2. Tinker with [https://teachablemachine.withgoogle.com/](Google Creative Lab's Teachable Machine) – get a rough gut feeling of what works, what doesn’t - for a simple Image Classifier based on Convolutional Neural Networks (CNNs).
3. Create a MLModel ( [https://www.customvision.ai](CustomVision.ai) can be used for rapid prototyping / map purposes ).
4. Load the model on your iPhone and get it to run in realtime with ARKit.
5. Bonus. Do a few iterations of data tweaking / augmenting to improve the recognition rates.


MIT Open License. Have fun! 😁

