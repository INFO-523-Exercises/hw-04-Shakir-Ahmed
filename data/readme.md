# Tornados:

Data set for Tornados:

### Data Dictionary

# `tornados.csv`

|variable     |class     |description  |
|:------------|:---------|:------------|
|om           |integer   |Tornado number. Effectively an ID for this tornado in this year.|
|yr           |integer   |Year, 1950-2022. |
|mo           |integer   |Month, 1-12.|
|dy           |integer   |Day of the month, 1-31. |
|date         |date      |Date. |
|time         |time      |Time. |
|tz           |character |[Canonical tz database timezone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).|
|datetime_utc |datetime  |Date and time normalized to UTC. |
|st           |character |Two-letter postal abbreviation for the state (DC = Washington, DC; PR = Puerto Rico; VI = Virgin Islands). |
|stf          |integer   |State FIPS (Federal Information Processing Standards) number. |
|mag          |integer   |Magnitude on the F scale (EF beginning in 2007). Some of these values are estimated (see fc). |
|inj          |integer   |Number of injuries. When summing for state totals, use sn == 1 (see below). |
|fat          |integer   |Number of fatalities. When summing for state totals, use sn == 1 (see below). |
|loss         |double    |Estimated property loss information in dollars. Prior to 1996, values were grouped into ranges. The reported number for such years is the maximum of its range. |
|slat         |double    |Starting latitude in decimal degrees. |
|slon         |double    |Starting longitude in decimal degrees. |
|elat         |double    |Ending latitude in decimal degrees. |
|elon         |double    |Ending longitude in decimal degrees. |
|len          |double    |Length in miles. |
|wid          |double    |Width in yards. |
|ns           |integer   |Number of states affected by this tornado. 1, 2, or 3. |
|sn           |integer   |State number for this row. 1 means the row contains the entire track information for this state, 0 means there is at least one more entry for this state for this tornado (om + yr). |
|f1           |integer   |FIPS code for the 1st county. |
|f2           |integer   |FIPS code for the 2nd county. |
|f3           |integer   |FIPS code for the 3rd county. |
|f4           |integer   |FIPS code for the 4th county. |
|fc           |logical   |Was the mag column estimated? |
