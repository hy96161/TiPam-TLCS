# Exploring Human Mobility: A Time-Informed Approach to Pattern Mining and Sequence Similarity

In this paper, we propose two methods: **Time-Informed Pattern Mining (TiPam)** for frequent pattern mining of time-informed sequences, and **T-LCS**, used to calculate the similarity score between two sequences.

## Instructions

### TiPam

`Time-informed pattern mining (TiPam).ipynb` contains the code for frequent pattern mining of time-informed sequences. Since the real activity sequences cannot be made publicly available due to confidentiality restrictions, a sample dataset with mocked temporal interval sequences is provided at the end of the code.

- **How TiPam Works**: The method extracts frequent patterns of varying lengths from the sequence data. Each extracted pattern includes information about the median start time and duration of activities.
- **Reproducing Results**: You can apply TiPam to your own mobility data to extract a hierarchical representation of frequent mobility patterns, similar to **Figure 5** in the manuscript.
- **Mocked Data**: While the mocked dataset provides a demonstration, the real dataset used in the manuscript is described in Section X. TiPam can be used to reproduce results similar to those reported.

### T-LCS

`T-LCS.ipynb` is the code for calculating the similarity score between two sequences.

- **Benchmark Data**: The benchmark data includes six sequences (S1, S2, S3, S4, S5, and S6). S1 represents a typical timestamped semantic sequence, while the other sequences are modified versions of S1, designed based on specific similarity criteria. These sequences are shown in **Table 1(a)** of the manuscript.
- **How T-LCS Works**: The T-LCS method calculates similarity between two sequences. This similarity score is then used to compute **Individual Regularity (IR)** and **Inter-personal Similarity (IS)**.
- **Reproducing Results**: For a dataset with multiple users and their corresponding sequences, you can compute their IR and visualize the distribution, as shown in **Figure 4** of the manuscript. Using the inter-personal similarity scores, you can apply clustering algorithms like OPTICS to group users into clusters, as demonstrated in **Figure 7** of the manuscript.

## Additional Information

- **Mocked Data Usage**: The mocked data is included for demonstration purposes, but all findings reported in the manuscript were generated using real-world data, which is confidential.
- **Figures**: To reproduce tables and figures similar to those in the manuscript (e.g., **Table 1**, **Figures 4, 6, 7, and 8**), use the provided scripts with your own datasets. Ensure that your data follows a similar structure to the real data described in Section X of the manuscript.

