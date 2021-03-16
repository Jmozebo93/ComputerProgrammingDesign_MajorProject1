# ComputerProgrammingDesign_MajorProject1
This program will require you to create a program that will allow faculty members to post their course and office hour schedules.
Enumeration

First of all, this project utilizes enumerated types which help your program’s readability. Here is an
example:


The code above would appear in a separate file named DaysOfWeek.java and would serve as the data type for variables that could only have the values: `SUNDAY`, `MONDAY`, `TUESDAY`, `WEDNESDAY`,
`THURSDAY`, `FRIDAY`, `SATURDAY`. Notice, these are not Strings! Internally, `SUNDAY=0`, `MONDAY=1`,
`TUESDAY=2`, `WEDNESDAY=3`, `THURSDAY=4`, `FRIDAY=5`, `SATURDAY=6`. However, the enumerated type is more elegant way of representing these values. The following examples should also prove helpful to you:


You can also retrieve the String value of an enumeration. The following example would give the String
`value` the value `"SUNDAY"`:

UML Class Diagrams

Here are the UML Class Diagrams for the classes you must implement in Java. You are free to add additional private methods if needed.
 
 

The method `getFormatedTimeBlock()` should return a string in the following format:





The method getCalendar() should return all course items, office hour items and appointment items. Each item (i.e. formatted TimeBlock) should be listed under a heading with the day of the week. Within a particular day, the items should be listed in sorted order by time (Hint: Sorting is not necessary -- use a loop that goes from 5 to 2400 by 5's.).
 

 

The toString() method

The toString method should return a String formatted as in the input file. Notice that TimeBlock.toString() will not include the location or comment properties. Most classes will have each property on a new line, TimeBlock properties will be separated by a comma.
Handling ArrayLists

Each ArrayList should have five associated methods to perform: getNum, add, get, set and remove. So if you have an ArrayList named widgets that stored items of type Widget, then the associated UML would be:


Input File

The input file will be read by the user using any file reader and input streams (BufferedReader or Scanner) to your main() method using command-line arguments. The format for the input file is shown below:
 
 
You should also reference the input file provided in this repository.
Notes

-	When outputting office hour information, use the string “Office Hours” as a description.
-	All start and end times will be a multiple of 5.
Output File

The format of the output file is the same as the input file. If you have created the toString() method for the Department class correctly, the produced String should match the input/output format. This should make this method trivial to write.
