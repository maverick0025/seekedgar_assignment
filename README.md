# seekedgar_assignment

## Question 1

## Question 2

- Create Database table
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
