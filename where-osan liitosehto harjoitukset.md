# where_osan liitosehto harjoitukset

# kysymys 1
select country.name as "country name", airport.name as "airport name"
from country, airport
where airport.iso_country = country.iso_country
and country.name = "Iceland";
