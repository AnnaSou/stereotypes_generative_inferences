# Analyzing Stereotypes in Generative Text Inference Tasks

By: [Anna Sotnikova] `<asotniko@umd.edu>`, [Yang Trista Cao]`<ycao95@umd.edu>`, [Hal Daumé III](http://hal3.name) `<hal3@umd.edu>`, [Rachel Rudinger]`<rudinger@umd.edu>` 

As part of a study of stereotypes in Generative Text Inference Tasks, we collected and annotated a dataset of models generated text inferences for a variety of social groups in the United States. We call this dataset the **Stereotypes in Generative Text Inference Tasks**; what follows below is the [datasheet](https://arxiv.org/abs/1803.09010) describing this data. If you use this dataset, please acknowledge it by citing the original paper:

```
@inproceedings{sotnikova-etal-2021-analyzing,
    title = "Analyzing Stereotypes in Generative Text Inference Tasks",
    author = "Sotnikova, Anna  and
      Cao, Yang Trista  and
      Daum{\'e} III, Hal  and
      Rudinger, Rachel",
    booktitle = "Findings of the Association for Computational Linguistics: ACL-IJCNLP 2021",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.findings-acl.355",
    doi = "10.18653/v1/2021.findings-acl.355",
    pages = "4052--4065",
}
```


## Motivation


1. **For what purpose was the dataset created?** *(Was there a specific task in mind? Was there a specific gap that needed to be filled? Please provide a description.)*
    
    This dataset was created to study stereotypes in masked English language models and measure how stereotypes in models align with human ones. The approach for measuring stereotypes is built on the Agency Beliefs Communion (ABC) model, which measures stereotypes toward a social group with respect to 16 traits in three dimensions: Agency/Socioeconomic Success, Conservative–Progressive Beliefs, and Communion.

1. **Who created this dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)?**
    
    This dataset was created by Anna Sotnikova, Yang Trista Cao, Hal Daumé III, and Rachel Rudinger. At the time of creation, Cao and Sotnikova were graduate students at the University of Maryland (UMD), and Daumé and Rudinger are Professors there.


1. **Who funded the creation of the dataset?** *(If there is an associated grant, please provide the name of the grantor and the grant name and number.)*
    
    Funding for Cao and Daum\'e III was provided in part from the National Science Foundation project 2131508 and in part from University of Maryland foundation funds. Funding for Sotnikova was provided through the UMD AMSC program. 


1. **Any other comments?**
    
    None.





## Composition


1. **What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?** *(Are there multiple types of instances (e.g., movies, users, and ratings; people and interactions between them; nodes and edges)? Please provide a description.)*
    
    The dataset contains four files: situations, target category and target domains, examples with single annotation, examples with four annotations.

In the Situations file, we provide 103 manually created situations, which can be divided into two groups: underspecified situations and neutral situations.

In the target category and target domain file, we have 71 target categories divided into 6 target domains that are common in the United States.


Examples with single annotation and four annotations contain one or four annotations respectively for the pairs of the permises and the respectie hypotheis.

2. **How many instances are there in total (of each type, if appropriate)?**
    
    In total, we have 2098 annotation. 

3. **Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set?** *(If the dataset is a sample, then what is the larger set? Is the sample representative of the larger set (e.g., geographic coverage)? If so, please describe how this representativeness was validated/verified. If it is not representative of the larger set, please describe why not (e.g., to cover a more diverse range of instances, because instances were withheld or unavailable).)*
    
    Our dataset contains all instances (for the details, please, see the paper above).


4. **What data does each instance consist of?** *(``Raw'' data (e.g., unprocessed text or images)or features? In either case, please provide a description.)*
    
    The data is raw.


5. **Is there a label or target associated with each instance? If so, please provide a description.**
    
    Each example has annotations for 6 questions from our survey, annotator ID, and example ID. <br />
    Q1: Valid? has possible answers: Yes (1) or No (5).<br />
    Q2: Plaus? has possible answers: Yes(1) or No(5).<br />
    Q3: Iden? has possible answers: Yes(1), Maybe yes(2), Not sure(3), Maybe no(4), or No(5).<br />
    Q4: Situ? has possible answers: Yes(1), Maybe yes(2), Not sure(3), Maybe no(4), or No(5).<br />
    Q5: Senti? has possible answers: Positive(1), Maybe positive(2), Neutral(3), Maybe negative(4), or Negative(5).<br />
    Q6: Stereo? has possible answers: Yes(1), Maybe yes(2), Not sure(3), Maybe no(4), or No(5).<br />
    For more details on questions from the survey,please, read the paper.

6. **Is any information missing from individual instances?** *(If so, please provide a description, explaining why this information is missing (e.g., because it was unavailable). This does not include intentionally removed information, but might include, e.g., redacted text.)*
    
    No.


7. **Are relationships between individual instances made explicit (e.g., users' movie ratings, social network links)?** *( If so, please describe how these relationships are made explicit.)*
    
  No. Instances were annotated independently. 

8. **Are there recommended data splits (e.g., training, development/validation, testing)?** *(If so, please provide a description of these splits, explaining the rationale behind them.)*
    
    We expect this data to be used for testing purposes.

    We do not explicitly provide a training/validation/testing split;   

9. **Are there any errors, sources of noise, or redundancies in the dataset?** *(If so, please provide a description.)*
    
   There are no errors due to data processing. However, one should always keep in mind that all annotations are subjective. 


10. **Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g., websites, tweets, other datasets)?** *(If it links to or relies on external resources, a) are there guarantees that they will exist, and remain constant, over time; b) are there official archival versions of the complete dataset (i.e., including the external resources as they existed at the time the dataset was created); c) are there any restrictions (e.g., licenses, fees) associated with any of the external resources that might apply to a future user? Please provide descriptions of all external resources and any restrictions associated with them, as well as links or other access points, as appropriate.)*
    
    The dataset is self-contained.


