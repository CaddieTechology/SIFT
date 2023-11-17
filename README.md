# Smart Imagery Framing and Truthing (SIFT) System
SIFT is an rapid accurate fine-grained image labelling and annotation system to assist annotators to identify abnormality, corresponding boundaries, and other abnormalities on large-amount of chest x-ray images to train and test machine learning and deep learning artificial intelligence. 
## A.	Background
Development of machine learning and deep learning (ML/DL) for medical application requires a very large amount of high-quality data (radiographs, genomics, pathological images, etc.) to train and test in order to reach very high accuracy and robustness.  High-quality data requires (1) a gold standard to confirm the cases (e.g., biopsy to confirm the cancer on chest x-ray and CT, etc.); (2) accurate location and delineation of lesion; (3) other possible lesions located on the image; and (4) large amount of data. Accurate and consistent annotation require the participation of annotators with specific domain knowledge operating annotation tool and many times are very time consuming, tedious, inefficient, and lack of accuracy.  Although many image-based annotation tools have been developed for radiological images, it still cannot meet such demand because annotators need to determine the type of diseases, use of pointing device to follow, draw, and edit the boundaries of diseases, and debate type of disease.  Sometimes, use of these annotation tools may deter the annotator to perform such task.  Furthermore, consistency of annotation remains challenge even for identical annotator (intra-observer variance) and different annotators may use different medical terminologies for identical diseases (inter-observer variance).  Smart Imagery Framing and Truthing (SIFT) System is developed in order to attack the above issues such that it can benefit for the fast and accurate development of ML/DL for medical applications. 
## B.	Purpose of SIFT
SIFT is intended to assist annotators to accurately and rapidly identify the location of abnormality, its boundary coordinates, confidence level, possible recommended types of abnormality, and other co-located abnormalities on large-amount of chest x-ray (CXR) images such that these information can be used to generate training and testing sets to develop robust and accurate artificial intelligence technologies.
SIFT is not intended to assist physician to perform any clinical function such as screening, diagnosis, triage, etc.   
## C.	Technologies:
SIFT is based on Multi-task, Optimal-recommendation, and Max-predictive Classification and Segmentation (MOM ClasSeg) technologies to detect and delineate 66 different abnormal regions of interest (ROI) on chest x-ray image, provide confidence score for detected ROI, and various recommendation of abnormality for each ROI. The MOM ClasSeg System integrating Mask R-CNN and Decision Fusion Network is developed on a training dataset of over 300,000 adult chest x-ray, which contains over 240,000 confirmed abnormal images with over 300,000 confirmed ROIs corresponding to 66 different abnormalities and over 67,000 normal (i.e., “no finding”) images.
 
## D.	Features of SIFT

