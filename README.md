# Object_detection_SSD

# SSD
  - Single shot detector the main thng to know about this is that earlier region proposals are used to predict object presence which was time consuming but here we don't require       regions since this work is done by CNNs itself.

# Data
  - The data structure for this SSD implementation is like
   
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
    
  - Here Annotations consist of ".xml" files which you have generated thriugh any labeling tool.
  - JPEGImages contains images of the frames on which we want to finr-tune our model.
  - trainval.txt or test.txt are the text files which contains the names of the file of corresponding image or label present in that directory.

  
# Run
  - There is a colab file which you can directly run after preparing data.
  - The important files in the repository are voc_dataset.py, train_ssd.py which will require manipulations.
  - I had attached both implementation ie. with command line as well as notebook version.
 
# Refferences
 -  https://github.com/qfgaohao/pytorch-ssd
 -  https://arxiv.org/pdf/1512.02325.pdf
