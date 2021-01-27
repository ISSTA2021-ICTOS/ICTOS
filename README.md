# ICTOS
This repository is the supplemental material related to a ISSTA 2021 submission.
In this repository, the code to repeat the experiments is available.
We reported the datasets to completely reproduce the experiments on MNIST.
The code to repeat the experiments on CIFAR10 is also available.

The python code in MNISTCNNs.py and CIFAR10CNNs.py can be executed to generate the .csv files containing the training, validation, and test sets ready to be submitted to ICTOS.

The implementation of ICTOS provideed need an installation of KNIME.
After the import of the .knar file into KNIME workspace the .csv file generated can be inserted in input in the "CSV Reader" blocks according to their tags.
With the "Double Configuration" blocks the minimum confidence and support can be setted.
The "CSV Writer" blocks can be configured with the path where the CSV containing the output of the testing session can be saved.