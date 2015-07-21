# Information of the dataset
Cross project validation

## Train 
All implementation and without classification comments from Apache Ant, Apache Jmeter, JfreeChart and Columba

## Test

All implementation and without classification comments from ArgoUml. 

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

WARNING: Number of tab-separated columns in /Users/evermal/git/npl_tools/datasets/implementation_vs_without_classification/argo_tested/classified_seq.train varies between 2 and 51
done [3.4s, 22310 items].

numDatums: 22310
numDatumsPerLabel: {WITHOUT_CLASSIFICATION=22113.0, IMPLEMENTATION=197.0}
numLabels: 2 [WITHOUT_CLASSIFICATION, IMPLEMENTATION]


8690 examples in test set

|Classification          | TP |FN |FP |TN  |ACC  | P   |  R  | F1  |
|------------------------|----|---|---|----|-----|-----|-----|-----|
|WITHOUT_CLASSIFICATION: |7918|121|139|512 |0.970|0.983|0.985|0.984|
|IMPLEMENTATION:         |512 |139|121|7918|0.970|0.809|0.786|0.798|

Accuracy/micro-averaged F1: 0.97008
Macro-averaged F1: 0.89068
