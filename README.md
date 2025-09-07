# Adult butterfly data for Lepidoptera monitoring in the Sierra Nevada
Adult butterfly data associated with Lepidoptera monitoring program in the Sierra Nevada, USA. For project description, see: https://www.westernbutterflies.org/

Details below for three data files:
PA_1972to2024_AllSites.csv
counts_1999to2024.csv
zones_2019to2024.csv


#############################
## PA_1972to2024_AllSites.csv (split into 5 equal parts)
#############################

This is our core data, consisting of presence and absence observations conducted biweekly for 163 species of butterflies across 11 sites, forming a roughly east-west transect across Northern California and into western Nevada. Columns of data are detailed below.

Site_name: the 11 sites.

visit_date: the date that an observation was recorded, in year-month-day format.

genus_species: individual taxa, either present or absent on a day at a site.

pa: 0 for absent, 1 for present; note than an absence for a given species at a particular site on a given day does not mean that a species has ever been present at that site, because zeros are imputed for absences across species and sites.

ordDate: the ordinal day of the observation, counting from the first of the year.

Year: year of observation.

Month: month of observation.

Observer: initials of individual recording observations.


#############################
## counts_1999to2024.csv (split into 2 equal parts)
#############################

For the 5 lower-elevation sites, counts of individuals have been recorded, in addition to presence and absence. The structure of this file is identical to the previous (see description of PA_1972to2024_AllSites.csv), with the exception that there is now a "count" column (counts of individuals), and the column for ordinal date is labelled as "day" rather than "ordDate."

 

#############################
## zones_2019to2024.csv
#############################

At the 6 higher-elevation sites, we have (in recent years) recorded presence not just at the whole site level, but separately within habitat zones at each site. Columns of data are detailed below.

Day: day of the month.

Month: month of observation.

Year: year of observation.

site_name: one of six locations.

genus_species: individual butterfly taxa.

PA: presence data, and note that four values are possible (0, 1, 2, and 3). Zero is absent, 1 indicates a species present with only one individual on a given day; 2 indicates two individuals; 3 indicates 3 or more individuals on that day.

Zone: habitat breakdown by site, with names mostly arbitrary (e.g., "1Valley") and should be treated as an unordered, categorical variable.

Observer: initials of individual recording observations.


