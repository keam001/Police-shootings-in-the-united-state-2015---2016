Police Shootings in the United States (2015-2016)
Overview

This project analyzes police shooting incidents that occurred in the United States during the years 2015 and 2016. 
The goal is to provide insights into the frequency, distribution, and characteristics of these incidents, 
exploring factors such as race, gender, location, and the nature of the incidents.
Dataset

The dataset used for this analysis includes records of police shootings reported in the United States from 2015 to 2016. 
The data contains various attributes for each incident, including:

    Date: The date of the incident
    State: The state and city where the incident occurred
    Race: The race of the individual involved in the incident
    Gender: The gender of the individual involved
    Incident Type: A description of the incident (e.g., armed, unarmed)
    Outcome: The outcome of the incident (e.g., fatal, non-fatal)

Objectives

    Analyze the number of police shootings per year, month, and state.
    Examine the demographic breakdown (race and gender) of individuals involved in shootings.
    Investigate trends and patterns in police shooting incidents over the specified period.
    Visualize the data using charts and graphs to convey findings effectively.

Requirements

To run the analysis and generate visualizations, ensure you have the following Python libraries installed:

    pandas
    matplotlib
Usage

    Load the Dataset: Load the CSV file containing the police shooting data.
    Data Preprocessing: Clean and preprocess the data, handling any missing values and converting date columns to datetime format.
    Analysis: Use groupby operations and visualizations to analyze the data based on the outlined objectives.
    Visualizations: Generate plots to illustrate key findings, such as the distribution of shootings by state and demographic breakdowns.

Example Code Snippet

python

import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_csv('police_shootings_2015_2016.csv')

# Convert date column to datetime
data['date'] = pd.to_datetime(data['date'])

# Count incidents by year
incidents_per_year = data['date'].dt.year.value_counts()

# Plot incidents per year
incidents_per_year.plot(kind='bar')
plt.title('Police Shootings Incidents per Year (2015-2016)')
plt.xlabel('Year')
plt.ylabel('Number of Incidents')
plt.show()

Conclusion

This analysis provides a comprehensive overview of police shootings in the United States for the years 2015 and 2016. By examining the data, we can gain insights into the prevalence and patterns of police shootings, contributing to discussions about policing practices and social justice.
License

This project is licensed under the MIT License - see the LICENSE file for details.
  
