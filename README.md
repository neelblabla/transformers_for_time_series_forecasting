# Multivariate Long Sequence Time-Series Forecasting with SOTA Transformers

We reproduce results from the following papers that introduced two special state-of-the-art transformer architectures for forecasting long sequence time-series data:- 

1) PatchTST - "A Time Series is Worth 64 Words: Long-term Forecasting with Transformers" (https://doi.org/10.48550/arXiv.2211.14730)
2) Informer - "Expanding the prediction capacity in long sequence time-series forecasting" (https://doi.org/10.1016/j.artint.2023.103886) + (https://doi.org/10.48550/arXiv.2012.07436)

Objective:  To harness the power of Transformer models for multivariate time series forecasting with a focus on improved efficiency and accuracy.

Details of the implementation are documented in the PDF report (Multivariate_Long_Sequence_Time-Series_Forecasting_with_SOTA_Transformers.pdf) made available in the repo.

### Results:
The results obtained in our implementation are presented below aside to their counterparts listed in the PatchTST introduction paper of 2023. 

![image](https://github.com/neelblabla/transformers_for_time_series_forecasting/assets/114079228/0ddc430c-a130-4a60-825d-0d1220a76e27)

As evident, our model implementations managed to reproduce results in close proximity of the ones produced by the authors of ‘PatchTST’ and ‘Informer’ for some datasets. In the case of Informer, the average deviance from the results obtained in the paper only amounts to 0.13 for MSE and 0.07 for MAE; while in case of PatchTST this is about 0.132 for MSE and 0.126 for MAE. Our implementation of PatchTST relies on a scaled-down architecture compared to the one featured in the original paper, primarily due to computational constraints. An intriguing insight gained from our experiments is that an increase in model size to a certain value does not consistently lead to lower MSE and MAE values respectively. Instead, it suggests that further augmenting the model's size may be necessary to achieve improved performance, which had computational constraints in our case.

Weights and Biases link for visualizations:
https://wandb.ai/kirteshpatel98/transformer_timeseries

### Instruction for Demo:
Before running the code please clone the OG time series repository into the patch-tst folder to import the model architecture.
```
git clone https://github.com/yuqinie98/PatchTST
```

Install dependent packages:
```
conda env create -n myenv -f transformer_timeseries.yml
```        



