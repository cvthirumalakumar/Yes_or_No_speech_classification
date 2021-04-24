# Yes_or_No_speech_classification
## Description
  This project is the my first project in speech processing and also some what dirty as I was the beginner and did this some what complicate....
  Main idea of this project is to classify yes or no sounds by using a deep learning model using pytorch..
  
  [Data set Link](https://www.openslr.org/1/)
  
  ### About the Data set
      
 This data set contains 60 wav files each file contains 8 yes or no sounds and the name of the file gives the labels of the sounds in the file.
 
 ## Steps involved in the project
 
 1. First we seperated the each and every file into single wav file containing a single file either yes for no and foolishly we renamed every sound with just numbes without considering the label.
 
 2. So we again written a program for renaming every file as yes_count.wav and no_count.wav based on the labes provided in the file names.
 
 3. After that we extracted mfcc coefficients from every file and started training the model as we have only 480(60-8) files,training erro didn't decreasing.
 
 4. So we did data agumentation by adding noise to the files.we successfully generated 2400 files from 480 files by adding 4 types of noise.
 
 5. Noises are white gaussian noise and 3 real word noises.
 
 6. After that we extracted mfcc from all 2400 files and stacked them in a csv file along with their respective labels.
 
 7. Finally started training the model and our model successfully tained with training loss converged to 0.00011546086990699497
 
 8. We trained model with 2000 examples and tested with 400 examples
 
 9. We got Test Accuracy of 0.9925
 
 10.  All files involved in this project are uploaded in the repository except the wav files as the data set link is provided above.
