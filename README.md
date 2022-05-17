# User Management Screen UI Specification

# 1. Requirements
## 1.1. Functional Requirements
## 1.1.1. General Requirements
Overall UI requirements for the user management screen are listed below.
### Details:
1. It is expected for the below components to be developed.
* Header Component
* Users Data Grid Component
* New User Component
### Screen Prototype:
![Screen Shot 2022-05-16 at 12 32 1](https://user-images.githubusercontent.com/51910678/168849901-52024965-82d1-4b5c-949e-a70d4fb09c87.png)

## 1.1.2. Header Component
Designing the header component and making checks.
### Details:
1. A left aligned "New User" button should be placed on the component.
2. On the right side of the new user button, a left aligned "Hide Disabled User" checkbox should be placed.

    1. If there are disabled users, checking the checkbox should update the Users Data Grid Component. In this case, disabled users should not be visible in the list.
3. A right aligned "Save User" button should be placed on the component. The button should look "disabled" (as in the component prototype) by default and the button should be clickable when every field in the New User Component is filled correctly.
### Component Prototype:
![Screen Shot 2022-05-16 at 12 32 1 (1)](https://user-images.githubusercontent.com/51910678/168853648-64465199-5819-4f21-9d66-d971d685bb12.png)
## 1.1.2. Users Data Grid Component
Designing the user list component and making checks.
### Details:
1. User list component is comprised of four columns, each with its own header.
2. A right aligned filter button is placed in each of the column headers.
3. The first column on the left is the "ID" column. 

    1. ID values should be in ascending order by default. When the filter button is clicked, the values should be listed in descending order.
4. The second column on the left is the "User Name" column. 
    
    1. User name values should be alphabetically sorted in ascending order by default. When the filter button is clicked, the values should be listed in descending order.
5. The third column on the left is the "Email" column.

    1. Email values should be alphabetically sorted in ascending order by default. When the filter button is clicked, the values should be listed in descending order.
6. The fourth column is the "Enabled" column. 

    1. The column consists of values of "true" or "false."
    2. True values should be displayed on top by default. When the filter button is clicked, the ordering should change.
    3. When Hide Disabled User checkbox in the header of the page is checked, users with an enabled value of false should not be displayed.

