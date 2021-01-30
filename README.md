# ICTOS
This repository is the code of ICTOS related to an ISSTA 2021 submission.
In this repository, the code to repeat the experiments on MNIST and CIFAR10 is available.

The python code in MNISTCNNs.py and CIFAR10CNNs.py can be executed to generate the .csv files containing the training, validation, and test sets ready to be submitted to ICTOS. All the requirements needed to execute the Python code are listed in the requirements.txt file.

The implementation of ICTOS provideed need an installation of KNIME (v4.0.0).
After the import of the .knar file into KNIME workspace the .csv file generated can be inserted in input in the "CSV Reader" blocks according to their tags.
With the "Double Configuration" blocks the minimum confidence and support can be setted.
The "CSV Writer" blocks can be configured with the path where the CSV containing the output of the testing session can be saved.
The "Java Snippet" block, named "IDI", inside the "ICTOS" metanode can be used to switch the partitioning criterion uncommenting the corresponding code.
The "Partitioning" blocks, "Node 15" and "Node 77" (inside "CRO" metanode), can be used to change the test set size for ICTOS and CRO respectively. 
