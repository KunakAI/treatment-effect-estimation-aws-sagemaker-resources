# Treatment Effect Estimator — AWS Marketplace sample

This repository contains the sample notebook and reference dataset for the **RCT Treatment
Effect Estimator** AWS Marketplace product (T-Learner/S-Learner heterogeneous treatment effect
estimation for randomized experiment data).

This is a companion sample repo, not the product's source code. It exists solely to satisfy AWS
Marketplace's requirement for a public sample notebook and sample input/output data so buyers can
see what a training/inference run looks like before subscribing.

## Contents

- `notebooks/sagemaker_algorithm_usage.ipynb` — end-to-end walkthrough: train the subscribed
  Algorithm on your own data, deploy a real-time endpoint, run real-time and batch inference,
  inspect the training report. Uses placeholder ARNs/values you replace with your own after
  subscribing — no setup beyond an AWS account with the product subscribed.
- `data/train.csv`, `data/test.csv` — the public reference dataset used by the notebook: the
  Levamisole + Fluorouracil adjuvant chemotherapy trial for colon cancer (929 patients, a public
  dataset from the [AI for Medical Treatment Coursera course](https://www.coursera.org/learn/ai-for-medical-treatment/),
  originally from R's `survival::colon` dataset). Used only to illustrate the algorithm's
  mechanics — the product itself works on any randomized experiment data (binary treatment,
  binary or continuous outcome), not just clinical trials.

## Not a medical device

This product is a general-purpose statistical/ML tool. It is not a medical device, is not
intended for clinical diagnosis, and must not replace professional medical or regulatory
judgment. See the product listing's EULA for full terms.
