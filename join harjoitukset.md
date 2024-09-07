# kysymys 1
select country.name as "country name", airport.name as "airport name"
from airport
inner join country on airport.iso_country = country.iso_country
and country.name = "Finland"
and scheduled_service = "yes";

