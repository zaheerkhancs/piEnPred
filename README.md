# piEnPred
A Bi-Layered Model for Prediction of Enhancers and their Sub Types.
# A Brief
piEnhPred model make use of k-mer, CKSNAP, DCC, PseDNC, PseKNC as a feature extraction technique and SVM  as the dominant classification algorithm.The proposed approach use a novel method of Cascade Multi-Level feature selection method. The techniques works over three different values of threshold, 0.03, 0.05 and 0.07 to select top most optimum featuers from a different primitive features. The 1st layer discriminates a given Enhancer sequence, if the query sequence is predicted as Enhancer then the 2nd Layer tries to predicts their types (strong enhance or weak enhancer)
## Getting Started

Following are list of todo, before making run of the propose model.

### Prerequisites
#####  Following are the lib need to be installed....
What things you need to install the software and how to install them
- python3.6  [follow](https://www.python.org/downloads/release/python-367/)
- keras 2.2.4 [follow](https://keras.io/)
- Flask 1.0.2 [follow](http://flask.pocoo.org/docs/0.12/installation/)
- scikit-learn 0.19.1 [follow](https://scikit-learn.org/stable/install.html)
- scipy 1.1.0 [follow](https://scipy.org/install.html)
- numpy1.15.4 [follow](https://docs.scipy.org/doc/numpy/user/install.html)
- matplotlib3.0.2 [follow](https://matplotlib.org/users/installing.html#building-on-windows/)
- tensorflow 1.12.0 [follow](https://www.tensorflow.org/hub/installation)

```
$pip install <lib_name>
```

### Evaluate a model.

```
EvaluateModel.py
```
EvaluateModel.py is used for Evaluating a pre-trained model, stored for each successive layeres 1&2.


### Making prediction.

```
ModelPrediction.py
```
ModelPrediction.py is used to use to Obtained class probibilities for successive Layeres 1&2 on feeding and unseen Fasta Sequence or Sequence File.



# Also Cite
- Z. U. Khan, D. Pi et al, “iRSpot-SPI: Deep learning-based recombination spots prediction by incorporating secondary sequence information coupled with physio-chemical properties via Chou’s 5-step rule and pseudo components,” Chemom. Intell. Lab. Syst., 2019.

- Z. U. Khan, F. Ali, I. Ahmad, M. Hayat, and D. Pi, “iPredCNC: Computational prediction model for cancerlectins and non-cancerlectins using novel cascade features subset selection,” Chemom. Intell. Lab. Syst., vol. 195, p. 103876, 2019.

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Inspiration
* etc.. Thanks to Professor.Pi for his Constructive Commments throughout all stages of this Paper.
