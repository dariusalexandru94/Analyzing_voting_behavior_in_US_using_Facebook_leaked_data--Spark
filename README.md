# Analyzing voting behavior in United States using Facebook leaked data

This study aims to analyze voting behavior in United States
relying on a one million records dataset with data collected
from Facebook personal profiles of US citizens after a
security breach in 2021. 
* Firstly, It aims to classify each individual from dataset in two groups (democrats and republicans) using **a simple rule-based classification approach** based on the RESIDENCE (state) and GENDER;
* Finally, I will try to obtain **insights regarding the voting behavior of voters in the U.S.A.**

## About dataset

* The most recent Facebook data breach happened in April 2021, when personal data pertaining to 533 million Facebook users was made public on an online forum. This information, which included names, phone numbers, and more, was originally scraped using Facebook's contact importer in 2019;

* A Facebook spokesperson said that the data had been scraped because of a vulnerability that the company patched in 2019. A user, in a low-level hacking forum, published the data for free;

* The exposed data includes the personal information of over 533 million Facebook users from 106 countries. It includes their phone numbers, Facebook IDs, full names, locations, birthdates, bios, and, in some cases, email addresses;

* For this study, I have focused just on data about U.S. citizens. From the original dataset I have deleted the phone numbers and email addresses and also, I have shuffled the the values from every column in order to not expose any real personal data. Also, I have shuffled the user_id for the exact same reason. **NO REAL PERSON CAN BE IDENTIFIED USING THIS STUDY.**

* Atributtes of the dataset are:
1. **uid** - User id;
2. **firstname** - Firstname of the user;
3. **lastname** - Lastname of the;
4. **gender** - Gender of the user;
5. **residence** - Residence state of the user;
6. **birthplace** - Birthplace state of the user;
7. **relationship** - Relationship status of the user;
8. **workplace** - Workplace of the user.

## Related work

There is a lot of scientific research that addresses the issue of voting behavior in U.S.A. 
However, these studies investigate the historical or social perspectives related to voting.

But with the phenomenon of digitization, political parties have seen an opportunity in studying open source data in order to create national databases of voters, collecting information from many sources to create detailed profiles of voters with thousands of data points and build models that predict people’s stances on issues or candidates.

**Political campaigns can use this data to help decide whom to target in their outreach efforts, how to reach them and how they might respond to certain messages.**

**It is clear that political parties use Big Data to study voters behavior, but such studies are not presented online. Moreover, the use of social networks data for political purposes is a sensitive topic. This trend started only in 2016 when the Russians influenced the presidential elections in the United States using Facebook.**

## Implementation

The main purpose of this paper is to analyze voters behavior in United States. In order to do so, I have constructed **a simple rule-based classifier** based on RESIDENCE state and GENDER of each individual.

**Red states vs blue states vs swing states**<br>
Starting in the 2000 United States presidential election, the terms "red state", "blue state" and "swing state" have referred to U.S. states whose voters predominantly and traditionally vote for the Republican Party (red states), Democratic Party (blue states) or which oscillates between those (swing states) in presidential and other elections.

**Partisan advantages by gender**<br>
In general, women lean Democratic while support among men is roughly evenly split between the two parties.

For this study I have used **Spark** because it provides a faster and more general data processing platform, leting you to run programs up to 100x faster in memory, or 10x faster on disk, than Hadoop. **(in reality is just like 2X faster)**
