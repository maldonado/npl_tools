# Information of the dataset
Cross project validation

`$ python generate_classification_files.py columba apache-ant apache-jmeter argouml jfreechart password `

## Train 
All implementation and without classification comments from Apache Ant, Apache Jmeter, JfreeChart and ArgoUml

## Test

All implementation and without classification comments from Columba. 

## Parameters
###Features

useClassFeature=true
1.useNGrams=true
1.usePrefixSuffixNGrams=true
1.maxNGramLeng=4
1.minNGramLeng=1
1.binnedLengths=10,20,30

###Printing

printClassifier=HighWeight
printClassifierParam=200

###Mapping

goldAnswerColumn=0
displayedColumn=1

###Optimization

intern=true
sigma=3
useQN=true
QNsize=15
tolerance=1e-4

## Results
1.usePrefixSuffixNGrams = true
QNsize = 15
useQN = true
goldAnswerColumn = 0
1.minNGramLeng = 1
trainFile = /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/columba_tested/classified_seq.train
tolerance = 1e-4
1.maxNGramLeng = 4
testFile = /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/columba_tested/classified_seq.test
sigma = 3
printClassifierParam = 200
displayedColumn = 1
intern = true
useClassFeature = true
1.binnedLengths = 10,20,30
1.useNGrams = true
Reading dataset from /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/columba_tested/classified_seq.train ...
WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/columba_tested/classified_seq.train varies between 2 and 23
done [5.1s, 24602 items].
numDatums: 24602
numDatumsPerLabel: {WITHOUT_CLASSIFICATION=23888.0, IMPLEMENTATION=714.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, IMPLEMENTATION]
numFeatures (Phi(X) types): 96608 [CLASS, 1-#-*, 1-#E- */, 1-#-tuff, 1-#-en, ...]

6398 examples in test set
Cls WITHOUT_CLASSIFICATION: TP=6252 FN=12 FP=9 TN=125; Acc 0.997 P 0.999 R 0.998 F1 0.998
Cls IMPLEMENTATION: TP=125 FN=9 FP=12 TN=6252; Acc 0.997 P 0.912 R 0.933 F1 0.923
Accuracy/micro-averaged F1: 0.99672
Macro-averaged F1: 0.96042

8690 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |7918|121|139|512 |0.970|0.983|0.985|0.984|
|IMPLEMENTATION:         |512 |139|121|7918|0.970|0.809|0.786|0.798|

Accuracy/micro-averaged F1: 0.97008
Macro-averaged F1: 0.89068
