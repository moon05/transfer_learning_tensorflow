# Transfer Learning for Dog Breed Classification

I peformed image classification on the Stanford Dogs Dataset. The dataset contains images of 120 breeds of dogs. You can read more about the dataset on this [page]. You can directly download the Images [here]. <br>

I used different models to test experiment what kind of accuracy is obtainable. <br>

|Model        | Learning Steps | Accuracy|
|-------------|----------------|----------|
|Inception-v3 | 1000           | 92%      |
|Inception-v3 | 4000           |          |
|Resnet       | 4000           |          |
|Mobilenet    | 4000           |          |


## Requirements
* Python <br>
* Tensorflow <br>
* Tensorhub <br>

## Usage
If you would like to test this model out you can use the label_image.py script to do so. <br>

__Format__:

python label_image.py --graph_data=<whichever_output_graph_learning_rate> --labels=output_labels.txt --input_layer=Placeholder --output_layer=final_result --image=<name_of_image_you_want_to_test> <br>

__Example__:

python label_image.py --graph_data=output_graph_inception_1000.pb --labels=output_labels.txt --input_layer=Placeholder --output_layer=final_result --image=./test_photos/doberman_2.jpg <br>

This will print out couple dog breed names followed by the likeliness of the picture belonging to that breed of dog. <br>

Of course you can experiment it with any dog picture you would like, but if you want to try it out with some of the existing pictures in the dataset below are some names. <br>

Some of the popular dog breed names that exist in the directory: <br>

1. Beagle, 2. Bernese Mountain Dog, 3. Bloodhound, 4. Border Collie, 5. Doberman, 6. German Shepherd, 7. Malamute <br>

Here are some less common dog breeds but equally beautiful looking: <br>

1.Afghan Hound, 2. Giant Schnauzer, 3. Ibizan Hound, 4. Irish Wolfhound, 5. Kuvasz 6. Vizsla, 7. Weimaraner <br>

I have also included a directory called "test_photos" which includes some random pictures of some dog breeds I grabbed from simple Google image searching if you think that would be easier for you to test it out.

Here's what the results looks like using the doberman_2.jpg file: <br>

<img src="https://github.com/moon05/transfer_learning_tensorflow/blob/master/test_photos/doberman_2.jpg" height="75">

![alt text][result]<br>


[page]: http://vision.stanford.edu/aditya86/ImageNetDogs/
[here]: http://vision.stanford.edu/aditya86/ImageNetDogs/images.tar
[dob_2]: https://github.com/moon05/transfer_learning_tensorflow/blob/master/test_photos/doberman_2.jpg
[result]: https://github.com/moon05/transfer_learning_tensorflow/blob/master/sample_result_screenshot.png

