# pastisML-tess
Code to produce simulated TESS lightcurves based on PASTIS

## Dependency
The package uses the PASTIS package

The main paper describing it is:

```
@ARTICLE{pastis,
       author = {{D{\'\i}az}, R.~F. and {Almenara}, J.~M. and {Santerne}, A. and
         {Moutou}, C. and {Lethuillier}, A. and {Deleuil}, M.},
        title = "{PASTIS: Bayesian extrasolar planet validation - I. General framework, models, and performance}",
      journal = {\mnras},
     keywords = {methods: statistical, techniques: photometric, techniques: radial velocities, planetary systems, Astrophysics - Earth and Planetary Astrophysics},
         year = "2014",
        month = "Jun",
       volume = {441},
       number = {2},
        pages = {983-1004},
          doi = {10.1093/mnras/stu601},
archivePrefix = {arXiv},
       eprint = {1403.6725},
 primaryClass = {astro-ph.EP},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2014MNRAS.441..983D},
      }
```
    
## Usage
Clone the current repo
```
git clone https://github.com/ckm3/pastisML-tess.git
```
Enter the folder
```
cd pastisML-tess/
```
Create an conda environment with the given environment.yml, and if you are going to install other packages with conda, make sure you are using conda-forge channel.
```
conda env create -f environment.yml
```
Activate the environment
```
conda activate pastis-env
```
Install pastis
```
cd ..
git clone https://github.com/ckm3/pastis.git
cd pastis
pip install -e .
```

Also download necessary lib files [https://storage.cuikaiming.com/share/pastis-lib.tar]([https://](https://storage.cuikaiming.com/share/pastis-lib.tar)) and put them under the lib folder of pastis.

The stellar sample file should contain the necessary columns listed in the main.py 
 