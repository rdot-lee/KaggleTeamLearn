## 595. Big Countries
```SQL
select name, population, area from world
where area >= 3000000
or
population >= 25000000;
```

## 175. Combine Two Tables
```SQL
#左邊為主
select firstName, lastName, city, state from Person left join Address on Person.personId = Address.personId;
```

## 176. Second Highest Salary
```SQL

```