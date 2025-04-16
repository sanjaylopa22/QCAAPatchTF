# QCAAPatchTF: Quantum-Classical Self-Attention Advanced Patch based Transformer

QCAAPatchTF is a quantum-classical hybrid attention module embedded into an advanced patch based transformer architecture which is suitable for deep time series analysis.

We provide a neat code base to evaluate advanced deep time series models or develop your model, which covers five mainstream tasks: **long- and short-term forecasting, anomaly detection, and classification.**

Usage
Install Python 3.8. For convenience, execute the following command.
pip install -r requirements.txt

Prepare Data. You can obtain the well pre-processed datasets from [Google Drive].
Train and evaluate model. We provide the experiment scripts for all benchmarks under the folder ./scripts/. You can reproduce the experiment results as the following examples:
# long-term forecast
bash ./scripts/long_term_forecast/ETT_script/QCAAPatchTF.sh
# short-term forecast
bash ./scripts/short_term_forecast/QCAAPatchTF.sh
# anomaly detection
bash ./scripts/anomaly_detection/PSM/QCAAPatchTF.sh
# classification
bash ./scripts/classification/QCAAPatchTF.sh

Develop your own model.
Add the model file to the folder ./models. You can follow the ./models/Transformer.py.
Include the newly added model in the Exp_Basic.model_dict of ./exp/exp_basic.py.
Create the corresponding scripts under the folder ./scripts.

# Contact
If you have any questions or suggestions, feel free to contact our maintenance team:

# Current:
Sanjay Chakraborty (Postdoc, sanjay.chakraborty@liu.se)
Or describe it in Issues.