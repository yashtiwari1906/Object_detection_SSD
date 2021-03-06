# Object_detection_SSD

# SSD
  - Single shot detector the main thng to know about this is that earlier region proposals are used to predict object presence which was time consuming but here we don't require       regions since this work is done by CNNs itself.

# Data
  - The data structure for this SSD implementation is like
    """
    data
      |----train
      |       |-Annotations
      |       |-JPEGImages
      |       |-ImageSets
      |                 |--Main
      |                      |-trainval.txt
      |----val
      |       |-Annotations
      |       |-JPEGImages
      |       |-ImageSets
      |                 |--Main
      |                      |-trainval.txt
      |----test
             |-Annotations
             |-JPEGImages
             |-ImageSets
                       |--Main
                            |-test.txt
    """
  - Here Annotations consist of ".xml" files which you have generated thriugh any labeling tool.
  - JPEGImages contains images of the frames on which we want to finr-tune our model.
  - trainval.txt or test.txt are the text files which contains the names of the file of corresponding image or label present in that directory.

  
# Run
  - There is a colab file which you can directly run after preparing data.
