# Synthetic Energy Data Generation using Time Variant Generative Adversarial Network
Authors: Shashank Asre, Dr. Adnan Anwar

Code Reference: Jinsung Yoon, Daniel Jarrett, Mihaela van der Schaar, "Time-series Generative Adversarial Networks," Neural Information Processing Systems (NeurIPS), 2019, https://papers.nips.cc/paper/8789-time-series-generative-adversarial-networks.

We would like to thank the authors, 'Jinsung Yoon, Daniel Jarrett, Mihaela van der Schaar'; for making 'TimeGAN' code publicly available. TimeGAN framework is baseline for our research on Timeseries Generation using AEMO dataset.

This Repository contains the execution of TimevariantGAN framework on energy dataset to generate synthetic energy data. The Original energy data is acquired from the "AEMO - Aggregated Price and Demand data" website (https://aemo.com.au/en/energy-systems/electricity/national-electricity-market-nem/data-nem/aggregated-data). Website contains monthly energy consumption data for various states of Australia. For this project, energy data is collected for whole 2020 year for the states Victoria, New South Wales, South Australia, Queensland and Tasmania.

We have perform below modification to execute the implementation of timeseries generation using AEMO-energy consumption dataset.
* New Dataset: Energy Consumption data obtained from AEMO website
* Modified Optimizer: RMSPropOptimizer
* Modified Activation function
* Added new metrics-
  * Accuracy
  * precision
  * recall
  * f1-score
  * cohens kappa
  * ROC AUC

The repository contains –
* One ‘.ipynb’ file named as “TimevariantGAN.ipynb”, 
* Original energy dataset named as “energy_data.csv”
* An output – Synthetic energy data, an excel file with annotation “Synthetic_energydata.xls” obtained from the execution of TimevariantGAN.

To implement the code, download the energy dataset 'energy_data.csv','TimevariantGAN.ipynb' and execute using Google colab, jupyternotebook and IDE of your choice.

System/technological requirement-
* Tensorflow- 1.15.0
* pandas- 0.25.1
* numpy- 1.17.2
* argparse 1.1
