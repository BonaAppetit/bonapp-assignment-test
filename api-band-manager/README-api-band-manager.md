# API Band Manager

# Instruction

- Please complete the problem below within 2 days of the assignment being sent.
- You may use the coding language you are most comfortable with. (if you use nodejs it will be a plus  point)
- Your fundamentals are more important to us than proficiency in our tech stack.
- Adding Unit test with various test case
- Please upload to your GitHub, and ensure the repository can be accessed public
- Don't forget to create `readme`. How to run the code and command to run the test
- It will be Plus point if you provide the documentation about the Structure database or flow API.

# **ASSIGNMENT**

John is a band manager, John has a responsibility to manage more than one band. Help Jhon to Create a simple API to manage personnel in each band.

### Requirement:

- Able to create a band with attributes: name and maximal size (personnel in the band)
- Able to create a player
- Able to see list of the band
- Able to see the detail of the band include the list of personnel band
- Able to update a band
- Able to add members into the band

### Acceptance Criteria

- Validate maximum members in a band when you add the members, this refers to maximal size when you created a band.
- One Personnel or member, only have 1 band

# Sample Inputs

- Create a band :

    ```
    **Post {host}/band**
    payload:
    - name
    - max personnel / member
    ```

- Add Members / Personnel into a band

    ```
    **Post {host}band/personnel**
    payload:
    - band_id
    - personnel_id
    ```


# Expected Outputs

- List of the band

    ```
    **Get {host}/band**
    response:
    - band_id
    - name
    - max personnel / member
    ```

- Detail of the band include list of Personnel

    ```
    **Get {host}/band/:band_id**
    response:
    - name
    - members:
    	- name
    	- position
    ```
