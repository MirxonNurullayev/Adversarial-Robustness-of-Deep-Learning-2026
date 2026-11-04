# Research Article Materials

## Article Title
Adversarial Robustness of Deep Learning-Based Network Intrusion Detection: Two-Sided Error Analysis and an Explainability-Guided Tandem Defence

## Authors
Nurullaev Mirkhon Muhammadovich

## Abstract
Deep-learning network intrusion detectors are usually evaluated against adversarial attacks with a single accuracy figure, which hides two different failures. We prove that, for a binary detector, untargeted, targeted and margin-based sign-gradient attacks generate identical iterates, so every such attack is the union of an evasion attack on malicious flows and a false-alarm flooding attack on benign flows. We relate the shift of the operating point to alarm precision and operational cost, and bound the robustness radius from below by the logit margin divided by the largest L_1 norm of the masked input gradient. Experiments on NSL-KDD and UNSW-NB15 with five training seeds support the analysis. Under projected gradient descent with budget 0.1, the false-alarm rate of an undefended NSL-KDD detector rises from 3.0% to 97.8% while its detection rate falls from 68.4% to 53.0%; the Youden index becomes −0.449 and flooding causes 82% of the accuracy loss. Benign records flip at a median budget of 0.047 against 0.260 for attacks (seed 42), because their margin changes much more steeply along the mutable features. Adversarial training holds the false-alarm rate under attack at 7.7%, and 90% of its accuracy gain is suppressed flooding, but it raises the clean false-alarm rate to 7.3%. A monitor on expected-gradients SHAP attributions detects non-adaptive perturbations almost perfectly (AUC 0.997 on NSL-KDD, seed 42) yet is substantially weakened by an adaptive attacker when used alone. Combined with adversarial training in a tandem defence, it keeps a system detection rate of 78.2% with 6.1% false intrusion alerts under a fully adaptive attack on NSL-KDD, against 62.8% and 8.7% for adversarial training alone under its strongest attack, at the price of flagging 40.8% of the manipulated benign records as manipulations. A monitor on the raw features detects non-adaptive perturbations at least as well, so explanation-based monitoring is best seen as an interpretable second layer, not a substitute for robust training.

## Repository Contents
- Article.pdf: Full research paper
- Data/: Research datasets
- Code/: Analysis scripts
- Figures/: Research figures

## License
CC BY 4.0
