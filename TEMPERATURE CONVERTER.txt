print("**********TEMPERATURE CONVERTER/ MEASUREMENT CONVERTER************\n" )
def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32

def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9

def inch_to_centimeters(inch):
    return inch * 2.54

def Centimeters_to_inch(centimeters):
    return centimeters / 2.54

def inch_to_meters(inch):
    return inch / 39.37
def Centimeters_to_meter(centimeters):
    return centimeters / 100


# Main program starts here
print("Welcome to the Temperature and Unit Conversion Program!")
print("Enter 1 to convert from Celsius to Fahrenheit")
print("Enter 2 to convert from Fahrenheit to Celsius")
print("Enter 3 to convert from Inch to Centimeters")
print("Enter 4 to convert from Centimeters to Inch")
print("Enter 5 to convert from Inches to Meters")
print("Enter 6 to convert from Centimeters to Meters")

choice = int(input("Enter your choice: "))

if choice == 1:
    celsius = float(input("Enter temperature in Celsius: "))
    print("Temperature in Fahrenheit is : ", celsius_to_fahrenheit(celsius))
elif choice == 2:
    fahrenheit = float(input("Enter temperature in Fahrenheit: "))
    print("Temperature in Celsius is : ", fahrenheit_to_celsius(fahrenheit))
elif choice == 3:
    inch = float(input("Enter the length in inches: "))
    print("length in centimeters is : ", inch_to_centimeters(inch))
elif choice == 4:
    centimeter = float(input("Enter the length in centimeter: "))
    print("length in inches is : ", Centimeters_to_inch(centimeter))
elif choice == 5:
    inch = float(input("Enter the length in Inches: "))
    print("length in meter is : ", inch_to_meters(inch))
elif choice == 6:
    centimeter = float(input("Enter the length in centimeter: "))
    print("length in meters is : ", Centimeters_to_meter(centimeter))
else:
    print("Invalid choice! Please enter a valid choice.")



