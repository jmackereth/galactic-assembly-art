#  🌌 Galactic Assembly as Abstract Art

## Powered by [matplotlib](https://matplotlib.org), [numpy](https://numpy.org), [ipywidgets](https://github.com/jupyter-widgets/ipywidgets), [voilà](https://github.com/voila-dashboards/voila) and the [EAGLE Simulations](http://eagle.strw.leidenuniv.nl)

<img src="img/output.gif" width="400px">

This is an interactive version of a visualisation that I originally made for understanding how galaxies assemble in the evolving Universe of the EAGLE simulations ([Schaye et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.446..521S/abstract), [Crain et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.450.1937C/abstract)). In the Lambda-Cold Dark Matter (LCDM) model, the current 'standard' cosmological model, galaxies assemble hierarchically, building their mass over time through the merging of smaller galactic building blocks. In the LCDM model, this hierarchical assembly is mainly governed by the distribution of the cold dark matter in the very early universe, itself determined by the details of the events following the Big Bang. The EAGLE simulations simulate these events from just after the Big Bang, right out to the present day in a representative volume of a Universe. This visualisation shows the track of all of the simulation particles which eventually form into a galaxy with a similar mass, shape and size to our galaxy, the Milky Way - a relatively large disc galaxy. 

You can download and run the notebook or the voila dashboard locally, which will require you to also download the dataset from [here](https://zenodo.org/record/3866403/files/EAGLE_MW_trace_coords_downsampled_10.npy?download=1) and place it in the same directory. Use:
```
git clone https://github.com/jmackereth/galactic-assembly-art.git
cd galactic-assembly-art
wget -q -O EAGLE_MW_trace_coords_downsampled_10.npy "https://zenodo.org/record/3866403/files/EAGLE_MW_trace_coords_downsampled_10.npy?download=1"`)
voila notebook/galaxy-assembly-art.ipynb
```

Alternatively, you can use the binder/voila dashboard, at this link: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jmackereth/galactic-assembly-art/master?urlpath=%2Fvoila%2Frender%2Fnotebook%2Fgalaxy-assembly-art.ipynb)

Be warned, the binder version takes quite some time to build and render, as it has to download the large data file necessary for the visualisation then load it into memory... The dashboard is not as responsive as it probably could be, and takes a while to render the new image upon changing settings, but it's fun to experiment! Perhaps one day, i'll be able to make it nice and fast!
