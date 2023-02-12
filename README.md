# train-yolov8-custom-dataset

#Preparing-a-custom-dataset

#Building a custom dataset can be a painful process. It might take dozens or even hundreds of hours to collect images, label them, and export them in the proper format. Fortunately, Roboflow makes this process as straightforward and fast as possible. Let me show you how!

#Step 1: Creating project
Before you start, you need to create a Roboflow account. Once you do that, you can create a new project in the Roboflow dashboard. Keep in mind to choose the right project type. In our case, Object Detection.
![creating-project](https://user-images.githubusercontent.com/55156159/218303607-99318cd5-3457-4f04-aa38-e2d2948812de.gif)

#Step 2: Uploading images
Next, add the data to your newly created project. You can do it via API or through our web interface.

If you drag and drop a directory with a dataset in a supported format, the Roboflow dashboard will automatically read the images and annotations together.
![uploading-images](https://user-images.githubusercontent.com/55156159/218303773-39f48f49-bbc3-45d5-b373-09a05fe9fce7.gif)

#Step 3: Labeling

If you only have images, you can label them in Roboflow Annotate.
![210901980-04861efd-dfc0-4a01-9373-13a36b5e1df4](https://user-images.githubusercontent.com/55156159/218303833-36432f74-700d-40f9-836e-fbb736e07429.gif)


#Step 4: Generate new dataset version

Now that we have our images and annotations added, we can Generate a Dataset Version. When Generating a Version, you may elect to add preprocessing and augmentations. This step is completely optional, however, it can allow you to significantly improve the robustness of your model.
![generate-new-version](https://user-images.githubusercontent.com/55156159/218303867-33b9544e-aaf4-45cf-8791-d78fdb5ca3c8.gif)

#Step 5: Exporting dataset

Once the dataset version is generated, we have a hosted dataset we can load directly into our notebook for easy training. Click Export and select the YOLO v5 PyTorch dataset format.
![export](https://user-images.githubusercontent.com/55156159/218303890-456cccba-f32f-4ca5-a947-f5803e0d85ab.gif)