11. **Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals' non-public communications)?** *(If so, please provide a description.)*
    
    No; 

12. **Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety?** *(If so, please describe why.)*
    
   Some generated hypothesis might be offensive to certain target categories.

13. **Does the dataset relate to people?** *(If not, you may skip the remaining questions in this section.)*
    
    Yes, all generations made about certain target categories.

14. **Does the dataset identify any subpopulations (e.g., by age, gender)?** *(If so, please describe how these subpopulations are identified and provide a description of their respective distributions within the dataset.)*
    
   We collect annotations for 71 target categories.

15. **Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset?** *(If so, please describe how.)*
    
    No.


16. **Does the dataset contain data that might be considered sensitive in any way (e.g., data that reveals racial or ethnic origins, sexual orientations, religious beliefs, political opinions or union memberships, or locations; financial or health data; biometric or genetic data; forms of government identification, such as social security numbers; criminal history)?** *(If so, please provide a description.)*
    
    Some generated hypothesis might be offensive to certain target categories.



17. **Any other comments?**
    
    None.





## Collection Process


1. **How was the data associated with each instance acquired?** *(Was the data directly observable (e.g., raw text, movie ratings), reported by subjects (e.g., survey responses), or indirectly inferred/derived from other data (e.g., part-of-speech tags, model-based guesses for age or language)? If data was reported by subjects or indirectly inferred/derived from other data, was the data validated/verified? If so, please describe how.)*
    
    The annotations were made by the paper authors.

1. **What mechanisms or procedures were used to collect the data (e.g., hardware apparatus or sensor, manual human curation, software program, software API)?** *(How were these mechanisms or procedures validated?)*
    
   N/A

1. **If the dataset is a sample from a larger set, what was the sampling strategy (e.g., deterministic, probabilistic with specific sampling probabilities)?**
    
   No.

1. **Who was involved in the data collection process (e.g., students, crowdworkers, contractors) and how were they compensated (e.g., how much were crowdworkers paid)?**
    
    The annotations were amde by the paper authors, no additonal compensation was provided.

1. **Over what timeframe was the data collected?** *(Does this timeframe match the creation timeframe of the data associated with the instances (e.g., recent crawl of old news articles)?  If not, please describe the timeframe in which the data associated with the instances was created.)*
    
    The dataset was collected in the Spring of 2021.

1. **Were any ethical review processes conducted (e.g., by an institutional review board)?** *(If so, please provide a description of these review processes, including the outcomes, as well as a link or other access point to any supporting documentation.)*
    
    No.

1. **Does the dataset relate to people?** *(If not, you may skip the remaining questions in this section.)*
    
    Yes; 


1. **Did you collect the data from the individuals in question directly, or obtain it via third parties or other sources (e.g., websites)?**
    
   Directly, all individuals filled the provided survey.

1. **Were the individuals in question notified about the data collection?** *(If so, please describe (or show with screenshots or other information) how notice was provided, and provide a link or other access point to, or otherwise reproduce, the exact language of the notification itself.)*
    
    N/A

1. **Did the individuals in question consent to the collection and use of their data?** *(If so, please describe (or show with screenshots or other information) how consent was requested and provided, and provide a link or other access point to, or otherwise reproduce, the exact language to which the individuals consented.)*
    
   N/A

