# clinicalBERT
This repo is a part of a greater project to scrape clinical trial data, feed it into a BERT language model, and then use the predictions to choose BioTech investments.

## AACT Relational Database 
Duke maintains the Aggregated Analysis of ClinicalTrials.gov (AACT) relational database, which takes the messy clinicaltrials.gov data dumps and makes them useable. Here is their [repo](https://github.com/ctti-clinicaltrials/aact).

## Scraping
This repo uses .txt files easily downloaded from AACT's website. They are then fed into the python script that grabs all the required text from each table and combines it into a labeled text for the BERT model. 

## TODO
Reinforcing the BERT model is the next step and requires clinical trial result data - this comes from information collected on how drugs/treatments/etc. move through the clinical trial system. The sponsor of the trial decides whether they want to go forward with the next phase, so that data is not aggregated anywhere with free access. 

## Dataflow 
Here is a diagram showing the dataflow of the completed project. The greyed-out blocks still need to be completed. 
