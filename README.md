# MiniProject_Speech_To_Text_Using_MFCC_and_HMM
Mini Project - Speech to text conversion using MFCC, GMM and HMM


## Problem definition

The goal of this synopsis is to build a real time speech recognizer demonstrator using a template matching approach The application would generate a visual feedback for the user after the speech recognition is performed, simply by displaying the recognized word and thus providing an interface to show and test the recognition capabilities.


## Automatic Speech Recognition

Nowadays speech signal is commonly represented as a sequence of vectors in an acoustic space. It is acquired that two sequences of the same succession of pronounced words have some similarities. The speech recognition problem becomes “simply” the measure of the dissimilarity between prerecorded and processed sequences and the speech pronounced. A decision rule will be used to decide with a certain confidence which words have been pronounced. The major work in speech recognition consists in enhancing the algorithm used for this method.

In ASR, the main task is to derive a sequence of words from a stream of acoustic information. One further processing step for an application is speech understanding. It includes a language analyzer and an expert system to select the correct/desired output, then to replace it in the context and finally to derive an appropriate command representing the user expectation. Sometimes ASR can also be seen as a process which includes speech understanding. But most of the time ASR and speech understanding are strongly linked and difficult to clearly distinguish, as the processing of each one depends closely on the other. In this work we will focus on the speech recognition process. The structure of any speech recognition system follows the three basic steps represented in Figure 1, namely feature extraction, pattern comparison and decision rule.


## Project design status

## Architecture

![image](https://user-images.githubusercontent.com/73153277/125280518-c3561280-e332-11eb-979e-892f251778fb.png)

## Acquisition of speech recordings from user
            
Using the audacity tool speech samples will be collected.

## Feature Extraction

![image](https://user-images.githubusercontent.com/73153277/125280686-f8fafb80-e332-11eb-8f95-624aa1a8a2c7.png)


## Test environment creation

![image](https://user-images.githubusercontent.com/73153277/125280785-19c35100-e333-11eb-82ad-8536046b767b.png)

Four words ‘yes’, ‘no, ‘left’, ‘right’  of different variations in the speech are recorded. 20 variations per word saved in the folder labelled with the respective words. These recorded words are fed into the speech recognition program to train and accuracy and confusion matrix are obtained.

![image](https://user-images.githubusercontent.com/73153277/125280851-2a73c700-e333-11eb-9465-77d8657f9c9b.png)
                             Folder containing all the audio samples 
                             
![image](https://user-images.githubusercontent.com/73153277/125280936-42e3e180-e333-11eb-88d4-0e75f23fd426.png)
                             Different variation Audio samples for the word ‘no’
          
          
          
## Result obtained

Accuracy and confusion matrix calculated and is shown below for standard Kaggale testing dataset

![image](https://user-images.githubusercontent.com/73153277/125281035-61e27380-e333-11eb-9104-d340dd82a11d.png)
                             Results with Confusion Matrix for Kaggle dataset
                             
Accuracy and confusion matrix calculated and is shown below for Kannada number testing dataset with noise.

![image](https://user-images.githubusercontent.com/73153277/125281161-83dbf600-e333-11eb-8c68-0e28fa4caa4d.png)
                             Results with Confusion Matrix for Kannada number recorded dataset
                             
Speech recognised for the test input audio ‘happy’ is below. 

![image](https://user-images.githubusercontent.com/73153277/125281273-a79f3c00-e333-11eb-9dcd-80a837a65c2a.png)


### Lessons learnt

           
* We used the peak detection  as the speech feature that resulted in the poor accuracy.

* Also, Peak detection works for single person speech. 

* During the peak detection  method, we learnt about the HMM model and using the speech features in HMM to predict the speech. 

* We learned about using the libraries related to speech and its implementation methodologies.




 



