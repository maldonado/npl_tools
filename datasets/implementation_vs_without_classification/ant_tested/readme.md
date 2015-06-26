# Information of the dataset
Cross project validation

## Script call

`$ python generate_classification_files.py apache-ant apache-jmeter argouml jfreechart columba password `

## Train 
All implementation and without classification comments from ArgoUml, Apache Jmeter, JfreeChart and Columba

## Test

All implementation and without classification comments from Apache ant. 

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

  -prop /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/ant_tested/dataset.prop
1.usePrefixSuffixNGrams = true
QNsize = 15
useQN = true
goldAnswerColumn = 0
1.minNGramLeng = 1
trainFile = /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/ant_tested/classified_seq.train
tolerance = 1e-4
1.maxNGramLeng = 4
testFile = /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/ant_tested/classified_seq.test
sigma = 3
printClassifierParam = 200
displayedColumn = 1
intern = true
useClassFeature = true
1.binnedLengths = 10,20,30
1.useNGrams = true
Reading dataset from /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/ant_tested/classified_seq.train ...
WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/ant_tested/classified_seq.train varies between 2 and 51
done [5.2s, 27017 items].
numDatums: 27017
numDatumsPerLabel: {WITHOUT_CLASSIFICATION=26185.0, IMPLEMENTATION=832.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, IMPLEMENTATION]
numFeatures (Phi(X) types): 96311 [CLASS, 1-Len-0-10, 1-#B-//?, 1-#-//??, 1-#B-//??, ...]

3983 examples in test set
Cls WITHOUT_CLASSIFICATION: TP=3965 FN=2 FP=11 TN=5; Acc 0.997 P 0.997 R 0.999 F1 0.998
Cls IMPLEMENTATION: TP=5 FN=11 FP=2 TN=3965; Acc 0.997 P 0.714 R 0.312 F1 0.435
Accuracy/micro-averaged F1: 0.99674
Macro-averaged F1: 0.71657

8690 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |7918|121|139|512 |0.970|0.983|0.985|0.984|
|IMPLEMENTATION:         |512 |139|121|7918|0.970|0.809|0.786|0.798|

Accuracy/micro-averaged F1: 0.97008
Macro-averaged F1: 0.89068
