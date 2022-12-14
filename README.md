# Image Enhancement Based on Visual Inference

In computer graphics, photorealism has been a goal that has gained enormous progress over the last half of the century. Nowadays, state-of-the-art techniques provide impressive results that one can find hard to differentiate from real images. However, these state-of-the-art techniques, although impressive, come with a high cost as they are computationally heavy and nearly impossible to achieve at interactive rates. Video games rely on interactive rates to perform a pleasant gameplay experience for the user. Even if the quality of graphics of recent video games has substantially advanced over the last decade, we can easily conclude that the output of current state-of-the-art rendering pipelines is fake, even in the most sophisticated games.
 
With the evolution of machine learning techniques, such as deep learning, convolutional networks, and generative adversarial networks, we can synthesize photorealistic images based on large datasets. These synthesized images produced by these networks can capture photorealism if trained with photographs of the real world. However, using these models in real-time rendering has been challenging as they are hard to implement and control.
 
In this project, we will implement and control the output of a generative adversarial network in the "post-processing" phase of the rendering pipeline. The post-processing phase, as its name indicates, comes after processing the so-called gbuffers that output the composite image of our interactive application. In essence, our model will evaluate the realism of this composite image and will output a corrected version of it in the post-processing phase.
 
In other words, our model will be able to interpret the intent of the synthetic image in the processed phase of the rendering pipeline and generate a corrected version of it in the post-processing phase capturing the aspects of photorealistic appearances. The expected output quality of the processing phase (i.e., gbuffers) can be something other than an attempt at photorealism. Instead, it should contain enough information to be distinguishable and ready for interpretation.

Attempting to achieve photorealism in the processed phase of the rendering pipeline comes with a high computational cost that is preferable to be avoided. We propose to have the lightest possible output from that phase. 

