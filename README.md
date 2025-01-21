
![](https://user-images.githubusercontent.com/970858/63474771-d6734700-c469-11e9-83bb-9429da563909.png)

# LAB-MYSQL-Query-Optimization

## Requirements

- [Learn how to fork this repo](https://guides.github.com/activities/forking/)
- Clone this repo into your `code/labs` folder
- Have MySQL installed
- Have Worbench installed

## **Warm-Up Queries**
These simple queries will help you get familiar with the tables and data:

- **Calculate the average power of the weapons assigned to each Imperial team.**
- **Get the total strength of the Rebel teams stationed at each base.**
  
<img src="frog.gif" alt="Descripción de la imagen" width="600" >

---

## **Views**

These exercises focus on creating views to simplify complex queries and make them reusable.

1. **Imperial Team with the Highest and Lowest Total Strength**  
   Create a view that identifies the Imperial team with the highest and lowest total strength.

2. **Summary of Resources by Location**  
   Create a view to get a summary of the resources available at each location, grouped by location.

3. **Imperial Teams and Weapon Count**  
   Create a view to list all Imperial teams and the total number of weapons assigned to each team, ordered by the total number of weapons.

     ![kermit-window-meme-template-full-03088594](https://github.com/user-attachments/assets/9a023c2b-c45b-47d6-b44b-bc06769d35c7)


---

## **Transactions**


These exercises will teach you to use transactions to ensure consistency and control over database changes.

1. **Insert and Commit**  
   Insert a new record into the `RebelTeams` table with a unique team name. Commit the transaction to save the changes.

2. **Insert, Update, and Rollback**  
   - Insert a new record into the `ImperialTeams` table.
   - Update the `team_size` of another team.
   - Rollback the transaction to undo all changes.

3. **Multiple Operations with Savepoints**  
   - Perform three operations:
     - Insert into the `RebelTeams` table.
     - Update the `Bases` table.
     - Delete from the `Intel` table.
   - Set a savepoint after each operation.
   - Rollback to the second savepoint and commit the remaining changes.
     
<img src="https://github.com/user-attachments/assets/cad19351-125d-4026-bcb4-88cba89b8d82" alt="Descripción de la imagen" height="400" width="700" >


---
## **Subqueries**

<img src="https://github.com/user-attachments/assets/fa51f17a-3b9a-407c-aa8d-8471bbba5800" width="150" height="200" align="right">


### **Subquery: Imperial Team with the Highest Average Weapon Power**
- Write a subquery that returns the name of the Imperial team with the highest average power of assigned weapons. Include the average power.

**Reflection:**  
Subqueries are powerful, but as queries grow more complex, they can become hard to read, maintain, and debug. To address this, we introduce **views**.



---

<img src="https://github.com/user-attachments/assets/04ed806f-969a-484b-a15c-92b8ca2ae23a" width="300" height="450" align="right">

### **Create and Use Views**

1. **Weapons Used in Successful Attacks**
   - **Step 1**: Create a view to calculate the average success probability of attacks.
   - **Step 2**: Use the view to filter weapons assigned to teams in successful attacks.

2. **Rebel Teams in Bases with the Lowest Security Level**
   - **Step 1**: Create a view to identify bases with the lowest security level.
   - **Step 2**: Use the view to find Rebel teams assigned to these bases.

3. **Imperial Teams Without Assigned Weapons**
   - **Step 1**: Create a view to identify Imperial teams with assigned weapons.
   - **Step 2**: Undefined
     
4. **Bases with Imperial Teams**
   - **Step 1**: Undefined
   - **Step 2**: Undefined


---

## **Bonus Challenges**

1. **Weapons with Power Greater Than 75**  
   List all weapons with power greater than 75 and the Imperial teams to which they are assigned.

2. **Summary of Planned Attacks**  
   Get a summary of all planned attacks, including the probability of success and the Imperial and Rebel teams involved.

3. **Rebel Teams and Attack Probabilities**  
   List all Rebel teams and the probabilities of success of the attacks targeting their bases.

4. **Successful Planned Attacks**  
   List all planned attacks with a success probability greater than 70%, including target base information and the assigned Imperial team.

5. **Rebel Teams with More Soldiers Than the Average**  
   - **Step 1**: Create a view to calculate the average number of soldiers in Rebel teams.
   - **Step 2**: Use the view to identify teams that exceed the average.

6. **Experiment with Indexes**  
   - Create and test different types of indexes (single-column and composite) on various tables.
   - Evaluate their impact on query performance.
   - Write an analysis explaining why the indexes improved (or didn’t improve) the performance, considering:
     - Query structure.
     - Table size.
     - Column cardinality.

## Submission

Upon completion, run the following commands:

```
$ git add .
$ git commit -m "done"
$ git push origin main
```

Then create a Pull Request!!

![happy_coding](https://user-images.githubusercontent.com/970858/63899010-c23fc480-c9ea-11e9-84a2-542907e42362.png)

