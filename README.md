# Multi-Armed Bandit Reinforcement Learning Project
## Overview
This project focuses on implementing and comparing three different algorithms for solving the Multi-Armed Bandit problem. The goal is to determine the most optimal advertisement type out of ten available options (Ad1 to Ad10). The algorithms we’ll compare are:

- Algoritma A/B Testing: A classic approach where we randomly assign users to different ads and measure their performance.
- Epsilon Greedy: An exploration-exploitation strategy that balances between trying new ads (exploration) and exploiting the best-performing ad (exploitation).
- Adaptive Epsilon Greedy: Similar to Epsilon Greedy, but with a dynamically adjusted exploration rate.

## Project Structure
```
├── data/
│   ├── Ads_CTR_Optimisation.csv                       # CSV file containing ad performance data
├── notebooks/
│   ├── Jupyter File.ipynb                             # Algorithm comparison and evaluation
├── TA
│   ├── Paulinus A. S. Jamlu 193114033.pdf             # Tugas Akhir
├── README.md                                          # Project documentation
```
## Getting Started
Clone this repository to your local machine.
Install the required libraries using pip install -r requirements.txt.
Explore the data in Ads_CTR_Optimisation.csv to understand the ad performance metrics.
Run the notebooks in the notebooks/ directory to analyze the data and compare the algorithms.
## Usage
Modify the parameters (e.g., epsilon, l,f, number of iteration/loop) in Jupyter File.ipynb as needed.
Run the bandit algorithms using the provided data.
Evaluate the performance of each algorithm using relevant metrics (e.g., click-through rate, conversion rate).
## Results
After conducting experiments and analyzing the performance of different algorithms, we observed the following:

- Adaptive Epsilon Greedy:
  * This algorithm adapts its exploration rate dynamically based on the observed rewards. It aims to strike a balance between exploration (trying out different ads) and exploitation (choosing the best-performing ad).
  * Optimal Ad Type: The adaptive epsilon greedy algorithm identified the most optimal ad type with a high degree of confidence.
  * Complexity: However, it is worth noting that the adaptive epsilon greedy algorithm is more complex to implement and tune compared to other methods.
- Algoritma A/B Testing:
  * A classic approach where users are randomly assigned to different ads, and their performance is measured.
  * Optimal Ad Type: While A/B testing provides a straightforward way to compare ads, it may not always identify the optimal ad type with high certainty.
  * Simplicity: A/B testing is simpler to set up and understand, making it a good choice for scenarios where complexity is a concern.
In summary, if you prefer a simpler approach and are willing to accept some uncertainty, A/B testing is a suitable choice. However, if you want a more sophisticated solution that adapts over time, Adaptive Epsilon Greedy is the way to go.

Remember to adjust the parameters and evaluate the algorithms based on relevant metrics.

## Acknowledgments
Special thanks to the open-source community and the authors of relevant research papers.

Feel free to add more details, references, and any other relevant information to your readme.md file. Good luck with your project! 🚀🤖