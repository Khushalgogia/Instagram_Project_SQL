# Instagram Project


1. Your Task: Identify the five oldest users on Instagram from the provided database.

```
select username from users
order by created_at 
limit 5;
```
![Alt text](image-1.png)

2. Your Task: Identify users who have never posted a single photo on Instagram.

```
select distinct u.id, u.username from users u
left join photos p
on u.id = p.user_id
where p.image_url is null
```
![Alt text](image-2.png)





































