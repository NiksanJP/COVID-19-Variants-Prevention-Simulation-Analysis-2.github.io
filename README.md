# COVID-19-Variants-Prevention-Simulation-Analysis-2.github.io
COVID-19 Simulation and Analysis on Unrestricted Environment. This simulation only has the simulation on the original variant and the UK variant and analyzing the difference in spread and preventions.

## URL
https://niksanjp.github.io/COVID-19-Variants-Prevention-Simulation-Analysis-2.github.io/

## Abstract
COVID-19 has ravaged the entire world, instead of case numbers declining the COVID-19 infection 
has been increasing daily. It took around 10 months for 50 million people to get infected and only 
another 2 months for another 50 million to get infected. The rate of infection is on the rise. Unlike 
other types of infections, COVID-19 has been the most widespread which has now spread and 
mutated with more transmissible variants and variants with higher death rate. To manage this crisis 
governments have put unprecedented plans but the effectiveness of the plan’s result can only be 
seen after a week or two [1]. We can use simulations to test in, what these policies effect the COVID19 
cases and Machine-learning to predict new infection numbers using our world data.

## Background and Research problem
We aim to determine how different measures can prevent infection numbers to surge and how 
different the new UK variant (B1.1.7) is compared to the original virus. As the case numbers increase 
around the world so does new variants, due to millions of people getting infected, countries must 
prevent the infection of more infectious variants than the original COVID-19 strain. The null 
hypothesis for this study is the new variant of COVID-19 or UK variant (B1.1.7) is more infectious 
than original strain of the virus and there will not be an effect predicting the covid-19 cases due to 
variants. The alternative hypothesis for this study is there will not be significant difference and cause 
the same number of infection numbers whilst making it harder to predict COVID-19 cases in the 
future. We will check if other factors such as lockdowns make big changes. We will also try to model 
and predict the next 7 days of COVID-19 infections from the past COVID-19 cases

## Approach Description
Firstly, we will need to confirm what happens if no preventive measures are taken place for a 
population of 200, for the normal COVID-19 or SARS-COV-2 (Figure 1), the population entered 
medical emergency at day 10 (frame 100) as seen in Figure 3, whilst the B1.1.7 variant or UK variant 
(Figure 2) took only half that of day 5 (frame 50) as seen in figure 4. From the fist simulation, we can 
see how dangerous the new variant is compared to the first confirmed COVID-19. 
To compare how dangerous the new variant is, we will simulate one population with both normal 
and B1.1.7 UK mutant simulated as in figure 5 and compare it with a population with the two normal 
variants simulated in figure 6. When the infection starts, the B1.1.7 infects most of susceptible 
people and dwarfs the original COVID-19 strain which puts the population of 200 into medical 
emergency before day 5(frame 50) as seen in Figure 7. In the other hand, the population of 200 with 
2 normal covid-19 infections, they only reach medical emergency at around day 9 as seen in figure 8.
Further on, we will look at preventive measures taken place by governments which are Curfews and 
Lockdowns. With curfew at 11p.m., prevention of movement till 6am will result in 30% of movement 
reduction, the results are shown in figure 9 where the population enters medical emergency only 
from day 12 which does not show enough potential to prevent the infection of COVID-19 for the 
normal variant.
Compared to curfews, lockdowns are harsher and are known to prevent sudden infection surge like 
in other simulations. In lockdowns only essential service workers were allowed travel meaning the 
risk to spread or contract the virus itself. As in Figure 10, the simulation shows the population of 200 
entered medical emergency at day 25 which is further than any other simulation showing the most effective infection prevention method. With the help of quick testing and quarantining ones who 
were infected will show the true capability of the measure.
From these simulations, we have found out that COVID-19 cases are directly associated with 
movement, the more movement is reduced, the better is for the population. COVID-19 variants will 
spread faster but if movement is reduced, it seems unlikely to spread widely. We can confidently say 
that from our simulation and conclusions from stage 1. the most important factors of predicting new 
COVID-19 cases movement, testing, positive rate etc.
For us to predict the covid-19 case numbers, we have to pick which features affect the number of 
new cases the most, for example if most cases are confirmed in places of worship and restaurants 
we can feed the model with information that are useful. In this case, we will be using mobility data 
from google [2] which are retail and recreation, grocery and pharmacy, residential, stations, parks, 
workplaces and covid-19 data such as new cases, new deaths, new tests, positive rate, total 
vaccination and population density.
As the infection count grows the higher the chances for the new variant to emerge proving new
problems. New variants were first spotted around April and December 2020, which means if we 
evaluate the data entire dataset, the dataset with and without variants will show similar results. We 
need to train the model so it knows that new variants will be there and make predictions assuming 
them. Therefore, providing the model with the information of the new variants will not be feasible 
as there will be a blank time where researchers will need to research about the variant and then only 
we can feed our model with it. Our data of 1+ year already includes dates where variants spread 
within the population and the model shall learn from these experiences.
In the first stage of the projected we assembled about 18k bytes or 76k rows of “our world in data” 
dataset. The dataset contains each line for every country and every date since 2020 March when the 
pandemic started. We further on collected google mobility data to track how much movement is 
going on a country. This Google mobility dataset is divided into Country, date, movement in retail, 
grocery, residential, transit, parks and workplaces. To determine what features are needed to 
predict COVID-19 infection numbers we will make simulations for different scenarios such as 
Lockdowns, curfews and variants.
For this problem we will use time-series prediction method which is implemented by giving the 
model past 7 days of data (infections, tests, etc..) and the model will predict the next 7 days of covid19 predictions. We will fit our data to two different countries with two very distinct situation which 
are United Kingdom and Japan. UK had very high number of COVID-19 cases with lockdown but UK 
has a swift vaccine roll where 60% have received the first vaccine shot, and Japan where the case 
numbers have been relative low but the vaccine shots have not been anywhere close to UK’s with 
mobility changes such as soft curfew and lockdowns.
