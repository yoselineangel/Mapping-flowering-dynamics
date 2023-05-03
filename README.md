# Mapping-flowering-dynamics
This repository comprises notebooks and files to perform a two-step framework for mapping and tracking flowering dynamics from hyperspectral datasets.

## Summary

A single pixel may contain several individual plants of different species, flowers, soil, and shadows with highly variable fractional coverage of the canopy area. You can find a Jupyter notebook comprising a two-step framework for mapping and tracking flowering dynamics from hyperspectral datasets:

- Spectral mixture residual analysis
- Unsupervised clustering based on the Gaussian mixture model (GMM)

We implemented the workflow on an open cloud computing environment (e.g., Amazon Web Service -AWS) that couples various Python libraries for imagery storage (e.g., Zarr), access (e.g., Intake), and managing multi-dimension arrays (e.g., Xarray), as described in (Lang et al., 2023). In addition, to perform the data analysis, we adapted the publicly available code posted by Sousa et al., 2022 to retrieve the mixture residual and the Gaussian Mixture module from the Scikit-learn library (Pedregosa et al., 2011) integrated with some visualization tools (e.g., hvPlot, Bokeh, matplotlib).

##References

Lang, E., Angel, Y., & Shiklomanov, A. N. (2023). SHIFT SMCE User Guide (v2.0.2). Zenodo. https://doi.org/10.5281/zenodo.7864544

Sousa, D., Brodrick, P., Cawse-Nicholson, K., Fisher, J. B., Pavlick, R., Small, C., & Thompson, D. R. (2022). The Spectral Mixture Residual: A Source of Low-Variance Information to Enhance the Explainability and Accuracy of Surface Biology and Geology Retrievals. Journal of Geophysical Research: Biogeosciences, 127(2), e2021JG006672. https://doi.org/10.1029/2021JG006672

Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., Blondel, M., Prettenhofer, P., Weiss, R., Dubourg, V., Vanderplas, J., Passos, A., Cournapeau, D., Brucher, M., Perrot, M., & Duchesnay, É. (2011). Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research, 12(85), 2825, https://doi.org/10.48550/arXiv.1201.0490
