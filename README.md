# seekedgar_assignment

## Question 1

[Click here to find the code](https://colab.research.google.com/drive/1ANEtfOEN_wPA7-YGCb5U1Y3Oy5-lZ26t?usp=sharing)

- Regarding the code for the 2nd SEC 10K Report, as expected the start line “ITEM 7.
MANAGEMENT'S DISCUSSION AND ANALYSIS OF FINANCIAL CONDITION AND RESULTS OF
OPERATIONS” because, in the 2nd report the start line actually is "Item 7. Management's Discussion and Analysis of Financial" so, it's quite not possible, one approach through which this can be tackled is by taking the longest substring that matches with the expected start line.

## Question 2

- Create a Database table
    ```
    CREATE TABLE employees (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    NAME VARCHAR(255) NOT NULL,
    CURRENT_POSITION VARCHAR(255) NOT NULL,
    AGE INT NOT NULL,
    EXPIRATION_OF_TERM INT NOT NULL,
    CONSTRAINT unique_name_position UNIQUE (NAME, CURRENT_POSITION)
    );
    ```
- Insert one line to the table
  ```
  INSERT INTO employees (NAME, CURRENT_POSITION, AGE, EXPIRATION_OF_TERM) VALUES 
  ('Johnny', 'Manager', 45, 1998);

  ```
- Update the line to change the AGE value
  ```
  UPDATE employees SET AGE = 46 WHERE NAME = 'Johnny' AND CURRENT_POSITION = 'Manager';
  ```
- Delete a line from the table
  ```
  DELETE FROM employees WHERE NAME = 'Johnny' AND CURRENT_POSITION = 'Manager';
  ```
