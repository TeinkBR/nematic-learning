# nematic-learning
<p align="center">
<img src="logo.png" width=50% height=50%>
</p>

---
This repository contains all the scripts used to generate and analyze the data in the paper  "Machine Learning Microscopic Form of Nematic Order in twisted double-bilayer graphene (2023)" arxiv: .

Zenodo Link:

Authors: Simon Eli Turkel ([@sturk111](https://www.github.com/sturk111)), Abhay Pasuphaty (Columbia University), Stefan Obernauer ([@stefob](https://www.github.com/stefob)), João Augusto Sobral and Mathias S. Scheurer (University of Innsbruck).

 Install the dependencies: `pip install -r requirements.txt`, and `Python 3.9.10`.
#### Continuum model for tDBG
1. TDBG.py is a variation of [pytwist](https://github.com/sturk111/pytwist) that contains the GN and MN couplings. For further documentation we refer 
to the original repository - that goes beyond tDBG by including other moiré heterostructures.

 
#### Toy model for TBG

2. Files for the investigations in Appendix D can be found in the folder `app_d` and some auxiliary *Mathematica* notebooks in `minimalmodel/matnb`.
#### Information about the experimental $D_{\text{exp}}$ and theoretical $D_{\text{th}}$ datasets

3. The raw data for the experimental dataset $D_{\text{exp}}$ can be found in the folder `expdata`. To see how you can access and preprocess it, take a look 
at `expdata_preprocessing.py`.
4. All test datasets and corresponding trained model files .h5 to reproduce the plots in the paper can be found in the Zenodo link.

The train/val datasets are bigger (TD: Remove this sentence if we upload everything to Zenodo), and we only present the one for Sec. 4. Alternative theoretical datasets can be  easily generate via the script `gendata/mpsingle.py`. 

5. Auxiliary scripts can be found in the folder `utils`. These consist of options to concatenate datasets generated by `mpsingle.py`, map the 
current labels to different ones (such as $\beta =\{\varphi\} \rightarrow \beta^{\prime} = \{\sin\left(\varphi\right), \cos\left(\varphi\right)\}$), and just  check the dimensions of 
the `npz` files.


Note: Codes will be eventually refactored for better readability.

