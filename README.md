# Speech_Emotion_Recognition_MLP_LSTM

In this project, I have built a speech emotion recogniser.  For that I have trained simple Speech Emotion Recognizer that identifies human emotions from audio files. I have used Python, Sci-kit learn, librosa, and Keras. 
Firstly, I have loaded the data (Ravdess dataset). After that I have extracted features (MFCC) from it, and split it into training sets and testing sets. 
Then, I have initialized two models (MLP and LSTM) as emotion classifiers and trained them. Finally, I have calculated and compared accuracies of the two models.

Software Requirements 
Anaconda 64-bit 
Python 3.6.6

Python Libraries Used
TensorFlow GPU v2.1.0
Keras v.2.3.1
Numpy v1.18.1
MatPlotLib v2.2.3
Pandas v1.0.3
Os
Librosa v0.7.2
Wave
Scikit-learn v0.23.1

Dataset used: 

“Ryerson Audio Visual Database of Emotional Speech and Song”

I have used Speech sound only records (16bit, 48kHz .wav) from the “RAVDESS" dataset. This bit of the RAVDESS contains 1440 records: 60 preliminaries for every entertainer x 24 on-screen characters = 1440. The RAVDESS contains 24 expert on-screen characters “12 female” and “12 male”, vocalizing two lexically-coordinated explanations in a nonpartisan “North American”  inflection. Discourse feelings incorporates quiet, cheerful, miserable, furious, dreadful, shock, and nauseate articulations. Every articulation is created at two degrees of enthusiastic force (ordinary, solid), with an extra nonpartisan articulation.

Model 1 using MLP classifier : 

In the first model using MLP classifier.
I have split the dataset into training and testing sets. Training set is a subset to train a model. Test set is a subset to test the test model. 
I have defined a function train_test_split. It will split the array into arbitrary train and test subsets. 80% of data is prepared as the “training set”. The rest 20% is kept as “testing set”. 


Model 2 using LSTM:

In the second model I have used the LSTM classifier. I have chosen LSTM because it is a subset of recurrent neural network and is the one of the most powerful domain of RNN.
Neural Networks is an amazing procedure and is utilized for picture acknowledgment and numerous different applications. One of the confinement is that, there is no memory related with the model. Which is an issue for successive information, similar to content or time arrangement. 
RNN addresses that issue by including an input look which fills in as a sort of memory. So the past contributions to the model leave an impression. LSTM broadens that thought and by making both a present moment and a drawn out memory part. 
Subsequently, LSTM is incredible instrument for whatever has an arrangement. Since the significance of a word relies upon the ones that went before it. This prepared for NLP and account investigation to use Neural Networks.


I was successful in creating two Speech Emotion Recognition models. The first model was created using MLP classifier and gave an accuracy of 57.29.
The second model was created LSTM and gave a good accuracy of 92.88.
So we can conclude that the LSTM model gave a higher accuracy.


