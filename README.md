# Satellite_Pool_Detection
 
Goal: Predict bounding boxes of pool using satellite images

Steps:
  1. Preprocess data <br />
      -convert bounding polygon to rectangles (just 4 points) <br />
          -source code: https://bitbucket.org/william_rusnack/minimumboundingbox/src/master/
      -find the min max x y coordinates <br />
      -convert json labels to xml label files (one xml file for each image) <br />
      -convert xml files to tf.records <br />
  
  2. Train Model <br />
      -transfer model? <br />
  
  3. Evaluate Model <br />


references: <br />
 -https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html <br />
 -https://medium.com/@ije_good/object-detection-on-satellite-imagery-using-retinanet-part-1-training-e589975afbd5 <br />
