# data_warehousing
## Repository for assignments created for DSSA 5102
****
****
### Data Source
The COVID case number data was posted on Figshare by Dr. Innocensia Owuor. The data is aggregated from a variety of sources, including the WHO, US CDC, and WorldMeters. (Tje full list is available on the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University [GitHub repository] (https://github.com/CSSEGISandData/COVID-19). I downloaded the .csv on 24 January 2024.

###Data Cleaning
I used​ R to clean the data. Data types were a mix of numbers and integers. I used sapply and lapply from the tidyverse library to first identify integers and then convert them to numbers. The "month" column was a factor, so I used as.Date from the lubridate library to convert that column to a date. In preparation for this data being used in a SQL database, I then used tolower to convert all column titles to lowercase. To make sure the sapply and lapply worked as expected, I printed the data types and manually confirmed the change.

### Data Use
The data is a part of the Creative Commons
OWUOR, I. (2022). S1_COVID19 data. figshare.
