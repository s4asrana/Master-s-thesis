# Master-s-thesis
The analysis in this thesis depends on the original code developed by Rana and her team, and which can be found here https://github.com/ranahanocka/MeshCNN/

The original code is developed for the classification and segmentation task on different datasets. The work is this thesis uses the multiclass classification task done on SHREC dataset, for studying and analysing the effects of different DL optimization algorithms on the training process of MeshCNN (a complex DL network). In the original code, Rana and her team uses the Adam algorithm for the training purpose. In this thesis, in addition to the Adam algorithm,  I uses various other algorithms namely, SGD, SGD with Momentum, NAG, AdaGrad, and RMSprop, to study and do comparative analysis of their behaviour.

To switch among various algorithms, go to models --> mesh_classifier.py in here https://github.com/ranahanocka/MeshCNN/ and make appropriate changes from line 38 in the .py file, as shown in the Switch_Algo.png.
After switching to differnt algorithms, text files can be extracted from the checkpoints --> shrec16 --> loss_log.txt or testacc_log.txt file. This checkpont folder is available only after downloading and importing all the packages and dependencies necessary to make MeshCNN work on your local system. The text files loss_log.txt and testacc_log.txt contain information that is necessary for plotting various graphs (for different algorithms).

loss-graphs.ipynb contains the code to extract the information and plot the loss graphs for all the algorithms except for SGD with Momentum (600 epochs).
Similarly, graphs-for-momentum-600.ipynb contains the loss graph and test accuracy graph for SGD with Momentum (600 epochs).
test-accuracy-graphs.ipynb contains the test accuracy graphs for all algorithms when trained upto 200 epochs (except for NAG).
Finally, test-accuracy-graphs-nag-nag-600-adagrad-600 has the test accuracy graphs for NAG (200 epochs), NAG (600 epochs) and AdaGrad (600 epochs)

The text files data folder contains all the text files used in the .ipynb files in this work.
