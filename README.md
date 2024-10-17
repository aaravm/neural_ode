# Neural ODE weather forecasting
Companion repo to my blog article [Forecasting the weather with neural ODEs](https://sebastiancallh.github.io/post/neural-ode-weather-forecast/). Contains code for training the neural ODE and plotting the fit.

###Link to the Project Report:
Project Report - [https://drive.google.com/file/d/1sTfBpmtCicVzsQPhCJEa8ZIUt9KMQWS1/view]
### Data
The dataset used is [available on Kaggle](https://www.kaggle.com/sumanthvrao/daily-climate-time-series-data). It is released under [CC0: Public domain](https://creativecommons.org/publicdomain/zero/1.0/) and included in this repo's [data](./data) folder for convenience.

### Reproducing the experiments
Make sure you have Julia installed (tested with Julia 1.8). `cd` to the project root folder and run `julia --project` to enter the Julia shell using the project environment. Run `using Pkg; Pkg.instantiate()`, to pull down the dependencies, followed by `include("scripts/fit_model.jl")` to fit the model and generate the plots and animations seen in the blog article. Don't be surprised if creating the training animation takes at least as long as fitting the model.

### Figures
#### Model training animation
![Training animation](./plots/training.gif)

#### Model extrapolation
![Model extrapolation](./plots/extrapolation.svg)
