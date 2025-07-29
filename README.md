# assignment4.py
try:
    
    with open("sample.txt", "r") as file:
        print("Contents of sample.txt:\n")
        
        
        for line in file:
            print(line.strip())  
except FileNotFoundError:
   






 first_input = input("Enter some text to write to the file: ")

with open("output.txt", "w") as file:
    file.write(first_input + "\n")

second_input = input("Enter more text to append to the file: ")

with open("output.txt", "a") as file:
    file.write(second_input + "\n")

print("\nFinal content of 'output.txt':")
with open("output.txt", "r") as file:
    for line in file:
        print(line.strip())

