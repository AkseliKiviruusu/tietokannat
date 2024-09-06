# where_osan liitosehto harjoitukset

# kysymys 1
select country.name as "country name", airport.name as "airport name"
from country, airport
where airport.iso_country = country.iso_country
and country.name = "Iceland";
![Näyttökuva 2024-09-06 144737](https://github.com/user-attachments/assets/9edcd437-cd0c-42e6-987d-9708443c7f96)
