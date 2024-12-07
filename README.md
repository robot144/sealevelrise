# sealevelrise
Some notebooks with computations around topic of sealevelrise

This repo starts building on this one: https://github.com/openearth/sealevel/tree/report/notebooks
It's about changes in the mean sealevel, mainly at the Dutch coast for now.

## Estimate for running year

It takes a bit of time before the official annual mean sealevel values become available. In the notebook `dutch_sealevels.ipynb` we compute an estimate from the operational database. This doesn't make any sense earlier in the year, but close to the end of the year, the last values are unlikely to change the mean a lot. Even after the end of the year differences with the official are possible because, the measurements undergo another validation, more values may be available outside the operational database, and the reference may be corrected by calibration.

- look at notebook in [nbviewer](https://nbviewer.ipython.org/github/robot144/sealevelrise/blob/main/dutch_sealevels.ipynb)

Here are the figures:

![vlissingen](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_vlissingen.png)
![hoekvanholland](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_hoekvanholland.png)
![ijmuiden](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_ijmuiden.png)
![denhelder](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_denhelder.png)
![harlinger](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_harlingen.png)
![delfzijl](https://raw.githubusercontent.com/robot144/sealevelrise/refs/heads/main/figures/series_delfzijl.png)