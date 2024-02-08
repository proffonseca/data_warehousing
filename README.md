# data_warehousing
Repository for assignments created for DSSA 5102
****
****
Where is the data from? ​Dr. Innocensia Owuor posted the .csv to Figshare. She obtained the data set from the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University

How was it collected?​The data is aggregated from a variety of sources, including WHO, US CDC, and WorldoMeters (full list is here:https://github.com/CSSEGISandData/COVID-19) 

How was it extracted?​I downloaded the data from Dr. Owuor's Figshare posting.

What program was used to clean the data?​ R

How was the data cleaned or transformed? Be specific.​ Data types were a mix of numbers and integers. I used sapply and lapply from the tidyverse library to first identify integers and then convert them to numbers. The "month" column was a factor, so I used as.Date from the lubridate library to convert that column to a date. In preparation for this data being used in a SQL database, I then used tolower to convert all column titles to lowercase. 

What are the units of the numeric data? The numeric data are counts of positive COVID tests.

What were the formulas used in column creation?​ I did not create any new columns

How is the data validated to ensure consistency?​ Much of the data had already been validated by Johns Hopkins and Dr. Owuor. The main issue with consistency was the data types, which were corrected in the steps listed above. To make sure the sapply and lapply worked as expected, I printed the data types and manually confirmed the change.

What are the definitions for the column names? Include all columns in your dataset.​The column names are the names of individual countries.

If there are set variable options in your dataset, what are thier definitions? ​There are no set variables.

What are the regulations to using the data? The data is a part of the Creative Commons

OWUOR, I. (2022). S1_COVID19 data. figshare.
