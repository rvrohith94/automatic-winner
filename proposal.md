# X-Team 117 Project Proposal - Monthly Budget Tracker

## Goal

Work as a team to implement the proposed project - *Monthly Budget Tracker*.

## Problem Description

- Keeping track of one's monthly expenses is one of the most important ways to be financially responsible in life. So we would like to make the task a bit more easier with a simple yet intuitive application called *Monthly Budget Tracker*.

- This application allows users to enter their preferred budget amount at the start of every month and then add the money spent on a day-to-day basis throughout the month (The total amount spent by the user so far will also be displayed - Refer figure1.png). At any point if the total amount spent during the course of the month exceeds the bugdet amount, an alert message would be displayed to warn the user about the same.

## Q & A

1. Name: **Monthly Budget Tracker**



2. Output: Output produced will be the amount spent by the user so far during the month (Will be a Double value - in Java terms).



3. Input: Input entered by the user will be the budget amount to be set at the start of month and the daily expenses incurred (All these    values will be of Double data type). Example value : 250.83 (in USD).



4. User Interface: The user interface for this application will be a simple graphic user interface (GUI) consisting of a calendar along    with text boxes which support entry of numeric data. The dates in the calendar have an add button (+), upon clicking on which a new      panel containing data entry fields would pop up. There is an alert widget in the top right corner, that displays an alert message if    the amount spent by the user exceeds the set budget amount.

   Please refer the attached file - **figure1.png**
   

5. Types List: The following are the proposed java classes to implement the back-end implementation of this application -

   - MonthlyBudgetTracker.java - Main driver class of this application that contains the  code to retrieve and write the values                                          displayed in the GUI to a file. Also contains the necessary logic to display the alert message
                                 when the total amount spent crosses the set budget.
   
   - BudgetTrackerHashTableADT.java - An ADT java interface containing standard methods like 
     * put(K key, V value)
     * get(K key)
     * remove(K key)
     * size()
     
   - BudgetTrackerHashTable.java - A class that implements the BudgetTrackerHashTableADT interface and has the implementation of APIs 
                                   to get the size of the hash table, to insert a new key-value pair into the hash table, to get the                                        value corresponding to a given key from the hash table, to remove a given key from the hash table.
     
     Note: The key-value pair for the BudgetTrackerHashTable in this application would be <Date, Double>
    
   - TestBudgetTrackerHashTable.java - Unit tests for the BudgetTrackerHashTable.java class.
   
   - MonthlyBudgetTrackerTests.java - Unit Tests that will test the APIs related to adding of the budget, amount spent values of the                                           Monthly Budget Tracker application.
   
   *NOTE: We didn't discuss how to implement the proposed GUI for this application, hence couldn't add the proposed files for the                 related front-end codebase.*
   