1. **If consent was obtained, were the consenting individuals provided with a mechanism to revoke their consent in the future or for certain uses?** *(If so, please provide a description, as well as a link or other access point to the mechanism (if appropriate).)*
    
    N/A

1. **Has an analysis of the potential impact of the dataset and its use on data subjects (e.g., a data protection impact analysis) been conducted?** *(If so, please provide a description of this analysis, including the outcomes, as well as a link or other access point to any supporting documentation.)*
    
    Yes, please, see the related paper. 


1. **Any other comments?**
    
    None.





## Preprocessing/cleaning/labeling


1. **Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)?** *(If so, please provide a description. If not, you may skip the remainder of the questions in this section.)*
    
    No.

1. **Was the "raw" data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?** *(If so, please provide a link or other access point to the "raw" data.)*
    
   No.

1. **Is the software used to preprocess/clean/label the instances available?** *(If so, please provide a link or other access point.)*
    
    No.


1. **Any other comments?**
    
    None.





## Uses


1. **Has the dataset been used for any tasks already?** *(If so, please provide a description.)*
    
    The dataset has been used to study stereotypical inferences in language models.

1. **Is there a repository that links to any or all papers or systems that use the dataset?** *(If so, please provide a link or other access point.)*
    
    No.


1. **What (other) tasks could the dataset be used for?**
    
    The dataset could be used for studying stereotypes in generative text inference tasks or overall in language models. 


1. **Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?** *(For example, is there anything that a future user might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other undesirable harms (e.g., financial harms, legal risks)  If so, please provide a description. Is there anything a future user could do to mitigate these undesirable harms?)*
    
    
    This dataset is limited to English and U.S. social stereotypes. 


1. **Are there tasks for which the dataset should not be used?** *(If so, please provide a description.)*
    
    This dataset should not be used for any systems which are deployed for real-users in tasks such as classification. This is a research purpose only dataset.

2. **Any other comments?**
    
    None.




## Distribution


1. **Will the dataset be distributed to third parties outside of the entity (e.g., company, institution, organization) on behalf of which the dataset was created?** *(If so, please provide a description.)*
    
    Yes, the dataset is freely available.


1. **How will the dataset will be distributed (e.g., tarball  on website, API, GitHub)?** *(Does the dataset have a digital object identifier (DOI)?)*
    
    The dataset is free for download at https://github.com/AnnaSou/stereotypes_generative_inferences.


1. **When will the dataset be distributed?**
    
    The dataset is distributed as of May 2022 in its first version.


1. **Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?** *(If so, please describe this license and/or ToU, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms or ToU, as well as any fees associated with these restrictions.)*
    
    The dataset is licensed under a MIT license.


1. **Have any third parties imposed IP-based or other restrictions on the data associated with the instances?** *(If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms, as well as any fees associated with these restrictions.)*
    
    Not to our knowledge.


1. **Do any export controls or other regulatory restrictions apply to the dataset or to individual instances?** *(If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any supporting documentation.)*
    
    Not to our knowledge.


1. **Any other comments?**
    
    None.





## Maintenance


1. **Who is supporting/hosting/maintaining the dataset?**
    
    Trista Cao and Anna Sotnikova are maintaining. Sotnikova is hosting on github.


1. **How can the owner/curator/manager of the dataset be contacted (e.g., email address)?**
    
    E-mail addresses are at the top of this document.


1. **Is there an erratum?** *(If so, please provide a link or other access point.)*
    
    Currently, no. As errors are encountered, future versions of the dataset may be released (but will be versioned). They will all be provided in the same github location.


1. **Will the dataset be updated (e.g., to correct labeling errors, add new instances, delete instances')?** *(If so, please describe how often, by whom, and how updates will be communicated to users (e.g., mailing list, GitHub)?)*
    
    Same as previous.


1. **If the dataset relates to people, are there applicable limits on the retention of the data associated with the instances (e.g., were individuals in question told that their data would be retained for a fixed period of time and then deleted)?** *(If so, please describe these limits and explain how they will be enforced.)*
    
    No.


1. **Will older versions of the dataset continue to be supported/hosted/maintained?** *(If so, please describe how. If not, please describe how its obsolescence will be communicated to users.)*
    
    Yes; all data will be versioned.


1. **If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so?** *(If so, please provide a description. Will these contributions be validated/verified? If so, please describe how. If not, why not? Is there a process for communicating/distributing these contributions to other users? If so, please provide a description.)*
    
    Errors may be submitted via the bugtracker on github. More extensive augmentations may be accepted at the authors' discretion.


1. **Any other comments?**
    
    None.


