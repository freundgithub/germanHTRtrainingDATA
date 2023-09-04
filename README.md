# germanHTRtrainingDATA
**German version below.

Introduction:

Handwritten Text Recognition (HTR) as a task of deep learning needs images of handwritten samples from different writers. Of course, there are many open source projects with training data for HTR tasks in different languages (like RIMES, IAM, CVL etc.), 
but not a specific german database with all german specific letters (like Ä, ä, Ö, ö, Ü, ü and ß). 
For example: In a scope of application of recognizing handwritten answers from open-ended-questions in paper and pencil questionnaires (PAPI) from german respondents a HTR-software (like HTR-scheidl) can't recognize german specific letters without 
specific training. Multiple outcomes are possible.

![false-recog-overview](https://github.com/freundgithub/germanHTRtrainingDATA/assets/144004963/ef42db1c-c1a9-424c-9346-21307e11e14c)


Therefore, due my master thesis i collected a small sample of 3,349 handwritten images from 288 writers from an amount of 650 different german terms of occupations to recognize german specific letters correctly. 

![correct-recog-orview](https://github.com/freundgithub/germanHTRtrainingDATA/assets/144004963/c2d899b2-83ba-4cd0-9e51-ebdc4a54b272)


Format of Data: 

For an easy implemantation with the pupular IAM database, the terms of german occupational data is prepared like the IAM database in form of ordner structer and ground thruth text file. (Hier noch beschrieben, dass die nur die GT-Daten und der Filename relevant ist.) The single german terms of occupational data is downloadable from [...]. 



Available trainingsdata and pretrained models:

Because, more training data is even better, in my master thesis i put the databases kaggle, IAM, CVL, MNIST together to slightly increase the recognizion rate. With this summarized training data you doesn't need to restart the training to add an additional dataset. 


German Version: 

Handwritten Text Recognition (HTR) als Aufgabenbereich des deep learnings benötigt Trainingsbilder von unterschiedlichen Schreibern. Natürlich gibt es einige frei zugängliche Projekte, die HTR-Trainingsdaten bereitstellen (darunter RIMES, IAM, CVL usw.), aber keine Datenbank weißt alle Buchstaben der deutschen Sprache auf (dazu gehören Ä, ä, Ö, ö, Ü, ü und ß).
Ein Anwendungsbeispiel: In der Surveyforschung erspart die automatische Handschriftenerkennung von die Befragungsantworten offener Angaben in Paper and Pencil Fragebögen die manuelle Eingabe von sog. Encodern. Eine Erkennungssoftware, die nicht auf die deutschen Buchstaben trainiert ist, kann diese Buchstaben nicht erkennen. Mehrere Fehlerquellen sind möglich. 

Für diesen Fall habe ich während meiner Masterarbeit einen kleinen Datensatz von 3.349 Trainingsbildern von insgesamt 288 Schreibern erstellt, um explizit auch deutsche Buchstaben automatisch erfassen zu können. 


Fromat der Daten: 




Verfügbare Trainingsdaten und vortrainierte Modelle:

Da aus einem Mehr an Trainingsdaten, bessere Ergebnisse erzielt werden können, habe ich für meine Masterarbeit mehrere Modelle anhand der Datenbanken kaggle, IAM, CVL, MNIST und den hier vorgestellten Berufs-Trainingsdaten trainiert, um die Erkennungsrate geringfügig zu verbessern. Diese besten Modelle sind im "line-mode" (CER = XX,XX%; WER = XX,XX%) und "word-mode" (CER = XX,XX%; WER = XX,XX%) verfügbar. 

