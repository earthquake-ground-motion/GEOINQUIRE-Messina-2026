<p align="middle">
    <a title='EFEHR' href='https://github.com/earthquake-ground-motion/GEOINQUIRE-Messina-2026/blob/update_17042026/logos/efehr_logo.png'></a>
    &nbsp;
    <a title='GFZ' href='https://github.com/earthquake-ground-motion/GEOINQUIRE-Messina-2026/blob/update_17042026/logos/GFZ_logo.png'></a>
    &nbsp;
    <a title='GEO-INQUIRE' href='https://github.com/earthquake-ground-motion/GEOINQUIRE-Messina-2026/blob/update_17042026/logos/Geo-INQUIRE_logo.jpg'></a>
    <br>
</p>

# GEOINQUIRE-Messina-2026
Repository containing Jupyter notebooks and data to demonstrate the EFEHR Earthquake Catalogue Web service and eGSIM Webservice at the GEO-INQUIRE Workshop in Messina, Italy, April 2026

## Webservices

### European Mediterranean Earthquake Catalogue (EMEC)

URL: https://emec.gfz.de

Citation:

> Lammers, Steffi; Weatherill, Graeme; Grünthal, Gottfried; Cotton, Fabrice (2023):
EMEC-2021 - The European-Mediterranean Earthquake Catalogue – Version 2021. GFZ Data Services. https://doi.org/10.5880/GFZ.EMEC.2021.001

### European Preinstrumental Earthquake Catalogue (EPICA)

URL: https://www.emidius.eu/epica/

Citation:

> Rovida A., Antonucci A. (2021). EPICA - European PreInstrumental Earthquake CAtalogue, version 1.1 [Dataset]. Istituto Nazionale di Geofisica e Vulcanologia (INGV). https://doi.org/10.13127/epica.1.1

> Rovida A., Antonucci A., Locati M. (2022). The European Preinstrumental Earthquake Catalogue EPICA, the 1000–1899 catalogue for the European Seismic Hazard Model 2020. Earth System Science Data. https://doi.org/10.5194/essd-14-5213-2022

### eGSIM Online Ground Shaking Intensity Model Service

URL: https://egsim.gfz.de

Citation:

> Zaccarelli, Riccardo; Weatherill, Graeme (2020): eGSIM - a Python library and web application to select and test Ground Motion models. GFZ Data Services. https://doi.org/10.5880/GFZ.2.6.2023.007

> Zaccarelli, R., Weatherill, G., Bindi, D., Cotton, F. (2026 online): Ground-Motion Models at Your Fingertips: Easy, Rapid, and Flexible Analysis with eGSIM. - Seismological Research Letters. https://doi.org/10.1785/0220250228

### Engineering Strong Motion Database

URL: https://esm-db.eu

Citation:

> Mascandola C., Felicetta C., Russo E., Luzi L., Lanzano G., Sgobba S., Brunelli G., Ramadan F., Pacor F., ORFEUS Strong-Motion SMC (2026). Engineering Strong Motion Database (ESM), version 3.0. Istituto Nazionale di Geofisica e Vulcanologia (INGV). https://doi.org/10.13127/esm.3

## Installation & Setup

[_Use a virtual environment_](https://docs.python.org/3/library/venv.html) with the following dependencies:

```
>$ pip install requests obspy h5py tables pandas geopandas jupyter
```

For Mac users with HDF5 installed via brew:

```
>$ pip install requests obspy h5py jupyter

>$ env HDF5_DIR=/opt/homebrew/Cellar/hdf5/#.##.# pip install tables pandas geopandas
```

To download the notebook repository, either click on the "Code" button and select "Download Zip", then move and unzip the contents to an appropriate place on your workstation.

Alternatively, the repository can be cloned via Git on the command line if it is installed on your system:

```
>$ git clone https://github.com/earthquake-ground-motion/GEOINQUIRE-Messina-2026.git
```

Once downloaded then enter the folder and begin a Jupyter Lab session

```
>$ cd GEOINQUIRE-Messina-2026
>$ jupyter lab
```

One notebook shows how to execute a large scale waveform download query from the ESM Webservice. This is shown for illustrative purposes, but we _strongly_ discourage running this during the workshop. Instead users can download the waveform outputs directly from here: https://nextcloud.gfz.de/s/2PNS3gbfCxirF5q


The waveforms are contained in the folder `esm_waveforms`, which should be placed in the directory path `/notebooks/data`.



## Acknowledgements

The notebooks were created by:
> Graeme Weatherill
> 
> GFZ Helmholtz Centre for Geosciences
> 
> Potsdam, Germany
>
> graeme.weatherill[at]gfz.de 

Additional contributions from:
> Elif Türker (GFZ)
> 
> Riccardo Zaccarelli (GFZ)

The notebooks are provided free for use via a GNU General Public License v 3.0

> © Geo-INQUIRE Consortium 2023-2026 | 
> Geo-INQUIRE is funded by the European Commission under project number 101058518 > within the HORIZON-INFRA-2021-SERV-01 call.