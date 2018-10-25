This is the first project that I have ever done using git. The project is called Gamegogy and it takes in students’ data and course data 
and combines them into a gui that allows the student to see where they are in their classes. It also allows them to see where they are in 
comparison to other students and ranks them as so. So if the student does well throughout the class they move up the leaderboard.
If they do bad, they move down the leaderboard.

The first class listed is a class called Bar.  Bar creates the GUI that shows the students on the right-hand side of the screen.  
The bar's color is green is set to green and it has a width and height of 20. 
Bar accesses the student id and assigns it to the ID that bar will be using throughout the process.
It adds a component listen that responds to when the user clicks on one of its components. 
It then calculates the text field it will need by taking the students points and dividing it by the points possible. 
Then it multiplies that by using the java command getWidth() and multiplying that by .8.

Once it calculates all of that it then moves to color in the e text my using a paint component. Once it does that it uses a couple of mouseClicked() events and mousePressed() events to change the data that is on the screen.
The next class is titled as BarGraph. 
BarGraph takes the bars made above and makes them into a leaderboard like system with bars above and below each other.  
The next class listed is the courseGrades . The courseGrades class takes in the data provided by the later mentioned DataReader Class and assigns them to its own class type. Making them easier to access later.
The next class is Course Grades. 
Course grade uses CSVreader to parse through a csv that contains that Student Ids and grades that the program 
will use in ranking and organizing the students. 
The next part of course grades allows the student to select one of their courses and select one of the assignments.


The next class is the DataReader class. This class is the backbone of the whole program. It is the one that does all the data computations. 
In the beginning, it creates 5 array lists. One of type Student, One of Type Course, Two of Type String, and One of type float. 
It then tries to read the respective files brought in by coursegrades and parses them as well. It has two csv readers within the program that activates when either the file type is student or course.  It then sets the id for the courses or the students. 
The bottom half of data reader computes which course is being chosen or student is being chosen as well as their respective ID.

The next class is the GUIPanels class. This class makes the GUI panel that the student first sees when they launch the program. It lays it out in a rectangle and forces full screen, but it still allows the user to make the window smaller if need be. 
The next class is Leaderboard. Leaderboard runs the back bone of the system and allows input from the command line as well as the gui
LeaderboardGUI is the back bone of the gui sytem and is what sets the frame sizes, which are 500,500 and allows the gui to be scrollable
