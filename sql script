Look through [Previous Repository](https://github.com/temidataspot/england-health-index-etl-sql) on the ETL Process in loading this data to SQL

# SQL Analysis

```sql
-- Get regional data for 2020 considering null region values
SELECT   
  area_name,
  life_expectancy_pe3,
  access_to_services_pl
FROM `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2020`
WHERE region IS NULL;

-- Get regional data for 2021 considering null values
SELECT 
  area_name,
  life_expectancy_pe3,
  access_to_services_pl
FROM `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2021`
WHERE region IS NULL;

-- Compare 2020 vs 2021
SELECT 
  a.area_name,
  a.life_expectancy_pe3 AS life_expectancy_2020,
  b.life_expectancy_pe3 AS life_expectancy_2021,
  a.access_to_services_pl AS access_to_services_2020,
  b.access_to_services_pl AS access_to_services_2021
FROM `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2020` a
JOIN `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2021` b
  ON a.area_name = b.area_name
WHERE a.region IS NULL;

-- Living conditions comparison
SELECT 
  a.area_name,
  a.living_conditions_pl AS living_conditions_2020,
  b.living_conditions_pl AS living_conditions_2021,
  a.access_to_services_pl AS access_to_services_2020,
  b.access_to_services_pl AS access_to_services_2021
FROM `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2020` a
JOIN `temiloluwa-jokotola-projects.england_health_index_dataset.Health_Index_2021` b
  ON a.area_name = b.area_name
WHERE a.region IS NULL;
```

# Visualizing on Looker
Dashboard 1: [Service Access and Life Expectancy](https://lookerstudio.google.com/s/vK-RRUSO1oU)
Dashboard 2: [Service Access and Living Conditions](https://lookerstudio.google.com/s/opyC8X47WYM)

# Further Reading
Read more details on analysis, insights and implications on [Medium](https://medium.com/@temiloluwa.jokotola/englands-2020-2021-health-index-service-access-living-conditions-and-life-expectancy-0d7ec577fbdf)
