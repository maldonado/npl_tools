# Information of the dataset
Cross project validation

## Script call

`$ python generate_classification_files.py apache-jmeter jfreechart apache-ant argouml columba password `

## Train 
All implementation and without classification comments from Apache Ant, ArgoUml, JfreeChart and Columba

## Test

All implementation and without classification comments from Apache Jmeter. 

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

WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/jmeter_tested/classified_seq.train varies between 2 and 51
done [4.3s, 23295 items].

numDatums: 23295
numDatumsPerLabel: {WITHOUT_CLASSIFICATION=22469.0, IMPLEMENTATION=826.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, IMPLEMENTATION]

7705 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |7674|9  |8  |14  |0.998|0.999|0.999|0.999|
|IMPLEMENTATION:         |14  |8  |9  |7674|0.998|0.609|0.636|0.622|

Accuracy/micro-averaged F1: 0.99779
Macro-averaged F1: 0.81056
