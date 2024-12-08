# Sealevel rise in the Netherlands

In the Netherlands, changes in the mean sealevel are tracked in the [zeespiegelmonitor](https://www.deltares.nl/expertise/onze-expertises/zeespiegelstijging/zeespiegelmonitor). The underlying observed annual mean sealevel values are taken from the [PSMSL database](https://psmsl.org/data/obtaining). The PSMSL collects monthly mean and annual mean sealevel data worldwide. Changes in the local reference, for example causes by subsidence or levelling updates, are compensated by translating values to a Revised Local Reference (RLR). This RLR has an offset with the current national NAP, that differs a bit per station. Rijkswaterstaat sends it's tide-gauge data to PSMSL every year after a thorough check of the data an possibly a correction based on recalibration of their instruments.

## Goals of this notebook

### An early estimate  of the annual mean

The process described above is thorough, but it's also slow. Updates in the zeespiegelmonitor tend to be published about a year after the end of the year. Here, we aim to make a rough estimate based on the raw measuerements, that become available a few minutes after the measurement is produced at the tide-gauge. This makes it possible to get a rough idea about the next value, even a bit before the end of the ongoing year.
Of course, these values are only rough estimates and both quality control and re-calibration can alter the values, it may be interesting to have a rough non official estimate much earlier. To assess the the impact of the quality control and re-calibration, a few overlapping years are collected.

- look at notebook in [nbviewer](https://nbviewer.ipython.org/github/robot144/sealevelrise/blob/main/dutch_sealevels.ipynb)

Here are the figures:

![vlissingen](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_vlissingen.png)
![hoekvanholland](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_hoekvanholland.png)
![ijmuiden](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_ijmuiden.png)
![denhelder](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_denhelder.png)
![harlinger](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_harlingen.png)
![delfzijl](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_delfzijl.png)

### Sealevel rise and global temperature

At longer times-cales, sealevel rise is claimed ([Dangendorf etal 2014](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1002/2014JC009901)) to be related to the changes in the surrounding ocean. Here, a simplistic link between the global mean temperature from [Copernicus Climate](https://climate.copernicus.eu/copernicus-2024-virtually-certain-be-warmest-year-and-first-year-above-15degc) These values were computed by averaging temperatures from the ERA5 reanalysis.

![Vlissingen with linear regression on global temperature](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_$(station)_including_regression_global_temperature.png)