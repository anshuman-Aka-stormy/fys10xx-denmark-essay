# FYS10XX real-energy data package

## Student file

`FYS10XX_energy_data_2010_2024.csv`

This teaching subset contains:

- 8 countries: Brazil, China, Denmark, Germany, India, Kenya, Norway, United States
- 15 years: 2010-2024
- 120 rows
- 16 documented columns
- no missing values in the selected columns

## Data provenance

- Dataset: Our World in Data, Energy Data
- Downloaded: 21 June 2026
- Dataset URL: https://owid-public.owid.io/data/energy/owid-energy-data.csv
- Codebook URL: https://raw.githubusercontent.com/owid/energy-data/master/owid-energy-codebook.csv
- Main underlying source for the electricity variables: Ember, Yearly Electricity Data
- Ember source page: https://ember-energy.org/data/yearly-electricity-data/

The exact source for each column is recorded in `FYS10XX_energy_data_dictionary.csv`.

## Processing

Only selection and ordering were performed:

1. eight countries selected,
2. common period 2010-2024 selected,
3. sixteen variables selected,
4. rows sorted by country and year,
5. index reset.

No numerical values were altered.

## Required source line below a graph or table

> Source: Our World in Data Energy Data, based on Ember Yearly Electricity Data and other documented sources; course subset accessed 21 June 2026. Country/countries: [names]. Year(s): [years]. Unit: [unit].

## Release rule

Always release together:

- the CSV,
- the data dictionary,
- this README,
- `SOURCE_RECORD.json`,
- the data-reference notebook.

Every real-data result must state source, country, year, variable, unit and any filtering or processing.
