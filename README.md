### Overview

The goal of this exercise is to investigate the forest fire dataset. The goals that were achieved was exploratory data analysis and creating a multiple class classification model that can predict the cause of forest fire based on the location, the date and the size of the fire. 

### Data Acquisition 

The dataset if public Kaggle dataset that came in SQLite format. It is extremely large, relevant columns were extracted into pandas dataset, it was transferred into csv for temporary use and transfer between notebooks. The repository does not contain said csv because their size was still too large to upload. Another dataset containing sets of coordinates and climate zones was downloaded from Hans W. Chen personal website, but it ended up not being used, since applying it to existing dataset via proximity function took extremely long time. 

### EDA

The dataset only has missing values in "county" column. None of the null counties appeared at top 50 most hazardous counties. Observations were made on forest fire number of incidents, the total area of forest fires that occured each year, of distribution of forest fires through counties and through coordinates. The last one basically covered the entire country, which is undestandable since the dataset covered 23 years worth of data. 

### Modeling

Due to extreme size of the dataset, only basic modeling was finished. Extra Trees classifier was able to predict the cause of a forest fire with 60% accuracy which is significant improvement over 23% baseline theory. The model is extremely overfit. 

### Conclusion and recommendations

The dataset is extremly large and any major adjustments require a lot of processing power. I think it would make sense to split the dataset in some way, the most sense would make either by the year or using the climate zones. The climate zone overall looked very promising and it was a real shame that I was unable to optimize it or at least run this function once and record it into a dataset. Splitting the dataset arbitrarily, applying function to parts and sewing it back together could also achieve same result. Unfortunatelly I was unable to make any proper predictions or create an unsupervized model that would produce any meaningful results as I originally planned. I also was unable to find comprehensive government spending data which could lead to some fun speculations. 