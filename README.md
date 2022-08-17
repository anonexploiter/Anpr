git clone : https://github.com/anonexploiter/Anpr.git

Step 1. Create a new virtual environment
```python -m venv recv```

Step 2. Activate your virtual environment
```
.\recv\Scripts\activate
``` 

Step 3. Install dependencies and add virtual environment to the Python Kernel
```
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
```

Step 4. Collect images using the Notebook.
```
jupyter notebook
```

Step 5. Intializing the path and download the tensorflow object detection

Step 6. Creating label map for identifying and train the detection of objects ( Number plate).--> green box

Step 7. Creating TF records and setup the folder for 'generated-tfrecord' to initialize the image annotations for train and test of a dataset

Step 8. Train the dataset with generated-tfrecord to initialize the child nodes for analyzing the number plate.

Step 9. Create a pipeline file for setting up the path to train the model folder.

step 10. Copy the model config (pipeline file --> which is used to mention the path when an detection runs) to training folder for the stage of pretraining.

step 11. Update the config files for Training the transfer learning using object detection api in tensor flow

Step 12. run the config file to setup the path for pipeline.

Step 13. Train the model with the respective tensorflow folders

Step 14. run the trained steps in cmd prompt to get checkpoint index(which is used to mention the accuracy of detection in realtime as well as image file)

Step 15. Evaluate the trained dataset model folder and checkpoints

Step 16. Load the trained model which as checkpoints , for that from object_detection api model_builder will used and that also allows to built the config_utils.

Step 17. preventing the gpu cores to setup virtual device.

Step 18. Load pipeline config and build a detection model.

Step 19. restore the checkpoints for the loaded pipeline line config file(it gives shape to that detection)

Step 20. Detection from an image Cv2 is used to load the path of trained model via the pipeline config file.numpy is used to make coordinates with the images annotaion files.matplotlib uses pyplot to make grap for accurate detection.

Step 21. Realtime detection from webcam. it uses opencv to open web cam and capture the number of objects and stores it as image.

step 22.For image file Apply ocr by using pytorch and easyocr , it gives more threshold in detection . it apply ocr filters like applying blur , gray scaling, mono scaling ....

Step 23. For Realtime Apply ocr by using pytorch and easyocr, it apply ocr filters like applying blur , gray scaling, mono scaling in detected and stored number plates.

Step 24. For better detection bringing those and makes ROI(region of intrest(number palte)) for storing , the detection boxes were applied when they are processed in generating ocr phase.

Step 25. Saving the result with the help of CSV module to store the extracted data in .csv file with the unique identifier id.(further steps involved to manage the detected number plates in cloud).


