# Satellite_Pool_Detection
 
Goal: Predict bounding boxes of pool using satellite images <br />
Original data: images.zip (cannot upload due to memory capacity) & metadata.json <br />

Steps:
  1. Preprocess data (Preprocess_01.ipynb) <br />
      -convert bounding polygon to rectangles (just 4 points) <br />
          -source code: https://bitbucket.org/william_rusnack/minimumboundingbox/src/master/
      -find the min max x y coordinates <br />
      -convert json labels to xml label files (one xml file for each image) <br />
      -grab 1000 images and their respective labels to upload on github and to use it on google colab to train (pool_detection.ipynb <- will change file name to subset_data.ipynb)<br />
      
  2. Convert xml files to tf.records and create label_map.pbtxt <br />
      -use generate_tfrecord.py to create tf.records
  
  3. Partition data into train, test <br />
      -use partition_dataset.py
  
  4. Train Model <br />
      -transfer model? <br />
  
  5. Evaluate Model <br />


references: <br />
 -https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html <br />
 -https://medium.com/@ije_good/object-detection-on-satellite-imagery-using-retinanet-part-1-training-e589975afbd5 <br />
