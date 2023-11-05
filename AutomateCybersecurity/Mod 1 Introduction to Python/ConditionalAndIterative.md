# Conditional and Iterative Statements

## If statements

Conditional statements evauluate code to see if it meets a specified set of conditions. These start with an 'if.'

For the body of an if statement to be executed, it must be indented further than the header. 

```py
if failed_attempts > 5:
    print("Account Locked")
```

### Operators

Determine the conditions being met

 - ">"
 - "<"
 - "<="
 - ">="
 - "=="
 - "!="

```py
if operating_system == "OS 2"
    print("Updates Needed")
```

This executes the code inside the if statement if the OS version matches OS 2.

## Else Statements

Else statements precede a code section that only evaluates when all conditions that precede it in a conditional statement evaluate to False.

```py
# Else statements
operating_system = "OS 3"
if operating_system == "OS 2"
    print("Updates Needed")
else:
    print("No updates needed")
```
## Elif statements

elif statements precede a condition that is evaluated when previous conditions evaluate to false. There can be multiple elif statements following an if statement. When python reaches an elif statement that evaluates to true, it only executes the code for that elif statement and all others after are ignored.

```py
if status == 200:

    print("OK")

elif status == 400:

    print("Bad Request")

elif status == 500:

    print("Internal Server Error")

else:

    print("check other status")
```

## Logical operators for multiple conditions

Can be used if more than one condition needs to be evaluated. 

### and

and requires both conditions on either side of it to evaluate to True.

```py
if status >= 200 and status <= 226:

    print("successful response")
```
### or

Or requires only one of the conditions on either side of the statement to evaluate to True.

```py
if status == 100 or status == 102:

    print("informational response")
```
### not

The not operator negates a given condition so that it evaluates to False if the condition is True and to True if it is False.

```py
if not(status >= 200 and status <= 226):

    print("check status")
```

# Iterative statements (Loops)

Code that repeatedly executes a series of instructions.

## For Loops

Repeat code for a specified sequence.

```py
for i in [1,2,3,4]:
    print(i)
```
### Range function

generates a sequence of numbers
Start at the first number and stops at the stop point. Stop point is not included.

```py
range(0,10)
```

0,1,2,3,4,5,6,7,8,9

## While loops

repeatedly execute based on a condition. While the condition is true, the loop executes. The loop stops when the condition becomes false.

```py
time = 0
while time <= 10:
    print(time)
    time = time +2

    
```

The loop variable (time) must be declared outside of the conditional header. The loop variable must be changed inside of the loop body.

### Practical example

Limit the amount of devices that can be connected at one time. 

```py
# create a while loop

max_devices = 5
i = i

while i < max_devices:
    print("User can still connect to additional devices")
    i = i + 1
print("User has reached the maximum number of devices")
```

## More on loops in Python

### Looping through a list

```py
computer_assets = ["laptop1", "laptop2", "desktop3"]
for asset in computer_assets:
    print(asset)
```
This will print all the assets in the list.

### Looping through a string

```py
string = "security"
for character in string:
    print(character)
```

This will print each letter of the string on a separate line.

### Using range

A range accepts input for starting point, ending point and increment in parenthesis.

range(0,5,1)

Must always define stop point, but start point can default to 0 and increment defaults to 1. 

```py
for i in range(5):
    print(i)
```
This will print 0 - 4.

### While loops

Using booleans to evaluate while loops

```py
count = 0
login_status = True
while login_status == True:
    print("Try again.")
    count = count + 1
    if count == 4:
        login_status = False
```

## Managing loops

'break' and 'continue' can be used to control loops. Break is used to exit a loop, and continue is used to skip an iteration and continue with the next one. 

### break

If you want to exit a for or while loop based on a condition. Use break. This will exit the loop even if original loop header condition is not met. 

```py
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    if asset == "desktop20":
        break
    print(asset)
```

In this instance, the loop exits on the second iteration due to the break condition being met. 

### continue

To skip an iteration based on an if condition being true, use continue. 

```py
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    if asset == "desktop20":
        continue
    print(asset)
```
In this instance, the loop will run all the way through, but desktop20 will not be printed due to the continue condition being met.

## Infinite loops

Infinite loops never meet an exit condition. They will continue to run until you manually break the loop, using CTRL + C or CTRL + Z. 

