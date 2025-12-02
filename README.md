# BDV Visualization Project: Crime Data
https://www.kaggle.com/datasets/utkarsh1093/crime-data-from-2020-to-nov2025

> Since the unmodified CSV file is very large (300 MB) and therefore can not be checked into Git,
> you need to convert the parquet file yourself.
> Please paste the CSV file into the `data/` folder named like `Crime_Data_from_2020_to_Present.csv`.
> The modified CSV file used for the visualizations will be included in this repository.

## Data
The dataset contains crime data from 2020 to November 2025, sourced from Kaggle. 
It includes various types of crimes reported in LA.
The original dataset can be found in `data/Crime_Data_from_2020_to_Present.parquet`.#
It was [converted](https://www.agentsfordata.com/parquet/to/csv) to the CSV.

The data contains the following columns, not all of them are used in the 
visualizations and are therefore removed in `data/data.csv`:

- DR_NO: Unique LAPD incident number used to identify each crime report.
- Date Rptd: The date the crime was reported to the police.
- DATE OCC: The date the crime occurred.
- TIME OCC: Time of occurrence in 24-hour format.
- AREA: Numerical code for the LAPD geographic division where the incident occurred.
- AREA NAME: Name of the LAPD division (for example, N Hollywood, Central, Pacific).
- Rpt Dist No: Reporting district number, representing a smaller neighborhood unit within an LAPD area.
- Part 1-2: Crime classification category.
   - Part I includes serious crimes such as homicide, robbery, burglary, and aggravated assault.
   - Part II includes less severe offenses such as fraud, vandalism, and simple assault.
- Crm Cd: Numeric code identifying the primary crime.
- Crm Cd Desc: Description of the primary crime type (for example, Theft of Identity, Burglary, Simple Assault).
- ~~Mocodes: Method of Operation codes that describe how the crime was committed.~~
- Vict Age: Age of the victim.
- Vict Sex: Sex of the victim (Male, Female, Unknown).
- Vict Descent: Victim’s descent or ethnic background (for example, Hispanic/Latin/Mexican, White, Black, Asian).
- Premis Cd: Numeric code for the type of location where the crime occurred.
- Premis Desc: Description of the premise or location type (for example, Sidewalk, Single Family Dwelling).
- Weapon Used Cd: Numeric code for the weapon used, if any.
- Weapon Desc: Description of the weapon used (for example, Knife, Handgun, Unknown).
- Status: Case status code.
- Status Desc: Full description of the case status (for example, Invest Cont, Adult Arrest, Juvenile Arrest).
- ~~Crm Cd 1: Additional crime code associated with the incident (if applicable). Often the same as Crm Cd for single-offense cases.~~
- ~~LOCATION: Address or block description where the incident occurred.~~
- ~~LAT: Latitude coordinate for the location.~~
- ~~LON: Longitude coordinate for the location.~~
- occ_year: Year extracted from DATE OCC.
- occ_month: month extracted from DATE OCC.
- occ_date: Day of the month extracted from DATE OCC.
- occ_day: Day of the week of the occurrence date (for example, Mon, Tue, Sat).
