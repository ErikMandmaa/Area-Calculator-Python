import math # imports the math module for mathematical functions

def calculate_area(shape, dimensions): # the function to calculate area based on shape and dimensions
    if shape == "triangle": # checks if the shape is a triangle
        base = dimensions.get("base", 0) # retrieves the base from dimensions
        height = dimensions.get("height", 0) # retrieves the height from dimensions
        area = 0.5 * base * height # calculates the area of the triangle using the formula 0.5 * base * height
    elif shape == "rectangle": # checks if the shape is a rectangle
        length = dimensions.get("length", 0) # retrieves the length from dimensions
        width = dimensions.get("width", 0) # retrieves the width from dimensions
        area = length * width # calculates the area of the rectangle using the formula length * width
    elif shape == "square": # checks if the shape is a square
        side = dimensions.get("side", 0) # retrieves the side from dimensions
        area = side ** 2 # calculates the area of the square using the formula side^2
    elif shape == "circle": # checks if the shape is a circle
        radius = dimensions.get("radius", 0) # retrieves the radius from dimensions
        area = math.pi * radius ** 2 # calculates the area of the circle using the formula pi * radius^2
    else: # otherwise
        raise ValueError("Unsupported shape") # raises an error for unsupported shapes
    
    return area # returns the calulated area

def main(): # main function to run the area calculator
    print("=" * 18) # prints a separator line with 18 equal signs
    print("Area Calculator 📐") # prints out area calculator with the triangle ruler emoji
    print("=" * 18) # prints another separator line with 18 equal signs
    
    while True: # starts an infinite loop of calculations
        print("1) Triangle") # prints option for triangle
        print("2) Rectangle") # prints option for rectangle
        print("3) Square") # prints option for square
        print("4) Circle") # prints option for circle
        print("5) Quit") # prints option to quit the program
        
        choice = input("Which shape: ").strip() # prompts the user to choose a shape and removes any trailing whitespace
        
        if choice == "5": # checks if the user chose to quit
            break # exits the loop and ends the program
        
        dimensions = {} # initializes an empty dictionary to hold dimensions
        
        if choice == "1": # checks if the user chose triangle
            shape = "triangle" # sets shape to triangle
            base = float(input("Base: ")) # prompts the user to input the base and converts it to a float
            height = float(input("Height: ")) # prompts the user to input the height and converts it to a float
            dimensions = {"base": base, "height": height} # stores the base and height in the dimensions dictionary
        elif choice == "2": # checks if the user chose rectangle
            shape = "rectangle" # sets shape to rectangle
            length = float(input("Length: ")) # prompts the user to input the length and converts it to a float
            width = float(input("Width: ")) # prompts the user to input the width and converts it to a float
            dimensions = {"length": length, "width": width} # stores the length and width in the dimensions dictionary
        elif choice == "3": # checks if the user chose square
            shape = "square" # sets shape to square
            side = float(input("Side: ")) # prompts the user to input the side and converts it to a float
            dimensions = {"side": side} # stores the side in the dimensions dictionary
        elif choice == "4": # checks if the user chose circle
            shape = "circle" # sets shape to circle
            radius = float(input("Radius: ")) # prompts the user to input the radius and converts it to a float
            dimensions = {"radius": radius} # stores the radius in the dimensions dictionary
        else: # otherwise
            print("Invalid choice. Please try again.") # informs the user of an invalid choice
            continue # restarts the loop
        
        area = calculate_area(shape, dimensions) # calls the calculate_area function to compute the area
        print(f"The area is {area}") # prints out the calculated area
        print() # prints a blank line for better readability

if __name__ == "__main__": # checks if the script is being run directly
    main() # calls the main function to start the program