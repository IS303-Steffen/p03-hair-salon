### MAX SCORE: 100
### YOUR SCORE:  
## Grader's Notes:
- TAs: Put any notes on points lost here.
---
## Rubric

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th>#</th>
      <th>Requirement</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>p3_db_classes.py has Customer class with all necessary variables and is created according to peewee syntax.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>2</td>
      <td>p3_db_classes.py has Stylist class with all necessary variables and is created according to peewee syntax.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>3</td>
      <td>p3_db_classes.py has Appointment class with all necessary variables and is created according to peewee syntax.</td>
      <td>7</td>
    </tr>
    <tr>
      <td>4</td>
      <td>p3_db_classes.py has initialize_database() function that connects to the database, creates tables, and returns a SqliteDatabase object</td>
      <td>2</td>
    </tr>
    <tr>
      <td>5</td>
      <td>p3_data_import.py fills the 3 tables in the database with the data from the provided excel file</td>
      <td>13</td>
    </tr>
    <tr>
      <td>6</td>
      <td>p3_data_import.py gets rid of the dashes "-" in the phone numbers.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>7</td>
      <td>p3_check_in.py allows for inputs of phone numbers to contain dashes "-" or spaces " ".</td>
      <td>10</td>
    </tr>
    <tr>
      <td>8</td>
      <td>p3_check_in.py gets existing customer if there is a match for the phone number.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>9</td>
      <td>p3_check_in.py calls returning_customer_message() for returning customers and allows returning customers to reuse their previously selected options.</td>
      <td>10</td>
    </tr>
    <tr>
      <td>10</td>
      <td>p3_check_in.py creates new customer for phone numbers not already in the database</td>
      <td>8</td>
    </tr>
    <tr>
      <td>11</td>
      <td>p3_check_in.py Gathers hair cut and stylist selection for new customers, and existing customers that choose to make new selections.</td>
      <td>10</td>
    </tr>
    <tr>
      <td>12</td>
      <td>p3_check_in.py creates a new appointment in the database based on the data collected in the previous steps</td>
      <td>5</td>
    </tr>
    <tr>
      <td>13</td>
      <td>p3_manager_tools.py shows the 5 most recent appointments that had dissatisfied customers. Should call get_appointment_info() method</td>
      <td>10</td>
    </tr>
    <tr>
      <td>14</td>
      <td>p3_manager_tools.py allows for deleting stylists</td>
      <td>5</td>
    </tr>
    <tr>
      <td>15</td>
      <td>p3_manager_tools.py allows for exiting and handling invalid inputs.</td>
      <td>3</td>
    </tr>
    <tr>
      <td colspan="2">Total</td>
      <td>100</td>
    </tr>
  </tbody>
</table>

## TA Guide:

1. #### p3_db_classes.py has Customer class with all necessary variables and is created according to peewee syntax.
    - 5 points
        - -.5 for each missing variable, or if the variable is of a wrong Field type.

2. #### p3_db_classes.py has Stylist class with all necessary variables and is created according to peewee syntax.
    - 5 points
        - -.5 for each missing variable, or if the variable is of a wrong Field type.

3. #### p3_db_classes.py has Appointment class with all necessary variables and is created according to peewee syntax.
    - 7 points
        - -.5 for each missing variable, or if the variable is of a wrong Field type.

4. #### p3_db_classes.py has initialize_database() function that connects to the database, creates tables, and returns a SqliteDatabase object
    - 2 points
      - -1 if it doesn't return a SqliteDatabase object

5. #### p3_data_import.py fills the 3 tables in the database with the data from the provided excel file
    - 13 points
        - -10 if the data isn't separated out into 3 tables.
        - -5 if there are duplicates
        - -4 if there are problems with the IDs not aligning between the primary keys and foreign keys.

6. #### p3_data_import.py gets rid of the dashes "-" in the phone numbers.
    - 2 points

7. #### p3_check_in.py allows for inputs of phone numbers to contain dashes "-" or spaces " ".
    - 10 points
        - -3 if it only works for just one of "-" or " "

8. #### p3_check_in.py gets existing customer if there is a match for the phone number.
    - 5 points

9. #### p3_check_in.py calls returning_customer_message() for returning customers and allows returning customers to reuse their previously selected options.
    - 10 points
        - -3 if returning_customer_message() doesn't handle when there are 0 appointments.
        - -6 if the message about the number of appointments and the last appointment data doesn't work correctly.
        - -3 if you can't choose to use previous appointment info for the current appointment.

10. #### p3_check_in.py creates new customer for phone numbers not already in the database
    - 8 points
        
11. #### p3_check_in.py Gathers hair cut and stylist selection for new customers, and existing customers that choose to make new selections.
    - 10 points
        - -5 if choosing haircut doesn't work
        - -3 if choosing stylist of same gender doesn't work.

12. #### p3_check_in.py creates a new appointment in the database based on the data collected in the previous steps
    - 5 points

13. #### p3_manager_tools.py shows the 5 most recent appointments that had dissatisfied customers. Should call get_appointment_info() method
    - 10 points
        - -5 if it some logic error in getting the 5 most recent appointments
        - -2 if some error in the message beign printed.

14. #### p3_manager_tools.py allows for deleting stylists
    - 5 points

15. #### p3_manager_tools.py allows for exiting and handling invalid inputs.
    - 3 points
        - -1 if if doesn't handle invalid inputs.
