# Programming-II-Assignment-III

February 19, 2015                                             Assignment-3                           Due: March 3, 2015
                                                                          COP 3337
[All definitions in this assignment are created by me just for you all to practice various features of Java programming. Many of them have absolutely no bearing on reality.]
There are many different types of Creatures, and talking about the intelligence level of a Creature makes perfect sense. HumanBeing is a Creature, each possessing, in addition to the intelligence level, a name and age. Male is a HumanBeing, and so is Female. Animal is another Creature which possesses some Intelligence Level, and so is Bird.
In this assignment, you are required to implement a Creature as an abstract class containing an abstract method getIntLevel; a HumanBeing class described as above; a Male class and a Female class. For each male, we wish to keep track of his height and weight, whereas for every female, we wish to keep track of her last degree. Male and Female classes have all required accessor methods to return the values of their attributes. Both, Male and Female classes allow users to calculate intelligence level defined (absurdly) as follows:
Male: (Calculation proceeds in the order given here)
If age > 40, then IntLevel = 5
If age is < 5 years, then IntLevel = 1
If weight >= 150 pounds and height is > 70 inches then IntLevel = 5
If weight is between 120 and 149 pounds, and height > 70 inches, then IntLevel = 4
If weight is between 50 and 119 pounds, then IntLevel = 3
If weight is between 120 and 149 pounds, and height is between 55 and 69 inches,
            then IntLevel = 2
In all other cases, the IntLevel = 3.
Female:
If lastDegree = "Ph.D.", then IntLevel = 5
If lastDegree = "MS", then IntLevel = 4
If last Degree = "BS", then IntLevel = 3
If last Degree = "AA", then IntLevel = 2
In all other cases, IntLevel = 1.
When a Male or Female object is created, the constructor checks if this is indeed a "valid" person. A "valid" male is someone whose weight is less than 400 pounds and height is less than 100 inches. A "valid" female is someone whose age is less than 110 years. If the user tries to create an "invalid" person, the class constructors throw an exception called notHumanBeingException to the calling program. The calling program rejects that person from consideration. In case the person was "valid", the constructor calculates the person's Intlevel and initializes it. Obviously, HumanBeing must provide a method that allows setting of one's IntLevel.
The test program will do the following:
From an input file (as always, get the name of the file from the user using JOptionPane), read the basic information about Human Beings. The first character identifies what type of Human Being this person is - M or F. Information in the input file is in the following order:
Male: name, age, height (in inches), weight (in pounds).
Female: name, age, last degree.
Create an ArrayList of all persons, an array of males, and an array of females from this given data. That is, each person will be included in an ArrayList and one array.
Output unsorted ArrayList of persons.
Sort the ArrayList based on names, using "sort" method of the Collections interface.
Output the sorted ArrayList of persons.
Output unsorted list of Males.
Sort the array of males based on their heights using Arrays.sort (array_of_males, comparator) call.
Output the sorted array of males.
Output the unsorted list of females.
Sort this array based on age using Arrays.sort (array_of_females) call. Note that no comparator is passed in this call. Do whatever you need to do to achieve this.
Output the sorted list of females.
As in the past, the output should be sent to an output file, and should be completely self-explanatory.
Submit as always:
·The soft copy of your NetBeans project on SCIS Moodle along with the input and output files.
·The hard copy of all your java code along with the I/O files at the beginning of the class on the due date.
·All methods in the source code should be well-documented specifying at the least, everything that the user of any method needs to know. Additionally, if there are some salient features of any class that the user needs to know, do document them, too.
Good Luck!
