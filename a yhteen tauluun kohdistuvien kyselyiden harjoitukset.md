# yhteen tauluun kohdistuvien kyselyiden harjoitukset
# kysymys 1
select * from goal;
![image](https://github.com/user-attachments/assets/55abd2ee-5543-49e1-9c0c-77964c34c2b2)

# kysymys 2
select name airport_type from airport where iso_country = "FI";
![image](https://github.com/user-attachments/assets/e8a90033-df4c-439e-8c30-41385a3e6426)

# kysymys 3
select name from airport where iso_country = "FI" order by name;
![image](https://github.com/user-attachments/assets/1a9d957d-4ac1-4ecf-8c6e-397abf6d2bc8)

# kysymys 4
select name, type from airport where iso_country = "FI" order by type, name;
![image](https://github.com/user-attachments/assets/d7ff5647-63fd-4d73-98d8-df3c59d35de8)

# kysymys 5
select name from country where name like "F%";
![image](https://github.com/user-attachments/assets/ccefd36a-4dd3-46b8-8420-2aac9589a941)

# kysymys 6
select name from country where name like "%F%";
![image](https://github.com/user-attachments/assets/d75b282e-a05e-42be-84c9-3002169dc254)

# kysymys 7
select location from game where location like "EGCC";
![image](https://github.com/user-attachments/assets/13b1beb4-339f-468a-832a-8162e70bd915)

# kysymys 8
select co2_consumed from game where co2_consumed like "8000";
![image](https://github.com/user-attachments/assets/137bf3f6-00b0-4322-b17f-614c8592a5c5)

# kysymys 9 
select co2_budget from game where co2_budget like "10000" and id like "1";
![image](https://github.com/user-attachments/assets/84a26694-c6df-412b-8eff-a0bc529b547f)


