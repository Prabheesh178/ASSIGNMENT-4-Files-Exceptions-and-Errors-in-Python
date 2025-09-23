# ASSIGNMENT-4-Files-Exceptions-and-Errors-in-Python
try:
    with open('sample.txt','r') as file1:
        reading_file=file1.read()
    print(reading_file)
except FileNotFoundError:
    print("Error: The file 'sample.txt' does not exist.")




#Task 2: Write and Append Data to a File

user_input= input ('enter some data to write in the file : ')
with open ("output.txt",'w') as file2:
    writing_file=file2.write(user_input+'\n')
    print('the number of character writen=',writing_file)

append_data=input ("enter some additional data to add int the file: ")
with open ('output.txt','a') as file2:
    appending_file=file2.write(append_data+'\n')

    print('the number of character writen=',appending_file)
