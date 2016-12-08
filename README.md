In the Analysis notebook I am trying to beat the accuracy on a P300 speller test data that was provided as part of a competition several years ago. 

Here is a layman's explanation of the dataset. It is described in more detail in the below references: 

Two subjects wear a device with multiple electrodes on their head and stare at a 6 by 6 table of letters and numbers shown on a screen. The subject is tasked with spelling out a certain phrase using his brain. The rows and columns of the table are randomly highlighted and the subject counts the number of highlights until the desired row or column (the one containing the target letter) is flashed. This technique has shown to elicit an observable signal using Electroencephalography (EEG). The signal is called P300 because it occurs roughly 300 milliseconds after the desired letter is highlighted.
 

This uses the BCI Comp III, Dataset # 2 from a P300 speller http://www.bbci.de/competition/iii/desc_II.pdf

The winning accuracy was 96.5%  http://www.bbci.de/competition/iii/results/#winners


I am using the processing flow and LDA model as a baseline taken from a Wyrm library example found at https://github.com/venthur/wyrm/blob/master/examples/ . I am then experimenting using Neural Networks to see if I can achieve a better result. So far I have only tried some MLP networks but I am thinking next I will try a convolutional network so that the spatial relationships in the data are preserved and modeled however this will require some work manipulating the raw signal data rather than the processed set that I am working on.





