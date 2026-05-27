NEURAL-STYLE-TRANSFER
COMPANY: CODTECH IT SOLUTIONS

NAME: BADVEL SUREKHA

INTERN ID: CTIS8404

DOMAIN: ARTIFICIAL INTELLIGENCE

DURATION: 8 WEEKS

MENTOR: NEELA SANTOSH KUMAR

This project is a Neural Style Transfer application developed using Python and TensorFlow. The main purpose of this project is to combine the content of one image with the artistic style of another image using Artificial Intelligence and Deep Learning techniques. Neural Style Transfer is a popular computer vision technique that uses Convolutional Neural Networks (CNNs) to create visually attractive images by applying painting or artistic styles to normal photographs.

For developing and running this project, the main platform used is Google Colab. Google Colab is a cloud-based Python programming environment provided by Google. It allows users to write and execute Python code directly in the browser without installing software on their local computer. Google Colab is highly useful for AI and deep learning projects because it provides free CPU and GPU support, which helps in faster image processing and model training.

This project also uses TensorFlow, which is one of the most popular deep learning frameworks developed by TensorFlow. TensorFlow provides pre-trained deep learning models and powerful tools for image processing and neural network operations. In this project, the pre-trained VGG19 model is used for extracting image features. VGG19 is a convolutional neural network trained on millions of images and is widely used in computer vision tasks.

The project mainly uses the following Python libraries:

tensorflow for deep learning operations and neural networks.

numpy for numerical calculations.

matplotlib for displaying images.

Pillow (PIL) for image loading and saving.

Before running the project, the required libraries are installed using:

!pip install tensorflow pillow matplotlib

The user needs two images for this project:

A content image – the main image whose structure and objects are preserved.

A style image – the artistic image whose texture and style are applied.

The paths of these images are specified using:

CONTENT_IMAGE_PATH = "content.jpg" STYLE_IMAGE_PATH = "style.jpg"

The program first loads and resizes the images using the load_img() function. The images are normalized and converted into tensors because TensorFlow works with tensor data structures. After loading the images, the VGG19 model extracts important style and content features from both images.

The project uses style layers and content layers from the VGG19 network. The content layers preserve the original structure of the content image, while the style layers capture artistic textures, colors, and patterns from the style image. A Gram Matrix is calculated to represent the style information mathematically.

The training process is performed using gradient optimization. During training, the model gradually modifies the target image to combine the content of the first image with the artistic style of the second image. The optimizer used in this project is Adam Optimizer, which helps improve image quality efficiently.

After training is completed, the final styled image is displayed using Matplotlib and saved automatically as:

styled_output.jpg

This project has many real-world applications in digital art, graphic design, entertainment, photo editing, and social media content creation. Artists and designers can create unique artistic effects automatically using AI. It is also useful in creative industries, gaming, advertising, and mobile photo editing applications.
output:

This project demonstrates how Artificial Intelligence and Deep Learning can be used to generate artistic images through Neural Style Transfer. By using Google Colab, TensorFlow, and VGG19, developers can easily create advanced AI-powered image transformation applications without requiring expensive hardware or advanced machine learning expertise.
