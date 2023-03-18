General workflow of mass downloading seismic data and preprocessing.
################################

***step0***
Download the earthquake catalog, i.e., the location of earthquakes 
including the longitude, latitude, depth and magnitude.

***step1***
Download the list of seismic stations, i.e., the location of stations 
including the longitude, latitude and height.

***step2***
Make the plot to show the distribution of earthquakes and seismic stations in our study 
region.

***step3***
Download the seismic waveforms from available seismic networks in our study region. 
The downloaded data are in format of miniseed, and we will transform it into 
the format of SAC, which is more convenient for us to deal with.

***step4***
Transform the seismic data in format of miniseed into SAC.

***step5***
Filter the seismic waveforms to the frequency periods of our interest.

***step6***
Select the seismic waveforms with high quality using the metric of the signal-to-noise 
ratio (SNR).

***step7***
Rotate the ENZ/12Z-coordinate data into RTZ-coordinate.

***step8***
Quickly check whether the waveform is good for the further depth-phase verification.

***step9***
Formally verification of depth phase, using amplitude partition on 3-component waveforms, 
particle motion analysis and dominant frequency of P and candidate sP.



##################################
Some needed softwares shall be installed on your computer, e.g., Ubuntu system.
***
Anaconda python @ https://docs.anaconda.com/anaconda/install/linux/
***
Jupyter Notebook or Lab @ https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html
***
PyGMT @ https://www.pygmt.org/latest/install.html   ,     https://github.com/MIGG-NTU/PyGMT2021
***
Obspy @ https://anaconda.org/conda-forge/obspy
***
SAC (seismic analysis code) @ http://ds.iris.edu/ds/nodes/dmc/forms/sac/  ,  https://seiscode.iris.washington.edu/projects/sac/wiki/Binary_Installation

Other useful link:
General introduction of seismology @ https://seismo-learn.org/seismology101/seismology/introduction/ (in Chinese)
Popular data format of seismic records @ https://seismo-learn.org/seismology101/seismology/data-format/ (in Chinese)
Introduction of seismic data @ https://github.com/MIGG-NTU/SeisData_Tools/blob/main/workshops/SeisTomo_Tutoriala_DATA/data-analysis/data-analysis.ipynb
Fetching data from seismic network @ https://github.com/MIGG-NTU/SeisData_Tools/blob/main/workshops/SeisTomo_Tutoriala_DATA/data-fetch/data-fetch.ipynb
