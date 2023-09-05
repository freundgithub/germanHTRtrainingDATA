# germanHTRtrainingDATA
**German version below.

Handwriting text recognition (HTR) as a deep learning task requires images of handwriting samples from different writers. Of course, there are many open source projects with training data for HTR tasks in different languages (like [IAM](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database), [CVL](https://cvl.tuwien.ac.at/research/cvl-databases/an-off-line-database-for-writer-retrieval-writer-identification-and-word-spotting/) etc.), 
but not a specific German database with all German characters (like Ä, ä, Ö, ö, Ü, ü and ß). 
For example: In an application to recognise handwritten answers to open-ended questions in paper and pencil questionnaires (PAPI) from German respondents, a [HTR software](https://github.com/githubharald/SimpleHTR/blob/master/README.md) can't recognise German-specific characters without special training. Multiple results are possible.

![false-recog-overview](https://github.com/freundgithub/germanHTRtrainingDATA/assets/144004963/ef42db1c-c1a9-424c-9346-21307e11e14c)


Therefore, for my master's thesis, I collected a small sample of 3,349 handwritten images from 288 writers from a set of 650 different German professional terms to correctly recognise German-specific characters. 

![correct-recog-orview](https://github.com/freundgithub/germanHTRtrainingDATA/assets/144004963/c2d899b2-83ba-4cd0-9e51-ebdc4a54b272)





# Available training data and pre-trained models:

Since more training data is even better, in my master thesis I combined the databases [kaggle](https://www.kaggle.com/datasets/vaibhao/handwritten-characters), [IAM](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database), [CVL](https://cvl.tuwien.ac.at/research/cvl-databases/an-off-line-database-for-writer-retrieval-writer-identification-and-word-spotting/), [MNIST](http://yann.lecun.com/exdb/mnist/) and the featured handwritten images of German occupational terms to slightly increase the recognition rate. The best pre-trained models are available in "line mode" (CER = 13.16%; WER = 20.17%) and "word mode" (CER = 12.37%; WER = 71.36%). When OCR predestined images (such as Kaagle or MNIST) are used for training, the error rates increase, but the empirical error rates decrease.

+ [Pretrained model for single word images (word mode)](https://drive.google.com/file/d/1xjkbVVRFC6yLFxsMP-9bhWJnOjVN7eZ0/view?usp=drive_link)

+ [Pretrained model for text line images (line mode)](https://drive.google.com/file/d/1j4R6E-KOYImYxOtKcfqACuH9uF8EdKV9/view?usp=drive_link)

+ [Datset of the terms of occupation](https://drive.google.com/file/d/1kfe0HKE5MY3UFjCdn6iF3H8EXeXJw-ki/view?usp=drive_link)


### Format of Data: 

For easy implementation with the popular IAM database, the terms of the German occupational data are prepared like the IAM database in the form of an ordner structer and a ground thruth text file. The metadata of the positional arguments of the bounding box, the word transcription and the grammatical tag are placeholders and don't represent the real value.

## Future work

Adding more data with the already missing german specific letters (like Ö and ß). 




# German Version: 

Handwritten Text Recognition (HTR) als Aufgabenbereich des deep learnings benötigt Trainingsbilder von unterschiedlichen Schreibern. Natürlich gibt es einige frei zugängliche Projekte, die HTR-Trainingsdaten bereitstellen (darunter [IAM](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database), [CVL](https://cvl.tuwien.ac.at/research/cvl-databases/an-off-line-database-for-writer-retrieval-writer-identification-and-word-spotting/) usw.), aber keine Datenbank weißt alle Buchstaben der deutschen Sprache auf (dazu gehören Ä, ä, Ö, ö, Ü, ü und ß).
Ein Anwendungsbeispiel: In der Surveyforschung erspart die automatische Handschriftenerkennung von die Befragungsantworten offener Angaben in Paper and Pencil Fragebögen die manuelle Eingabe von sog. Encodern. Eine [Erkennungssoftware](https://github.com/githubharald/SimpleHTR/blob/master/README.md), die nicht auf die deutschen Buchstaben trainiert ist, kann diese Buchstaben nicht erkennen. Mehrere Fehlerquellen sind möglich. 

Für diesen Fall habe ich während meiner Masterarbeit einen kleinen Datensatz von 3.349 Trainingsbildern von insgesamt 288 Schreibern erstellt, um explizit auch deutsche Buchstaben automatisch erfassen zu können. 




# Verfügbare Trainingsdaten und vortrainierte Modelle:

Da aus einem Mehr an Trainingsdaten, bessere Ergebnisse erzielt werden können, habe ich für meine Masterarbeit mehrere Modelle anhand der Datenbanken [kaggle](https://www.kaggle.com/datasets/vaibhao/handwritten-characters), [IAM](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database), [CVL](https://cvl.tuwien.ac.at/research/cvl-databases/an-off-line-database-for-writer-retrieval-writer-identification-and-word-spotting/), [MNIST](http://yann.lecun.com/exdb/mnist/) und den hier vorgestellten Berufs-Trainingsdaten trainiert, um die Erkennungsrate geringfügig zu verbessern. Die besten Modelle sind im "line-mode" (CER = 13,16%; WER = 20,17%) und "word-mode" (CER = 12,37%; WER = 71,36%) verfügbar. Werden Modelle mit OCR prädestinierten Daten (d.h. mit Bildern einzelner Charaktere wie kaggle, MNIST) trainiert, verschlechtern sich die WER-/CER-Fehlerraten, aber die empirische Erkennungsrate steigt. 

+ [Trainiertes Modell im word-mode für einzelne Wörter](https://drive.google.com/file/d/1xjkbVVRFC6yLFxsMP-9bhWJnOjVN7eZ0/view?usp=drive_link)

+ [Trainiertes Modell im line-mode für mehrere Wörter in einer Zeile](https://drive.google.com/file/d/1j4R6E-KOYImYxOtKcfqACuH9uF8EdKV9/view?usp=drive_link)

+ [Trainingsdaten der Berufsbezeichnungen](https://drive.google.com/file/d/1kfe0HKE5MY3UFjCdn6iF3H8EXeXJw-ki/view?usp=drive_link)


### Datenformat: 

Die Trainingsdaten sind im Format der IAM-Datenbank erstellt, sodass sie sich einfach in diese Trainingsdaten integrieren lassen. Die Metadaten zur Transkription, Bounding-Box Position usw. sind als Platzhalter eingefügt und entsprechen nicht den tatsächlichen Werten.
