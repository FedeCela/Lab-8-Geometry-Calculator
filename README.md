# Lab-8-Geometry-Calculator

# Initial Plan
# What will your program do?
My program will display a menu that allows the user to calculate the area of three different shapes: a circle, a rectangle, and a triangle. It will also give the user the option to quit the program.

# What inputs will the user enter?
The user will enter a number from 1 to 4 to select an option from the menu. Depending on the selection, the user will enter the radius of a circle, the length and width of a rectangle, or the base and height of a triangle.

# What variables will you use?
I will use an integer variable called choice to store the menu selection. I will use double variables called radius, length, width, base, height, and area to store the measurements and calculation results. I will also use a constant called PI with the value 3.14159.

# What calculations will the program perform?
The program will calculate the area of a circle by multiplying PI by the radius twice. For a rectangle, it will multiply the length by the width. For a triangle, it will multiply the base by the height and then by 0.5.

# What checks will you include?
The program will check if the user enters a valid menu choice between 1 and 4. It will also check that the measurements are not negative before calculating the area. Zero will be accepted as a valid measurement.

# What output do you expect?
I expect the program to display the area of the selected shape with a clear label. If the user enters a negative measurement or an invalid menu choice, the program will display an error message. If the user selects option 4, the program will display a goodbye message and end.

# Compile and Run Instructions
first, you will select one of the 4 options by tipping the number and clicking enter. 1= Calculate the Area of a Circle, 2= Calculate the Area of a Rectangle, 3= Calculate the Area of a Triangle, 4= Quit. depending on your answer the code will ask you for specific information option 1: radius, option 2: length and width, option 3: base and height, option 4: program ends.


# How does your selection logic send each choice to the right calculation?
 The program uses if and else if statements to check the user's choice. Each number has a different calculation, and the program performs the calculation that matches the selected number.
 
 # Why is radius * radius correct while radius ^ 2 is not?
 In C++, the multiplication operator (*) is used to multiply numbers. The ^ symbol is not used for exponents, so radius * radius is the correct way to square the radius.
 
# Why does the triangle calculation use 0.5 rather than integer division 1 / 2?
 The number 0.5 represents one half. If we use 1 / 2 with integers, C++ gives us 0 instead of 0.5, which would make the triangle area incorrect.
 
# Where do you check negative dimensions, and how do you handle zero and choice 4? 
The program checks if the dimensions are negative before calculating the area. If a measurement is negative, it displays an error. Zero is allowed and produces an area of zero. Choice 4 ends the program without asking for measurements.

# Test Results

Test	                         Input	                                         Expected result
Circle                      	Radius 2                                            	12.56636
Rectangle	                Length 3, width 4.5	                                        13.5
Triangle                  	Base 5, height 3                                         	7.5
Quit                        	Choice 4	                                            Program ends
Invalid choice              	Choice 0                                             	Error message
Invalid choice	             	Choice 5	                                            Error message
Negative radius                  	-1	                                              Error message
Negative length	                 	-1	                                              Error message
Negative width	                 	-1		                                            Error message
Negative base                  		-1	                                            	Error message
Negative height	                 	-1		                                            Error message
Zero                   	         radius	0		                                        Area 0
