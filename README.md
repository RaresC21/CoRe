# CoRe: Coherency Regularization for Hierarchical Time Series

This repository implements the ideas in the paper "CoRe: Coherency Regularization for Hierarchical Time Series" and evaluates on three datasets. The paper is also attached in this repo.

For each dataset, we test both point forecasts and distributional forecasts. To run point forecast experiments, use the following command: 

``python run_point_forecast.py -d dataset_name``

where ``dataset_name`` can refer to one of: ``traffic``, ``tourism``, ``labor``

To run distributional forecast experiments, use the following command

``python run_distributional_forecast.py -d dataset_name``

These will generate plots showing the MSE, WMAPE, Coherency, and CRPS (only for distributional forecasts) at each level of the hierarchy for the given dataset. 

### Parameters

The config files ``config.yaml`` and ``distribution_config.yaml`` contain the parameter choices for each set of experiments. One can choose various hyperparameters, including network widths, learning rates, number of runs (times to repeat each experiment) and more.
