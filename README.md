<h1> Invenetory managment system</h1>
This is a simple inventory managment system built using C++.
Following are the details of the project.

<h2>User Defined Data Types</h2>
<b>Struct</b> Faculty conatins the data of faculty members. ID, name, Designation.
<b>Struct</b> IneventoyItems conatins the data of each Inventory Item. ID, name, Designation.
<b>Vector</b> Vector I using a STL vectors to read our data from file into it and writing our data on to it.

<h2>File Reading and Writing</h2>
File Reading and Writing is done in binary mode using two function. Both of the fucntions handles error while openeing file.
When the program starts the ReadFromFile() reads the data from the file and stores in the vector.
When user exits the program it stores the data in the vector to the file by WriteToFile().

<ol>
  <li>
    <h3>ReadFromFile()</h3>
      This function opens the file in input mode and binary mode using Fstream class object.
  </li>
  <li>
    <h3>WriteToFile()</h3>
      This function opens the file in output mode and binary mode using Fstream class object.
  </li>
      
 </ol>
 
 <h2>AddItem()</h2>
  Add item Function allows the user to add an item into the records.
  If at any stage user presses -1 it go backs to main menu
  It uses two helper functions.
  <ol>
  <li>
    <h3>goBack(int), goBack(String)</h3>
  </li>
  <li>
    <h3>WriteToFile()</h3>
  </li>
      
 </ol>
 
  <h2>RetrieveItem()</h2>
This function retrieves an item that has been allocated to a facutly member.
This uses following helper function
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
  <li>
    <h3>goBack(int), goBack(String)</h3>
  </li>
 </ol>
 
 <h2>ViewAll()</h2>
 This fucntion displays all the items available in the inventory along with their details.
 
 
 <h2>SearchItem()</h2>
 This function is used to search for a particular item in the inventory by name or ID.
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
 </ol>
 
 <h2>EidtItem()</h2>
This fucntion searches for a particular item and displays the user to enter the new data for the item. If the user wants to leave the field of the data as it is then enter -1. This uses following helper functions.
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
  <li>
    <h3>goBack(int), goBack(String)</h3>
  </li>
 </ol>
 
  <h2>DeleteItem()</h2>
This fucntion searches for a particular item and deletes it from inevnetory i.e the vector.
This uses following helper functions.
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
 </ol>
 
  <h2>AssignItem()</h2>
This fucntion searches for a particular item and displays the user to enter the new data for the faulty Member to assign the item. 
This uses following helper function.
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
  <li>
    <h3>goBack(int), goBack(String)</h3>
  </li>
 </ol>
 
  <h2>EidtItem()</h2>
This fucntion searches for a particular item and displays the user the lsit of Faculty members that the item has been allocated to.
This uses following helper functions.
  <ol>
  <li>
    <h3>searchMenu()</h3>
  </li>
 </ol>
 
 <h1>Helper Functions</h1>
 Following are the list of the fucntion used in our project other than the main function.
 
  <ol>
  <li>
    <h3>searchMenu()</h3>
    This Function is used to display the user option to search by ID or name or go back to main menu. It returns the index position of the item if item is found or -1 in case if it is not found and the also -1 when user wants to go back to main menu.
  </li>
  <li>
    <h3>goBack(int), goBack(String)</h3>
    This function takes int or string as input and returns true if user enters -1 else false. Used to see if user has entered -1 to go back or in edit item to leave the field as it is.
  </li>
  <li>
    <h3>setClr()</h3>
    This function sets the color of the console sreen text and background.It uses setConsoleTextAttributes funcion taken from the Windows.h library to set the colors. The colors are already defined as MACROS in our project.
  </li>
  
  <li>
    <h3>menu()</h3>
    This function displays the main menu to the user and takes the valid input and returns an int based on user's choice.
  </li>
  
  <li>
    <h3>compare(char [], char [])</h3>
   This is a custom defined function to comapare to char arrays irrespective of their case.
  </li>
  
  <li>
    <h3>printItem(int)</h3>
    This function takes an int input which is the index of item in inventory and prints the item details. Name, ID, Count, Allocated_to.
  </li>
  <li>
    <h3>goBack(int), goBack(String)</h3>
    This function takes int or string as input and returns true if user enters -1 else false. Used to see if user has entered -1 to go back or in edit item to leave the field as it is.
  </li>

 
 </ol>
 
