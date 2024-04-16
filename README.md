# Hepatocellular carcinoma Computer Vision Project

## Context

Hepatocellular carcinoma (HCC) being the most common liver cancer, with more than 40.000 cases in the United States in 2020. With a growing number of diagnosed cases, optimizing the evaluation of treatment effects on the tumor size can be a key driver to quicken this task for radiologist. In this case, the work presented aims at estimating the effects of transarterial chemoembolization (TACE), which delivers chemotherapy to targeted liver tumors.

Even though TACE is the most common treatment, up to 60\% of patients do not benetif from this treatment, highlighting the importance of knowing the effect it is having in the patient. As it is a treatment with high vaariability, several models have been developed aiming at predicting the effectiveness of this training.

AI models to predict,

TCIA database, ..

In this work, the HCC-TACE collection is used, presented in paper [pap]. The dataset contains a collection of 105 patients with HCC who where treated with TACE at The University of Texas MD Anderson Cancer Center between 1997 and 2012. The dataset contains computer tomography scans both from pre-treatment and post-treatment, containing a segmentation for the cancerous mass.

## Dataset

Data is obtained through The Cancer Imaging Archive (TCIA) [ref] which contains numerous datasets for different types of cancer. In this case, the dataset is the one mentioned before \textit{HCC-TACE-Seg | Multimodality annotated HCC cases with and without advanced imaging segmentation}. The dataset has to be downloaded through the NBIA Data Retriever, and contains 51,968 images in DICOM format and has a size of 28.57 GB. The CT scans can be visualized online through the National Cancer Institute [ref] searching for the HCC-TACE dataset. As example, a sample of the image  \ref{fig:sample_pre}

\begin{figure}[h]
\centering
\includegraphics[width = 0.5\textwidth]{figures/sample_image_con_seg_25.png}
\caption{Patient number 25 pre-treatment image with and without segmentation}
\label{fig:sample_pre}
\end{figure}

The computer tomography scans contain several sections of the patient's body, so the ones shwoing the cancerous mass have to be searched among all of the images in each series, which will contain a quantity of images ranging from 30 to 100 separate sections.
