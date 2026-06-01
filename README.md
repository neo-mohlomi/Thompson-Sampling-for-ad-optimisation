# Advertisement Optimization using Thompson Sampling

## Project Overview

This project applies the **Thompson Sampling** Reinforcement Learning algorithm to identify the advertisement most likely to generate customer clicks. The results are compared against a previously implemented **Upper Confidence Bound (UCB)** model.

Using customer interaction data from **10,000 customers** and **10 advertisements**, the algorithm learns which advertisement performs best while continuously updating its beliefs based on observed outcomes.

---

## Business Problem

Organizations want to maximize click-through rates while minimizing the cost of displaying ineffective advertisements.

The challenge is to determine:

* Which advertisement generates the highest customer engagement?
* How quickly can an algorithm identify the best-performing advertisement?
* Which reinforcement learning strategy reaches the optimal decision faster?

---

## Dataset

The dataset contains:

* 10,000 customer observations
* 10 advertisements
* Binary outcomes:

  * 1 = Click
  * 0 = No Click

Each row represents a customer interaction and each column represents a specific advertisement.

---

## Methodology

### Thompson Sampling

Thompson Sampling is a probabilistic Reinforcement Learning algorithm that balances exploration and exploitation by sampling from posterior probability distributions.

The algorithm:

1. Explores different advertisements when uncertainty is high.
2. Gradually favors advertisements with stronger evidence of success.
3. Learns the optimal advertisement through Bayesian updating.

---

## Results

The model identified **Advertisement 4** as the highest-performing advertisement.

Key findings:

* Thompson Sampling consistently converged toward Advertisement 4.
* The algorithm identified the optimal advertisement with fewer observations than UCB.
* Around 500 customer interactions, Thompson Sampling had already developed a strong preference for Advertisement 4.
* Compared to UCB, Thompson Sampling demonstrated faster learning and more efficient exploration.

---

## Comparison with UCB

| Metric                        | UCB               | Thompson Sampling |
| ----------------------------- | ----------------- | ----------------- |
| Best Advertisement Identified | Ad 4              | Ad 4              |
| Convergence Speed             | Slower            | Faster            |
| Exploration Strategy          | Confidence Bounds | Bayesian Sampling |
| Efficiency                    | Good              | Better            |

Both algorithms successfully identified the optimal advertisement. However, Thompson Sampling reached the correct conclusion more quickly, making it a more efficient approach for this dataset.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Reinforcement Learning
* Thompson Sampling
* Bayesian Methods

---

## Business Impact

This solution can help businesses:

* Increase click-through rates
* Reduce advertising costs
* Improve marketing ROI
* Accelerate decision-making
* Optimize customer engagement strategies

---

## Future Improvements

* Compare cumulative rewards between UCB and Thompson Sampling.
* Apply the algorithms to real-world advertising datasets.
* Extend the framework to contextual advertising.
* Evaluate performance in dynamic environments where customer preferences change over time.

---

## Author

Neo Mohlomi

MSc Astrophysics Candidate | Data Science & Machine Learning Enthusiast

GitHub: https://github.com/neo-mohlomi
