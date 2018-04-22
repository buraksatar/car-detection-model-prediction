## This is how I define ground truth labels of images by using a pretrained SSD

```pseudo
Go to the main path that contains the files related to classes
Get into the first file
    For all image:
        Read the image, go through pre-trained SSD to extract cars
            If the object is higher than certain size:
                Label it as a class related to file that reading
            If not:
                Ask the annotator to label it:
                    Annotator can label it as one of 7 classes or delete it\
Do it for every file
```

## There are three approaches in this work

![alt text](images/overview.png "Overview of the Approaches")

