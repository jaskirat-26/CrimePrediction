Hi
I was motivated to work on real life data based on crime. I wanted to predict the type of crime that can occur at a specific location at a given time.

I faced the following problems:
  1. The data was completely random, there were no clear distinctions based on time or location in the beginning.
  2. The dataset was large, thus visualising it was difficult.
  3. I did not know which models would be best to implement.
  4. Which factors should I use to train the model?
  5. What to do with Null values.

After some further inspection of the data I decided to do the following:
  1. I chose the following crimes for my model:
        {Primary Type}               {Description}              {IUCR Code}
     a.   Narcotics            (Found Suspect Narcotics)           2093
     b.   Burglary                 (Home Invasion)                 0650
     c. Deception Practice        (Credit Card Fraud)              1150
     d.    Theft                     (Retail Theft)                0860
     e. Criminal Damage              (To Vehicle)                  1320
  2.The following would be the inputs:
     a. Latitude
     b. Longitude
     c. Location Description
     e. Hour of Day

  
I did the following steps during *PreProcessing* of data:
  1. I dropped the columns which were not of use to me in MS EXCEL:'ID', 'Case Number', 'Arrest', 'Domestic', 'Beat', 'District', 'Ward', 'Community', 'FBI Code', 
     'X-Cordinate', 'Y-Cordinate', 'Updated On','Year' and 'Location'.
  2. After uploading this csv file onto my jupyter notebook I took the mean of lattitude and longitude to replace the null values with mean.
  3. Using dummy encoding I made columns for the outputs.
  4. Using Label Encoder I encoded my 'location description' column.
  5. Then I converted date to: hour of day, day and day of week.
  6. After dropping the extra columns I proceeded to save the file as 'Final_Dataset'
  
  
The Prediction:
   1. 
