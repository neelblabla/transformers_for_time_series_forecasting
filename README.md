# transformers_for_time_series_forecasting

We reproduce results from the following papers that introduced two special transformer architectures for forecasting long sequence time-series data:- 

1) PatchTST - "A Time Series is Worth 64 Words: Long-term Forecasting with Transformers" (https://doi.org/10.48550/arXiv.2211.14730)
2) Informer - "Expanding the prediction capacity in long sequence time-series forecasting" (https://doi.org/10.1016/j.artint.2023.103886) + (https://doi.org/10.48550/arXiv.2012.07436)

The objective is to harness the power of Transformer models for multivariate time series forecasting with a focus on improved efficiency and accuracy.

Weights and Biases link for visualizations:
https://wandb.ai/kirteshpatel98/transformer_timeseries

## Instruction:
Before running the code please clone the OG time series repository into the patchTST folder to import the model architecture.
<div class="code-snippet">
    <button class="copy-button" onclick="copyCode(this)">Terminal</button>
    <pre>
        <code>
            git clone https://github.com/yuqinie98/PatchTST
        </code>
    </pre>
</div>

## Install dependent packages:
<div class="code-snippet">
    <button class="copy-button" onclick="copyCode(this)">Terminal</button>
    <pre>
        <code>
            conda env create -n myenv -f environment.yml
        </code>
    </pre>
</div>



