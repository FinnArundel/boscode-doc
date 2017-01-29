## Table of content

*1 Pseudocode*  

[Pseudocode guidelines](#pseudocode-guidelines)     
[Sequence](#sequence)     
[Binary selection](#binary-selection)    
[Casewhere](#casewhere)          
[Pre-test repetition: while](#pre-test-repetition-while)         
[Post-test repetition: repeat](#post-test-repetition-repeat)         
[FOR/NEXT or counted loop](#for/next-or-counted-loop)         
[Subprogram](#subprogram)         
[Load array](#load-array)         
[Print array contents](#print-array-contents)         
[Add the contents of an array](#add-the-contents-of-an-array)         
[Find maximum value in an array](#find-maximum-value-in-an-array)         
[Find minimum value in an array](#find-minimum-value-in-an-array)         
[Creating a sequential file](#creating-a-sequential-file)         
[Printing the contents of a file using sentinel value](#printing-the-contents-of-a-file-using-sentinel-value)         
[Printing the contents of a file using EOF (end of file)         ](#printing-the-contents-of-a-file-using-eof-end-of-file)         
[Appending rows to an existing sequential file](#appending-rows-to-an-existing-sequential-file)         
[Creating a relative file](#creating-a-relative-file)         
[Reading from a relative file](#reading-from-a-relative-file)         
[Updating records in a relative file](#updating-records-in-a-relative-file)         


[2.3 Classification of systems - Activities]( https://github.com/Quobject/boscode-doc/blob/master/doc/IST/learning_activities.md#23-classification-of-systems---activities)   
[2.4 Hardware solutions]( #24-hardware-solutions )   


*3 Software*    


# 1 Pseudocode
It is expected that students are able to develop and interpret algorithms using pseudocode and flowcharts.

## Pseudocode guidelines
The pseudocode keywords are:

* for each procedure or subroutine
```
BEGIN name
END name
```
* for binary selection
```
IF condition THEN
  statements
ELSE
  statements
ENDIF
```
* for multi-way selection
```
CASEWHERE expression evaluates to
  A: process A
  B: process B
  ....
  OTHERWISE: process ...
ENDCASE
```
* for pre-test repetition
```
WHILE condition
  statements
ENDWHILE
```
* for post-test repetition
```
REPEAT
  statements
UNTIL condition
```
* for FOR/NEXT loops
```
FOR variable = start TO finish STEP increment
  statements
NEXT variable
```

In pseudocode:
* keywords are written in capitals
* structural elements come in pairs, eg for every BEGIN there is an END, for every IF there is an ENDIF.
* indenting is used to identify control structures in the algorithm
* the names of subprograms are underlined. This means that when refining the solution to a problem, a subroutine can be referred to in an algorithm by underlining its name, and a separate subprogram developed to show the logic of that routine. This feature enables the use of the top-down development concept, where details for a particular process need only be considered within the relevant subroutine.
*

___

## Examples

### Sequence 
```
Get firstNumber
Get secondNumber
sum = firstNumber + secondNumber
Display "the sum of your 2 numbers is ", sum
```

___

### Binary selection
```
myguess = 7
Get guess
IF guess = myguess THEN
  Display "Well done — you guessed my number!"
ELSE
  Display "That is not correct"
ENDIF
```

___

### Casewhere
```

N = 20  

CASEWHERE n is    
  less than 10 : n = n + 5
  30 : Display "n is thirty"
  greater than 50 : n = n + 30    
  OTHERWISE : n = n + 50  
ENDCASE  

Display n 

```

___

### Pre-test repetition: while
```
number = 5 

WHILE number < 200  
  Display number  
  Increment number by 2 
ENDWHILE 
	
```

___

### Post-test repetition: repeat
```
number = 0

REPEAT  
  Display number  
  number = number + 2 
UNTIL number > 200 
```

___

### FOR/NEXT or counted loop
```
FOR i = 1 to 12 STEP 1
  Display "12 x ", i," = ", (12 * i) 
NEXT i
```

___

### Subprogram
```
BEGIN Main
  Get a
  Get b
  Sum(a,b,c)
  Display "a + b = ", c
END Main

BEGIN Sum(a,b,c)
  c = a + b
END Sum
```
Note: The word <u>Sum</u> should be underlined in the above code
___

### Load array
```
BEGIN LoadArray
  i = 1
  Get DataValue
  WHILE DataValue < > "xxx"
    element(i) = DataValue
    i = i + 1
    Get DataValue
  ENDWHILE
  numElements = i
  Display "There are", numElements, " items loaded into the array" 
END LoadArray

```

___

### Print array contents
```
BEGIN PrintArrayContents
  element(1) = 3
  element(2) = 7
  element(3) = 10

  i = 1
  WHILE i <= 3
    Display element(i) 
    i = i + 1
  ENDWHILE
END PrintArrayContents
```

___

### Add the contents of an array
```
BEGIN SumArrayContents
  element(1) = 3
  element(2) = 7
  element(3) = 10

  i = 1
  sum = 0

  WHILE i <= 3
    sum = sum + element(i)
    i = i + 1
  ENDWHILE  

  Display "The sum of all of the elements in the array = " , sum 

END SumArrayContents
```

___

### Find maximum value in an array
```
BEGIN FindMAX
  element(1) = 3
  element(2) = 7
  element(3) = 23
  element(4) = 3
  element(5) = 7
  element(6) = 10

  maxIndex = 1
  i = 2 
  WHILE i < 7
    IF element(i) > element(maxIndex) THEN
      maxIndex = i
    END IF
    
    i = i + 1
  ENDWHILE

  max = element(maxIndex)
  Display "The highest value is ", max, " at position ", maxIndex 

END FindMAX
```
___

### Find minimum value in an array
```
BEGIN FindMIN
  element(1) = 3
  element(2) = 7
  element(3) = 23
  element(4) = 3
  element(5) = 7
  element(6) = 10

  maxIndex = 1
  i = 2 
  WHILE i < 7
    IF element(i) < element(maxIndex) THEN
      maxIndex = i
    END IF
    
    i = i + 1
  ENDWHILE

  max = element(maxIndex)
  Display "The highest value is ", max, " at position ", maxIndex 

END FindMIN
```

___

## Sequential file


### Creating a sequential file

Pseudocode
```
BEGIN CreateASequentialFile
  Open FriendsData for output

  firstName = "Joe"
  lastName = "Bloggs"
  emailAddress = "jbloggs@example.com"

  Write FriendsData from firstName, lastName, emailAddress

  firstName = "Jim"
  lastName = "Doe"
  emailAddress = "jdoe@example.com"

  Write FriendsData from firstName, lastName, emailAddress

  Close FriendsData
END CreateASequentialFile


```

___

### Printing the contents of a file using sentinel value

Pseudocode
```
BEGIN DisplayFileContents
  Open FriendsData for input

  Read firstName, lastName, emailAddress from FriendsData
  ’This is a priming read, performed just before entering the loop to provide
  'the first record (if there is one) for printing

  WHILE firstName <> “xxx”
    Display firstName, lastName, emailAddress
    Read firstName, lastName, emailAddress from FriendsData
    ’this reads subsequent records which can then be tested for the sentinel
    'value before they are processed
  END WHILE

  Close FriendsData
END DisplayFileContents

```

___

### Printing the contents of a file using EOF (end of file)

Pseudocode
```
BEGIN DisplayFileContents
  Open FriendsData for input

  Read firstName, lastName, emailAddress from FriendsData
  ’This is a priming read, performed just before entering the loop to provide
  'the first record (if there is one) for printing

  WHILE not EOF
    Display firstName, lastName, emailAddress
    Read firstName, lastName, emailAddress from FriendsData
    ’this reads subsequent records which can then be tested for the sentinel
    'value before they are processed
  END WHILE

  Close FriendsData
END DisplayFileContents

```

___


### Appending rows to an existing sequential file

Pseudocode
```
BEGIN AppendNewRows
  Open FriendsData for append

  Display “Please enter the details for the first new person to be added:”
  Display “Enter xxx for first name to indicate there are no more rows to be added.”

  Get firstName, lastName, emailAddress

  WHILE firstName <> “xxx”
    Write FriendsData from firstName, lastName, emailAddress

    Display “Please enter the details for the next new person to be added:”

    Get firstName, lastName, emailAddress
  END WHILE

  Close FriendsData
END AppendNewRows
```

___

## Relative file

### Creating a relative file

Pseudocode
```
BEGIN CreateARelativeFile
  Open ProductData for relative access

  productNumber = 1
  description = "Laundry Liquid 2L"
  quantity = 100
  price = 1.49

  Write ProductData from productNumber, description, quantity, price using productNumber

  ’note the use of the variable productNumber as the key field, specifying where this record will be written in the file.

  productNumber = 2
  description = "Mate Laundry Liquid 1L"
  quantity = 300
  price = 3.99

  Write ProductData from productNumber, description, quantity, price using productNumber

  Close ProductData
END CreateARelativeFile
```
___

### Reading from a relative file

Pseudocode
```
BEGIN ReadRecordsFromARelativeFile
  Open ProductData for relative access

  RequiredProdNumber = 1

  Read ProductData into productNumber, description, quantity, price using RequiredProdNumber
  ’note the use of the variable RequiredProdNumber as the key field, specifying where this record will be found in the file
  
  IF RecordNotFound THEN
    ’note the use of the flag RecordNotFound returned by the operating system 
    Display “Sorry – no such product”
  ELSE
    Display productNumber, description, quantity, price
  END IF
  
  Close ProductData
END ReadRecordsFromARelativeFile

```

___

### Updating records in a relative file

Pseudocode
```
BEGIN UpdateRecordsInARelativeFile
  Open ProductData for relative access

  RequiredProdNumber = 1

  Read ProductData into productNumber, description, quantity, price using RequiredProdNumber
  
  IF RecordNotFound THEN
    'note the use of the flag RecordNotFound returned by the operating system 
    Display “Sorry – no such product”
  ELSE
    Display productNumber, description, quantity, price
    newPrice = 1000

    Write ProductData from productNumber, description, quantity, newPrice using productNumber
    'update record using data for the new price and the existing data in the other fields

  END IF
  
  Close ProductData
END UpdateRecordsInARelativeFile

```
___