# Lab-8-Geometry-Calculator


# Course information
- What is your course section?
- Your assignment title.

# Initial Plan
Your professor asks you to explain:
- What will your program do?
- What inputs will the user enter?
- What variables will you use?
- What calculations will the program perform?
- What checks will you include?
- What output do you expect?


# Compile and Run Instructions
first, you will select one of the 4 options by tipping the number and clicking enter. 1= Calculate the Area of a Circle, 2= Calculate the Area of a Rectangle, 3= Calculate the Area of a Triangle, 4= Quit. depending on your prerrior answer the code will ask you for specific information option 1: radius, 2:


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
