## This is how I define ground truth labels of images by using a pretrained SSD

In this case, every image of a class stays under the same file. 

```pseudo
Go to the main path that contains the files related to classes
Get into the first file
    For all images of the file:
        Read an image and pass through the pre-trained SSD to extract only cars
            If detected object is higher than certain size:
                Label it as a class related to that file
            If not:
                Ask annotator to label it:
                    Annotator can label it as one of 7 classes or delete it
        Go to next image
Go to next file if any
```

## There are three approaches in this work

![alt text](images/overview.png "Overview of the Approaches")

## It is flowchart of the application

![alt text](images/flowchart.png "Overview of the Approaches")
