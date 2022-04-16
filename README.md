# Satellite_Pool_Detection
 
Goal: Predict bounding boxes of pool using satellite images

Steps:
  1. Preprocess data
      -convert bounding polygon to rectangles (just 4 points)
      -find the min max x y coordinates
      -convert json labels to xml label files (one xml file for each image)
      -convert xml files to tf.records
  2. Train Model
      -transfer model?
  3. Evaluate Model
