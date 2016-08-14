# Dog

Dog is a project designed to recognize the type of a dog. It was written in Python, which means the code can run on major OS, such as Windows 7 or up, Ubuntu 14.04 or up and other Linux distributions.

# Build

To build this project, you must have [Keras](https://github.com/fchollet/keras#installation) and one of its back-ends to be installed, h5py and PIL is also required for building this project.

You could just type the command below to make the project work:

```shell
python run.py tmp.jpg
```

# Example

It's very easy to use. Suppose you want to recognize a new dog and prepared a Image file(suppose dog.jpg). We can write a new Python script and name it as test.py:

```Python
from PIL import Image
img = Image.open('dog.jpg')
img = img.resize(128, 128) # omit this if this is already resized
img = img.convert('RGB') # omit this if this is already converted
img.save('dog_1.jpg')
```

And then we could just type the command below to make the project work:

```shell
python test.py
python run.py dog_1.jpg
```

For more usage, please go to the [project wiki](https://github.com/peterjc123/SMU-JWC-API/wiki) for more information.