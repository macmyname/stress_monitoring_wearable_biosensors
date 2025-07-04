📊 Project Title: Stress Monitoring and Recent Advancements in Wearable Biosensors

🗭 Overview

This project explores how wearable biosensor data can be used to monitor stress over time using real-world physiological datasets. With growing interest in employee wellness, understanding stress patterns through physiological signals can guide individuals and organizations in making better-informed decisions.

❗ Problem Statement

Stress is a critical factor influencing workplace productivity and health, yet it is often under-monitored. While wearable biosensors offer potential for real-time physiological monitoring, many organizations lack the systems or expertise to harness their data effectively. In low-resource settings, limited access to mental health services further emphasizes the need for early, objective detection of stress markers.

Using publicly available physiological data collected from healthcare workers, this study aims to explore how stress manifests across different temporal phases using biosignals such as Electrodermal Activity (EDA), Heart Rate (HR), and Inter-Beat Interval (IBI). These insights can inform early intervention strategies and support organizational well-being programs.

🎯 Objectives

To clean, process, and analyze wearable biosensor data.

To extract stress-related features from physiological signals (EDA, HR, BVP, IBI).

To monitor and visualize changes in physiological stress indicators across time.

To derive insights that inform workplace stress management.

⚙️ Methodology

A real-world physiological dataset was obtained from Dryad.

Signal pre-processing and statistical feature extraction were performed using Python.

Sessions were categorized into:

Initial Phase: early exposure to occupational demands.

Adjustment Phase: period of adaptation and increasing workload.

Features such as EDA mean, HR mean, and HRV (measured by RMSSD) were computed.

Visualizations and descriptive analyses were used to compare stress indicators across phases.

📁 Dataset

Source: Ozcelik, D. et al. (2021). Wearable sensor dataset to track physical activity, posture, and social interactions of nurses in a hospital unit. Dryad. https://doi.org/10.5061/dryad.5hqbzkh6f

🔹 Note: While the dataset does not track employees across industries or onboarding cycles, it includes high-quality physiological data from nurses, offering a proxy for stress in occupational contexts.

📄 Data Preprocessing and Lifecycle Tagging

Incomplete sessions were filtered based on presence of key biosensor files (EDA, HR, IBI).

Session start timestamps were used to calculate days since baseline.

Sessions were tagged as:

Initial Phase (0–14 days)

Adjustment Phase (15–90 days)

📊 Feature Extraction

Key computed features:

EDA: Mean, standard deviation, peak count

HR: Mean, standard deviation

IBI: RMSSD (Root Mean Square of Successive Differences), as a proxy for Heart Rate Variability (HRV)

🔢 Data Visualization

Boxplots were generated to display distributions of EDA_mean and HRV (RMSSD) across the two time phases.

🔍 Insight & Interpretation

EDA: The median EDA_mean is higher in the Adjustment Phase, suggesting elevated sympathetic nervous system activity and possible increased stress levels during adaptation.

HRV (RMSSD): Lower median RMSSD values in the Adjustment Phase suggest reduced parasympathetic activity, commonly associated with stress.

Initial Phase: Greater variability in both metrics, indicating mixed physiological responses. Some individuals may experience anticipatory stress, while others remain stable.

📌 Recommendation

Stress is real and often unrecognized until it leads to burnout or attrition. While this dataset is based on nurses in a healthcare setting, the findings demonstrate the value of wearable biosensor data in monitoring stress over time.

Organizations should consider incorporating periodic physiological assessments into workplace health strategies. By tracking stress markers over time—from entry-level exposure to periods of increasing responsibility—employers can better support employee well-being and performance.

🛠️ Tools & Tech Stack

Python

Pandas, NumPy

Seaborn, Matplotlib

Scikit-learn

Jupyter Notebook

📍 Significance

This project illustrates how biosensor data can be used to identify stress dynamics in high-demand roles. It serves as a stepping stone toward building scalable, data-driven tools for workplace well-being and early stress detection.

🔖 References

Ozcelik, D., et al. (2021). Wearable sensor dataset to track physical activity, posture, and social interactions of nurses in a hospital unit. Dryad. https://doi.org/10.5061/dryad.5hqbzkh6f

Shaffer, F., & Ginsberg, J. P. (2017). An Overview of Heart Rate Variability Metrics and Norms. Frontiers in Public Health, 5, 258. https://doi.org/10.3389/fpubh.2017.00258

ChatGPT by OpenAI (2025). Used for code troubleshooting, technical writing, and insight formulation.

