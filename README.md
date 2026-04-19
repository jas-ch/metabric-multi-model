# Multi-Model Machine Learning identifies MAPT, CHEK1, AURKA as Breast Cancer Prognostic Markers

** Abstract

Breast cancer is the most common cancer among women globally, and the second leading cause of cancer death. While early detection improves survival rates, personalizing treatment based on genomic biomarkers could further increase survival duration. This project applies a multi-model machine learning approach to identify key gene biomarkers correlating with breast cancer survival duration, enabling physicians to personalize treatment. I hypothesized that different models contribute complementary findings: linear regression captures proportional gene-survival relationships, random forest reveals non-linear interactions, and neural network could perform deep analysis on larger datasets but was anticipated to underperform on the small METABRIC dataset (n=1904 patients). 

Using the METABRIC dataset, I preprocessed gene expression and clinical data by imputing missing values and encoding categorical variables. I trained three models?ElasticNet linear regression, random forest, and PyTorch neural network?using 70/15/15 train/validation/test split to predict overall survival time. 

Random forest achieved the best test performance (r?=0.147), followed by linear regression (r?=0.138), while the neural network underperformed (r?=0.052) as anticipated. The models identified MAPT, CHEK1, and AURKA as top gene biomarkers strongly associated with survival duration, consistent with published cancer genomics research. 

The analysis focused on genomic factors, yet survival duration also depends on age, comorbidities, lifestyle, and unrelated causes of death, introducing variance. The consistent under-prediction of survival durations aligns with this limitation and validates the integrity of our genomic-focused approach. These findings demonstrate that complementary models can uncover actionable genomic biomarkers, offering a pathway toward personalized breast cancer treatment and improved prognosis outcomes. 
