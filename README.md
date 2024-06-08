# MNIST_digit_recognizer

MNIST, short for "Modified National Institute of Standards and Technology," has been a cornerstone dataset in the field of computer vision since its release in 1999. It serves as the quintessential "hello world" dataset for classification algorithms, providing tens of thousands of handwritten images of digits for researchers and learners to benchmark their techniques.


data:image/png;base64,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