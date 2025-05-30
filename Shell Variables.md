# Printing Variables
*echo* = printing. <br>
Adding a *$* symbol will indicate to print the variable and not the text.<br>
eg: echo hi = hi <br>
eg: echo $hi = value stored in variable hi.
<br> ***Commands***
```
echo $FLAG
```
***Output***<br>
![{2EC71ADD-EB11-4080-8259-63B52906CB9A}](https://github.com/user-attachments/assets/c247aac7-70ce-4b8c-a310-35393f2e8e88)

# Setting Variables
Basically assigning --> variable=value (No space given between value and variable)
<br>***Commands***
```
PWN=COLLEGE
```
***Output***<br>
![{29E74EF4-4235-40BE-BA71-DEB39AF5DE1A}](https://github.com/user-attachments/assets/102cc9f7-f9b8-4c67-bb44-8e6f2284b42e)

# Multi-word Variable
We need to add quotes when assigning a variable to a multi word value. <br>
eg: Variable="2 words"
<br>***Commands***
```
PWN="COLLEGE YEAH"
```
***Output***<br>
![{974EF787-6EDC-4EC1-B456-FD43A2837807}](https://github.com/user-attachments/assets/9576d2a0-f6cc-4a24-baaf-4b4f516b3dab)

# Exporting Variables
*sh* --> opens a child shell within the main shell.
To use the variables from main shell to the child shell we use export process. <br>
syntax --> export variable=value<br>
***Commands***
```
COLLEGE=PWN
export PWN=COLLEGE
/challenge/run
```
***Output***<br>
![{88747431-1C87-4782-BC1E-056C4C53F663}](https://github.com/user-attachments/assets/c9738341-9e35-4e4e-bf26-6a41f5b77373)

# Printing Exported Values
Just like *echo* the ***env*** command prints out every exported variable in the shell
<br>***Commands***
```
env
```
***Output***<br>
![{33809CC6-E7A8-448F-A2E9-6AA8DCA6E3E2}](https://github.com/user-attachments/assets/cd300aae-186c-43ae-ab9a-532ca12213b1)

# Storing Command Output
Command substitution is used to store an output in a variable. <br>
syntax--> variable=$(command) 
<br>***Commands***
```
PWN=$(/challenge/run)
echo $PWN
```
***Output***<br>
![{9C9FCFCE-A538-4A0A-9716-9F9E54A3C9DD}](https://github.com/user-attachments/assets/3b822ebe-cb28-431d-b245-3383890d3f11)

# Reading Input
*read* argument reads the input given by the user. <br>
"-p" is like a semi print statement which we use during printing the input values. <br>
syntax --> read -p "INPUT:" variable <br>
***Commands***
```
read PWN
COLLEGE
```
***Output***<br>
![{2FDEA4DB-FA46-4392-BBE2-82EDE7922BC2}](https://github.com/user-attachments/assets/e11d0ef9-9588-4a79-8c20-3a57f5df87fe)

# Reading Files
*Important*<br>
read variable < file
<br> ***Commands***
```
read PWN < /challenge/read_me
```
***Output***<br>
![{84C6BA98-C2BD-48A1-B8D3-4D398149A3B8}](https://github.com/user-attachments/assets/19b5cf0a-00cd-4a47-8fb6-4424c4837120)



