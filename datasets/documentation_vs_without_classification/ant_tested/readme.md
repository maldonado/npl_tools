# Information of the dataset
Cross project validation

## Script call

`$ python generate_classification_files.py apache-ant apache-jmeter argouml jfreechart columba password `

## Train 
All documentation and without classification comments from ArgoUml, Apache Jmeter, JfreeChart and Columba

## Test

All documentation and without classification comments from Apache ant. 

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
trainFile = /Users/evermal/git/npl_tools/datasets/documentation_vs_without_classification/ant_tested/classified_seq.train
tolerance = 1e-4
1.maxNGramLeng = 4
testFile = /Users/evermal/git/npl_tools/datasets/documentation_vs_without_classification/ant_tested/classified_seq.test
sigma = 3
printClassifierParam = 200
displayedColumn = 1
intern = true
useClassFeature = true
1.binnedLengths = 10,20,30
1.useNGrams = true
Reading dataset from /Users/evermal/git/npl_tools/datasets/documentation_vs_without_classification/ant_tested/classified_seq.train ...
WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/documentation_vs_without_classification/ant_tested/classified_seq.train varies between 2 and 51
done [4.4s, 26234 items].
numDatums: 26234
numDatumsPerLabel: {DOCUMENTATION=49.0, WITHOUT_CLASSIFICATION=26185.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, DOCUMENTATION]
numFeatures (Phi(X) types): 95168 [CLASS, 1-Len-0-10, 1-#B-//?, 1-#-//??, 1-#B-//??, ...]

3967 examples in test set
Cls WITHOUT_CLASSIFICATION: TP=3967 FN=0 FP=0 TN=0; Acc 1.000 P 1.000 R 1.000 F1 1.000
Cls DOCUMENTATION: TP=0 FN=0 FP=0 TN=3967; Acc 1.000 P 1.000 R 1.000 F1 1.000
Accuracy/micro-averaged F1: 1.00000
Macro-averaged F1: 1.00000

8069 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |8039|0  |29 |1   |0.996|0.996|1.000|0.998|
|DOCUMENTATION:          |1   |29 |0  |8039|0.996|1.000|0.033|0.065|

Accuracy/micro-averaged F1: 0.99641
Macro-averaged F1: 0.53136
