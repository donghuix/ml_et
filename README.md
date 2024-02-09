# ml_et

1. data/test1 contains the training/validation data based on speperation of evaporation and transpiration.
    * xe.dat: input variables for Evaporation
    * ye.dat: Evaporation

    * xt.dat: input variables for Transpiration
    * yt.dat: Transpiration

    * xet.dat: input variables for ET
    * yet.dat: ET

2. data/test2 contains the training/validation data based on data spliting in time
    * xtrain.dat: input variables for the first 80% of the time
    * ytrain.dat: ET for the first 80% of the time

    * xval.dat, xtest.dat: input variables for the other 20% of the time
    * yval.dat, ytest.dat: ET for the other 20% of the time

3. data/mep contains the benchmard ET simulation with Maximum Entropy Production thoery
    * me.dat:  modeled evaporation using input of xe.dat in data/test1
    * mt.dat:  modeled transpiration using input of xt.dat in data/test1
    * met.dat: modeled ET using input of xet.dat in data/test1


Note: each column of input matrix represents a feature. Below is the header for each input matrix:
IGBP, NDVI, air temperature, net radiation, soil water content, nighttime temperature, daytime temperature, daytime temperature standard deviation, potential incoming shortwave radiation, incoming shortwave radiation, incoming longwave radiation, vapor pressure deficit, air pressure, precipitation, wind speed, friction velocity, outgoing shortwave radiation, outgoing longwave radiation, CO2 mole fraction, soil temperature

IGBP varies from 1 to 17, which corresponds to the following order:
['BSV','CRO','CSH','CVM','DBF','DNF','EBF','ENF','GRA','MF','OSH','SAV','SNO','URB','WAT','WET','WSA']
