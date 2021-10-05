---
layout: post
title: "Golden Gate Protocol Progress"
date: 2021-10-05
---

I have been making great progress towards creating a Golden Gate Assembly protocol for the opentrons robot. First, I have modified the input files so that each fragment is either amplified or digested independently. The protocol also has the new unique feature of being able to handle assemblies that include pcr amplified fragments as well as linearized fragments from enzyme digests. 
One feature that I'm very excited about that I just got worked out today is the pcr conditions calculator. This script loops through every fragment and performs calculations to determine the most suitable pcr extension time and annealing temperature. Today I updated it to be able to calculate annealing temps for every fragment involved to generate one, good annealing temp. This required looping through multiple dataframe, which I have had trouble figuring out until now. I realized that you can create a new datframe with the names of the dataframes that you want to loop through, and then you can use the strings in this new dataframe to loop through dataframes by saving each row as x using iterrows then calling x with locals()[x]
I'm sure that is convoluted and hard to follow, but it is a big break for me and the example can be seen in the code once we release it to the public. 
Looking forward to making an update in a day or two about a completed Golden Gate protocol!
