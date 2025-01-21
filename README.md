
![](https://user-images.githubusercontent.com/970858/63474771-d6734700-c469-11e9-83bb-9429da563909.png)

# LAB-MYSQL-Query-Optimization

## Requirements

- [Learn how to fork this repo](https://guides.github.com/activities/forking/)
- Clone this repo into your `code/labs` folder
- Have MySQL installed
- Have Worbench installed

## Queries :

- Calculate the average power of the weapons assigned to each Imperial team.

- Get the total strength of the Rebel teams stationed at each base.

- List all weapons with power greater than 75 and the Imperial teams to which they are assigned.

- Get a summary of all planned attacks, including the probability of success and the Imperial and Rebel teams involved.

- List all Rebel teams and the probabilities of success of the attacks in which their bases are involved.

- List the planned attacks with a success probability greater than 70%, including target base information and the assigned Imperial team.

## Vistas

- Find the Imperial team with the highest and lowest total strength
  
- List all Rebel teams that have more than 2 members, ordered by the total number of members (Table RebelTeamMembers With Join).

- Get all intelligence information about bases with a high-security level.

- Get a summary of the resources available at each location, grouped by the location.

- List all Imperial teams and the total number of weapons assigned to each team, ordered by the total number of weapons.

## Subquerys

### Returns the name of the imperial team that has the highest average power of assigned weapons. Includes the average power.

As you have seen subqueries are a powerful tool in SQL that allow you to solve complex problems.However, as queries become more advanced, these subqueries can become difficult to read, maintain and debug.To solve these problems, we can introduce views.

### Create a view Weapons used in successful attacks

**Step 1**: Create a view to calculate the average success probability of attacks.

**Step 2**: Use the view to filter weapons assigned to teams in successful attacks.

 
### Create a view Rebel teams in bases with the lowest security level

**Step 1**: Create a view to identify bases with the lowest security level.

**Step 2**: Use the view to find the rebel teams assigned to these bases.

### Create a view Imperial teams without assigned weapons

**Step 1**: Create a view to identify imperial teams with assigned weapons.

### Create a view to identify bases with imperial teams.



## Bonus

1. Rebel teams with more soldiers than the average

**Step 1**: Create a view to calculate the average length of intelligence details.

**Step 2**: Use the view to find bases with details longer than the average.




