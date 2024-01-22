# transformer-forecasting
Using a transformer as the basis for a time series forecasting algorithm.

## The Data
I will be using spot price data in terms of $USD for cryptocurrencies to test the forecasting of a transformer model. I have 5 min, hourly and daily price data for ETH; hourly and daily data for BTC.

This data has been downloaded from https://www.cryptodatadownload.com/data/.

## Version 1
Version 1 of the forecasting model, uses the decoder structure of the transformer architecture in "Attention is All You Need" (2017). The whole architecture of the model described in this paper uses both an encoder (left-half of diagram) and decoder (right-half of diagram) as the objective of the model was to translate text. The encoder part of the model uses cross attention to condition the decoder on the translation of the language as well as the past of the decoder. Since I am not using the model for translation but purely to predict the future tokens based on past tokens in the first version of this model, I have only taken the decoder part of the model from the paper.

![Attention is All You Need transformer architecture](/images//TransformerArchitecture.png)

Also for reference, I used a video lecture from Andrej Karpathy, so a lot of the code is taken straight from his work on this video. If anyone is interested in understanding how the transformer actually works, specifically from a practical and programming standpoint, his video is great!

### Results:


## Version 2