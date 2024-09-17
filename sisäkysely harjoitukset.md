# kysymys 1

select country.name
from country
where iso_country in(
select iso_country
from airport
where airport.name like "Satsuma%"
);

![image](https://github.com/user-attachments/assets/8f9e77ed-880e-4d87-9fe3-2f5012ba6f1a)
