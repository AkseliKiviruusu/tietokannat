# where_osan liitosehto harjoitukset

# kysymys 1
select country.name as "country name", airport.name as "airport name"
from country, airport
where airport.iso_country = country.iso_country
and country.name = "Iceland";
![Näyttökuva 2024-09-06 144737](https://github.com/user-attachments/assets/9edcd437-cd0c-42e6-987d-9708443c7f96)

# kysymys 2
select airport.name as "airport name"
from country, airport
where airport.type = "large_airport"
and airport.iso_country = country.iso_country
and country.name = "France";
![image](https://github.com/user-attachments/assets/53ac8d9c-6dca-4890-914c-d4f001e3cfd4)

# kysymys 3
select country.name as "country_name", airport.name as "airport_name"
from country, airport
where airport.iso_country = country.iso_country
and country.continent = "AN";
![image](https://github.com/user-attachments/assets/e0a069ae-6ad6-4a40-b3a1-0390714c21c8)
