# Sign-Language-prediction

Sign language recognition is a problem that has been addressed in research for years. However, we are still far from finding a complete solution available in our society.
Among the works developed to address this problem, the majority of them have been based on basically two approaches: contact-based systems, such as sensor gloves; or vision-based systems, using only cameras. The latter is way cheaper and the boom of deep learning makes it more appealing. This post presents a prototype of a dual-cam first-person vision translation system for sign language using convolutional neural networks. The post is divided into three main parts: the system design, the dataset, and the deep learning model training and evaluation.

Trying to understand sign language from a first-vision perspective has the same limitations, some gestures will end up looking the same way. But, this ambiguity can be solved by locating more cameras in different positions. In this way, what a camera can’t see, can be perfectly observable by another camera.
The vision system is composed of two cameras: a head-mounted camera and a chest-mounted camera. With these two cameras we obtain two different views of a sign, a top-view, and a bottom-view, that works together to identify signs.
