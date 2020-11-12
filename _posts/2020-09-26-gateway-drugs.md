---
layout: post
title: Gateway Drugs
---

9/26/2020

The Gateway effect of Alcohol, Tobacco, and Marijuana:  Does the Use of Legal Drugs Increase the Risk of Illegal Drug Use?

## Abstract
Alcohol and tobacco are legal, and marijuana is becoming legal in more states every year. Regardless of legality, they are widely available to users of all ages. This begs the question: do users of alcohol, tobacco, and/or marijuana tend to move on to harder illegal drugs such as heroin and cocaine? In this study, I used data analysis, statistics, and machine learning to answer this question. I used data obtained from the Center for Behavioral Health Statistics and Quality that includes responses for questions about demographics, tobacco use, alcohol use, marijuana use and illicit drug use, including historical and current habits of each individual respondent. 

With alcohol and tobacco available legally, and marijuana available legally in some states, it is important to know what the effects these drugs have on people and society overall. Healthcare professionals and teachers can use this information to educate children about the dangers of legal as well as illegal drugs. Also, medical professionals, rehab centers, and health insurance companies can learn about the risks of drug use. After analyzing the data, I hope to answer the question: does the use of legal drugs increase the use of illegal drugs?
## Data Source
I used a data source from the Center for Behavioral Health Statistics and Quality, National Survey on Drug Use and Health 2015 (NSDUH-2015-DS0001) (Center for Behavioral Health Statistics and Quality, n.d.). This data set includes 2,679 columns and 57,146 rows. It includes responses for questions about demographics, tobacco use, alcohol use, marijuana use, and illicit drug use, including historical and current habits of each. Using feature selection, I narrowed down the data set to five imputed fields (see Appendix). These fields include answers to questions about legal and illegal drug use, particularly if the respondent ever in their life tried alcohol, tobacco, marijuana, and/or any harder drugs. The harder drugs field was created using questions about cocaine, heroin, and methamphetamines.
## Background
According to the DSM 5 (Diagnostic and statistical manual of mental disorders, 5th edition), substance use disorders can be split up into different types of drugs (alcohol, caffeine, cannabis, hallucinogens, inhalants, opioids, sedatives, stimulants, tobacco, and other or unknown) (2013). A patient must fit criteria for substance use disorders, which include 11 different criteria in how the drug use affects their life. Using these criteria, a healthcare professional can determine the severity of a patient’s disorder by how many of the criteria they meet. For the purpose of this study, I am not looking at the severity of the substance use disorder. I am only looking at whether or not the subject ever tried a drug in their lifetime. For simplicity, I am grouping the drugs into tobacco, alcohol, cannabis, and harder drugs (cocaine, heroin, and methamphetamines). 
Many studies exist in the subject area of gateway drugs. It is common knowledge that marijuana is a gateway drug. One study suggests that alcohol, tobacco, and marijuana are all three gateway drugs (American Addiction Centers, 2019). In fact, this study concluded that alcohol is a higher risk gateway drug than marijuana. Other studies show that alcohol, tobacco, and marijuana can all be gateway drugs at varying degrees (Kirby & Barry, 2012) (National Institutes of Health, 2011) (NIDA, 2020).
## Methodology
After exploring the data set, I found that only 11.7% of the respondents had ever tried hard drugs, while 56.2% tried tobacco products, 72.8% tried alcohol, and 42.5% tried marijuana. I under-sampled the respondents that had never tried hard drugs to create a dataset with 50/50 on the HARDFLAG field. After testing several models, I determined that the most accurate is a logistic regression model. Using a logistic regression model on this balanced dataset returned an accuracy of 84% (1,445 true positives, 548 false positives, 107 false negatives, and 1,944 true negatives). The ROC (Receiver Operating Characteristic) curve for the model shows a much higher accuracy than purely random.
## Conclusion
Tobacco, alcohol, and marijuana can each be a gateway drug by themselves, but put together, they are a strong indicator of use of heavier, illegal drugs. This may suggest that making only harder drugs illegal is not a deterrent to their use. After trying one or all of the three legal drugs, it is common for the respondent to also try harder, illegal drugs, suggesting that the legality and danger of the drug is less of a factor than the fact that they are drugs. 
## References
American Addiction Centers. (2019). The Real Gateway Drug. Retrieved August 29, 2020, from https://americanaddictioncenters.org/the-real-gateway-drug

American Psychiatric Association. (1994). Diagnostic and statistical manual of mental disorders (4th ed.). Washington, DC: American Psychiatric Association.

Center for Behavioral Health Statistics and Quality. (n.d.). 2015 National Survey on Drug Use and Health (NSDUH): Survey Materials. Substance Abuse and Mental Health Services Administration, Rockville, MD.

Center for Behavioral Health Statistics and Quality. (n.d.). National Survey on Drug Use and Health 2015 (NSDUH-2015-DS0001). Retrieved August 29, 2020, from https://www.datafiles.samhsa.gov/study-dataset/national-survey-drug-use-and-health-2015-nsduh-2015-ds0001-nid16894

Center for Behavioral Health Statistics and Quality. (2014). 2015 National Survey on Drug Use and Health (NSDUH): CAI Specifications for Programming (English Version). Substance Abuse and Mental Health Services Administration, Rockville, MD.

Center for Behavioral Health Statistics and Quality. (2014). 2015 National Survey on Drug Use and Health (NSDUH): Screener Specifications for Programming (English Version). Substance Abuse and Mental Health Services Administration, Rockville, MD.

Center for Behavioral Health Statistics and Quality. (2018). 2015 National Survey on Drug Use and Health Public Use File Codebook, Substance Abuse and Mental Health Services Administration, Rockville, MD.

Kirby, T., & Barry, A. E. (2012). Alcohol as a gateway drug: a study of US 12th graders. The Journal of school health, 82(8), 371–379. Retrieved August 29, 2020, from https://pubmed.ncbi.nlm.nih.gov/22712674/

National Institutes of Health. (2011). Why Nicotine is a Gateway Drug. Retrieved August 29, 2020, from https://www.nih.gov/news-events/nih-research-matters/why-nicotine-gateway-drug

NIDA. (2020). Is marijuana a gateway drug?. Retrieved August 29, 2020, from https://www.drugabuse.gov/publications/research-reports/marijuana/marijuana-gateway-drug.

NIDA. (2020). Marijuana Research Report. Retrieved August 29, 2020, from https://www.drugabuse.gov/download/1380/marijuana-research-report.pdf?v=87b7363dc6bd7b778ecd726d0f3d8f26
