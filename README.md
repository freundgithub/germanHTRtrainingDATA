# germanHTRtrainingDATA
Handwritten Text Recognition (HTR) as a task of deep learning needs images of handwritten samples from different writers. Of course, there are many open source projects with training data for HTR tasks in different languages (like RIMES, IAM, CVL etc.), 
but not a specific german database with all german specific letters (like Ä, ä, Ö, ö, Ü, ü and ß). 
For example: In a scope of application of recognizing handwritten answers from open-ended-questions in paper and pencil questionnaires (PAPI) from german respondents a HTR-software (like HTR-scheidl) can't recognize german specific letters without 
specific training (upload picture for example).    
Therefore, due my master thesis i collected a small sample of 3,349 handwritten images from 288 writers from an amount of 650 different german terms of occupations. 


Format of Data: 
For an easy implemantation with the pupular IAM database, the terms of german occupational data is prepared like the IAM database in form of ordner structer and ground thruth text file. (Hier noch beschrieben, dass die nur die GT-Daten und der Filename relevant ist.) The single german terms of occupational data is downloadable from [...]. 


Extra bonus: 
Because, more training data is even better, in my master thesis i put the databases kaggle, IAM, CVL, MNIST together to slightly increase the recognizion rate. With this summarized training data you doesn't need to restart the training to add an additional dataset. 
