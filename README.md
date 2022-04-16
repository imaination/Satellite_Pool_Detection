# Satellite_Pool_Detection
 
Goal: Predict bounding boxes of pool using satellite images

Steps:
  1. Preprocess data
      -convert bounding polygon to rectangles (just 4 points) <br />
      -find the min max x y coordinates <br />
      -convert json labels to xml label files (one xml file for each image) <br />
      -convert xml files to tf.records <br />
  
  2. Train Model <br />
      -transfer model? <br />
  
  3. Evaluate Model <br />
