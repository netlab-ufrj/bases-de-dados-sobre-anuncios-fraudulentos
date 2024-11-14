# Datasets of scam and fraudulent ads served on Meta platforms

[![Static Badge](https://img.shields.io/badge/lang-pt-blue?style=flat)](https://github.com/netlab-ufrj/bases-de-dados-sobre-anuncios-fraudulentos/blob/main/README.md)
[![Static Badge](https://img.shields.io/badge/lang-en-red?style=flat)](https://github.com/netlab-ufrj/bases-de-dados-sobre-anuncios-fraudulentos/blob/main/README.en.md)

## About the project

**_[The Disinformation Industry Observatory and its impact on consumer relations in Brazil](https://netlab.eco.ufrj.br/en/observatorio-industria-desinformacao)_** is a project established in partnership between NetLab UFRJ and Brazil’s National Consumer Secretariat of the Ministry of Justice and Public Security (Senacon/MJSP) which aims to provide input that can support public policies and transparency parameters to protect consumers and advertisers based on analyses of digital platform data infrastructure and case studies on scam and fraudulent advertising on social media platforms in Brazil.

## Studies on fraudulent ads developed at the observatory

With a view to addressing the project’s **specific objective II** (“_Develop research on fake ads and the disinformation ecosystem that culminates in financial operations, based on evidence based on data and scientific methods_”), we published two studies, available on the **[NetLab UFRJ website](https://netlab.eco.ufrj.br/en/observatorio-industria-desinformacao)**, namely:

1. **_Fake ads, their mechanisms and potential harm to Brazilian consumers_**, in which we detail six different case studies on fraudulent and irregular ads which appropriate the images of public and private institutions and organizations, politicians and other well-known figures in order to convey trust;

2. **_Ecosystem of disinformation that culminates in financial operations_**, in which we present four different case studies detailing the serving of scam advertisements about two government programs: _Desenrola Brasil_ and _Voa Brasil_.

Both studies are based on advertising data from **Meta platforms** (Facebook, Instagram, Messenger and Audience Network) as the Meta Ad Library is the only systematic source of information for advertising on digital platforms in Brazil with a searchable and navigable system of ad data.

This does not mean that the problems exposed are not to be found on other platforms, only that they do not have robust transparency policies in Brazil: opacity makes platforms without transparency more attractive to fraudsters and scammers. 

## About the datasets

With the datasets made available in this repository and following the precepts of **open science**, the project’s **specific objective III** was achieved (“_Create a data repository with fake or fraudulent accounts and pages in which advertisers deceive consumers, steal their data, make them suffer financial losses, scams or any other type of material or moral loss or damage_”), and it provided the basis for the preparation of the **studies previously described**.

In total, there are ten CSV datasets, named according to the following pattern:

`studyn_casey.csv`

Where **_n_** refers to the study in question, while **_y_** refers to a case from that study, in the order in which it is presented. For example, the file _study2_case3.csv_ refers to data from the **third case of the second study**.

All data on **commercial and political ads** was sourced from the **Meta Ad Library**.

### Data dictionary

To facilitate handling, we have grouped and consolidated these datasets according to a common dictionary, namely:

| Field         | Description |
| ------------- |:-------------|
| **ad_id**      | Unique identifier of the ad. |
| **ad_url**     | Unique URL to access the ad in the Meta Ad Library user interface. Please note that ads not tagged as political are not stored in the repository. |
| **ad_start_date** | Date the ad was first served. |
| **ad_end_date** | Date the ad stopped being served, or, in the absence of this information, the date it was last seen in the Meta Ad Library user interface. |
| **page_id** | Unique identifier of the advertiser page. |
| **page_name** | Advertiser page name. |
| **sponsor_name** | Name registered by whoever financed the ad on Meta platforms, in the case of ads originally tagged as political. |
| **publisher_platforms** | Meta platforms in which the ad was served. |
| **ads_with_same_creative_text** | In the case of manual data collections of ads not tagged as political from the Meta Ad Library user interface, the number of ads identical to the identified ad. |
| **political_disclaimer** | Indicates whether the ad was tagged as political or not, and therefore whether it was collected from the Meta Ad Library user interface or, in the case of political ads, from the Meta Ad Library API. |

Fields filled with - indicate problems in data recovery or non-applicability.

## Usage permissions and contact

The datasets may be investigated and analyzed free of charge for non-commercial teaching and research purposes. All datasets comply with the **_[Brazilian General Data Protection Law](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)_** and are composed solely of data previously made public through Meta Ad Library. Any problems or questions should be sent by email to **netlab@eco.ufrj.br**.
