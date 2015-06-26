# Information of the dataset
Cross project validation

## Script call

`$ python generate_classification_files.py jfreechart apache-ant apache-jmeter argouml columba password `

## Train 
All defect and without classification comments from Apache Ant, Apache Jmeter, ArgoUml and Columba

## Test

All defect and without classification comments from Jfreechart. 

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
.usePrefixSuffixNGrams = true
QNsize = 15
useQN = true
goldAnswerColumn = 0
1.minNGramLeng = 1
trainFile = /Users/evermal/git/npl_tools/datasets/defect_vs_without_classification/jfreechart_tested/classified_seq.train
tolerance = 1e-4
1.maxNGramLeng = 4
testFile = /Users/evermal/git/npl_tools/datasets/defect_vs_without_classification/jfreechart_tested/classified_seq.test
sigma = 3
printClassifierParam = 200
displayedColumn = 1
intern = true
useClassFeature = true
1.binnedLengths = 10,20,30
1.useNGrams = true
Reading dataset from /Users/evermal/git/npl_tools/datasets/defect_vs_without_classification/jfreechart_tested/classified_seq.train ...
WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/defect_vs_without_classification/jfreechart_tested/classified_seq.train varies between 2 and 51
done [4.7s, 26128 items].
numDatums: 26128
numDatumsPerLabel: {WITHOUT_CLASSIFICATION=25953.0, DEFECT=175.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, DEFECT]
numFeatures (Phi(X) types): 100649 [CLASS, 1-#-*, 1-#E- */, 1-#-tuff, 1-#-en, ...]

4208 examples in test set
Cls WITHOUT_CLASSIFICATION: TP=4196 FN=3 FP=9 TN=0; Acc 0.997 P 0.998 R 0.999 F1 0.999
Cls DEFECT: TP=0 FN=9 FP=3 TN=4196; Acc 0.997 P 0.000 R 0.000 F1 0.000
Accuracy/micro-averaged F1: 0.99715
Macro-averaged F1: 0.49929

8166 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |7950|89 |68 |59  |0.981|0.992|0.989|0.990|
|DEFECT:                 |59  |68 |89 |7950|0.981|0.399|0.465|0.429|

Accuracy/micro-averaged F1: 0.98077
Macro-averaged F1: 0.70966