#### 1.	Providing Initial Type of Abnormalities
a.	SIFT can automatically detect and classify ROI into specific type of abnormality (“Predicted Disease”).  Annotator just clicks to confirm or reject its type.  
b.	SIFT can automatically predict 66 different types of abnormalities.  
c.	SIFT can automatically recommend several different abnormalities if the score of originally predicted abnormality is not high enough.  Annotator just clicks to select the recommended type.
#### 2.	Fully Compliance and Uniqueness of Abnormalities
a.	Among these unique abnormalities predicted by SIFT, 90% of disease lexicons comply with Medical Dictionary for Regulatory Activities (MedDRA) UMLS CUI coding and rest of 10% comply with Radiopaedia (international collaborative radiology educational resource from Wikipedia).
#### 3.	Providing Coordinates of Boundaries for ROI
a.	SIFT can automatically draw the boundary of ROI to predict the location coordinates.  
b.	Annotators can accept or edit the boundary using SIFT graphic user interface (GUI).
#### 4.	Providing Confidence Score for Each AI-specified ROI
a.	SIFT can automatically generate confidence score of ROI for each predicted disease.
#### 5.	Batch Processing of Large Amount of Images   
a.	SIFT can process large-amount of CXR to generate initial location and boundaries without any human intervention.
#### 6.	Providing Other Possible Abnormalities, Location, and Boundaries
#### 7.	Allowing Annotator to use SIFT GUI to determine types of abnormality and draw the boundaries of specific ROI on any place of image.
#### 8.	Allowing to store annotations and train train models
a.  Allowing Annotator to store any type of abnormality, corresponding boundary coordinates, confidence score, and recommended types, if any, in an editable excel spreadsheet file.   
b.	AI developers can use these files along with images to train their deep learning artificial intelligence technologies.
## References:
1.	[Self-Rating Curriculum Learning for Localization and Segmentation of Tuberculosis on Chest Radiograph, International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI), "Source: MEDICAL IMAGE COMPUTING AND COMPUTER ASSISTED INTERVENTION, MICCAI 2022, PT I , Book Series: Lecture Notes in Computer Science, DOI: 10.1007/978-3-031-16431-6_65, Conference Date: SEP 18-22, 2022, Conference Location: Singapore, ISSN: 03029743"](https://conferences.miccai.org/2022/en/https://link.springer.com/chapter/10.1007/978-3-031-16431-6_65)   
2.	[Developing and Assessing an AI-based Multi-Task Prediction System to Assist Radiologists Detecting Lung Diseases in Reading Chest X-Ray Images	Proceedings of SPIE Medical Imaging, "Source: MEDICAL IMAGING 2022: PHYSICS OF MEDICAL IMAGING, Book Series: Proceedings of SPIE, DOI: 10.1117/12.2652338, Conference Date: FEB 19-23, 2023, Conference Location: San Diego, California, United States, ISSN: 16057422"](https://spie.org/conferences-and-exhibitions/medical-imaging/programhttps://spie.org/Publications/Proceedings/Paper/10.1117/12.2652338)   
3.	[Assessing an AI-based Smart Imagery Framing and Truthing (SIFT) system to assist radiologists annotating lung abnormalities on chest X-ray images for development of deep learning models, Proceedings of SPIE Medical Imaging, "Source: MEDICAL IMAGING 2022: PHYSICS OF MEDICAL IMAGING, Book Series: Proceedings of SPIE, DOI: 10.1117/12.2653826, Conference Date: FEB 19-23, 2023, Conference Location: San Diego, California, United States, ISSN: 16057422"](https://spie.org/conferences-and-exhibitions/medical-imaging/programhttps://spie.org/Publications/Proceedings/Paper/10.1117/12.2653826)   
4.	[Automatic classification of pulmonary abnormalities from chest X-ray images: a multi-task deep learning model, Union World Conference on Lung Health, "Source: The 53rd Union World Conference on Lung Health 
Conference Date: NOV 8-11, 2022, Conference Location: Virtual, ISSN: 997-1098"](https://conf2022.theunion.org/https://theunion.org/sites/default/files/2022-11/Abstract_Book_2022-compressed.pdf)   
5.	[Automatic Detection of Multiple Abnormalities and Generation of Diagnostic Report from Radiological Images Using Multi-Task Optimal-Recommendation Max-Predictive Chest X-Ray Classification and Segmentation (MOM ClasSeg) System, "RSNA, Scientific Session (Chest Imaging)", 2022/7/28, "Source: 108th RSNA Annual Meeting, Scientific Session (Chest Imaging) T3-SSCH04-03, Conference Date: NOV 27 - DEC 1, 2022, Conference Location: Chicago, Illinois, United States"](https://www.rsna.org/annual-meeting)   
6.	[Using Artificial Intelligence for Chest Radiograph Interpretation: A Prospective Multi-site Study of the Automatic Detection of Multiple Abnormalities and Generation of Diagnostic Report System, "RSNA, Cutting Edge (Artificial Intelligence)”,"Source: 108th RSNA Annual Meeting, Cutting Edge (Artificial Intelligence), S3B-STCE Conference Date: NOV 27 - DEC 1, 2022,  Conference Location: Chicago, Illinois, United States"](https://www.rsna.org/annual-meeting)   
7.	[Impact of artificial intelligence on chest radiography reporting: a multireader-multi-center (MRMC) study of automatic detection of multiple abnormalities and generation of diagnostic report system, Union World Conference on Lung Health, "Source: The 54th Union World Conference on Lung Health, Conference Date: NOV 15-18, 2023 Conference Location: Paris"](https://conf2023.theunion.org/)   
8.	[Using artificial intelligence to assist radiologists in distinguishing COVID-19 from other pulmonary infections. J Xray Sci Technol. 2021;29(1):1-17. doi: 10.3233/XST-200735. PMID: 33164982; PMCID: PMC7990455.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7990455/#:~:text=Conclusion%3A,infections%20using%20chest%20CT%20images)   
9.	[Using artificial intelligence for chest radiograph interpretation: a retrospective multi-reader-multi-center (MRMC) study of the automatic detection of multiple abnormalities and generation of diagnostic report system](https://spie.org/medical-imaging/presentation/Using-artificial-intelligence-for-chest-radiograph-interpretation--a-retrospective/12927-31?SSO=1)   
## Acknowledgement
1.	National Institute of AIDS and Infectious Diseases, NIH (NIAID/NIH) TB Portals (https://tbportals.niaid.nih.gov/) Bethesda, MD, USA
2.	National Institute of Library, NIH (NLM/NIH), Bethesda, MD, USA
3.	University of Chicago, Chicago, IL.
4.	University of Oklahoma, Oklahoma City, OK.
5.	Association for Chinese Infectious Diseases Society, Beijing. China
6.	Shenzhen Smart Imaging Healthcare Corp (Zying), Shenzhen, China
7.	MS Technologies Corporation, Rockville, MD, USA
## Collaborators:
#### •	TB Portals, National Institutes of Allergies and Infectious Diseases (NIAID), NIH
The NIAID TB Portals Program is a multi-national collaboration for tuberculosis (TB) data sharing and analysis to advance TB research. (https://tbportals.niaid.nih.gov/about)
Since March 31, 2022, Zying has worked with NIAID to annotate NIAID-collected TB CXR images.  So far, Caddie has provided AI annotation of over 7,500 TB DR images for TB Portals using unique MedDRA ontology identifier.  Caddie will continue to provide AI annotation and image analysis to TB Portals as more cases are collected in the future.

#### •	MIDRC (Medical Imaging and Data Resource Center)
MIDRC is funded by the National Institute of Biomedical Imaging and Bioengineering (NIBIB) of NIH and hosted at the University of Chicago, is co-led by the American College of Radiology® (ACR®), the Radiological Society of North America (RSNA), and the American Association of Physicists in Medicine (AAPM). (https://www.midrc.org/more-about-midrc)
Since March 15, 2023, MIDRC will post Caddie-annotated COVID-19 radiographs on MIDRC web site.  Caddie has provided AI annotation of over 100,000 COVID-19 DR images including identification of COVID lesion, other comorbidity, and their detailed boundaries.  Caddie will continue to provide annotation service, tools, and data.

