# Excel-crash-course
My excel syntax
ROUND FUNCTION
It calculates the rounded value of its inputs according to standard rules.
Syntax
=ROUND(number, num_digits)
number    Required. The number that you want to round.
num_digits    Required. The number of digits to which you want to round the number argument.

Remarks
If num_digits is greater than 0 (zero), then number is rounded to the specified number of decimal places.
If num_digits is 0, the number is rounded to the nearest integer.
If num_digits is less than 0, the number is rounded to the left of the decimal point.i.e -2(round off to the nearest hundredth.
To always round up (away from zero), use the ROUNDUP function.
To always round down (toward zero), use the ROUNDDOWN function.

VLOOK UP
It is an excel function to lookup and retrieve data from a specific column in a table.
V=Vertical lookup, significant when a table has column headers.
Purpose-To look up a value in a table by matching on the first column.
Syntax
=VLOOKUP(value, table, col_index, range_lookup)
Value-the value to look for in the first column in a table.
Table –the table from which to retrieve a value
Col_Index-the column in table from which to retrieve a value.
Range look up-True(approximate match),False(Exact match).

HLOOK UP
Horizontal look up, significant when a table has column headers.
Syntax
=HLOOKUP(value, table, row_index, range_lookup)

IF FUNCTION
Purpose 
Test for a specific condition
Return value 
The values you supply for TRUE or FALSE
Syntax 
=IF (logical_test, [value_if_true], [value_if_false])
Eg.=IF(C2>=60 ,“pass” ,”fail”)
Arguments 
logical_test - A value or logical expression that can be evaluated as TRUE or FALSE.
value_if_true - [optional] The value to return when logical_test evaluates to TRUE.
value_if_false - [optional] The value to return when logical_test evaluates to FALSE.

Nested IF statements
Refers to a formula where at least one IF function is incorporated inside another in order to test for more conditions and return morevpossible results.
For example, the following formula can be used to assign an grade rather than a pass / fail result:
Eg. =IF (C2<=40,”E”,IF(C2<=50,”C”,IF(C2<=60”B”,IF(C2<=70”A””Y”))))

  
 Comparison operator & Meaning
=	equal to
>	greater than
>=	greater than or equal to
<	less than
<=	less than or equal to
<>	not equal to

IF,WITH,AND,OR
The IF function can be combined with the AND function and the OR function. For example, to return "OK" when A1 is between 7 and 10, you can use use a formula like this:

IF(AND(C2>6,C2<10),”VERY GOOD”,”POOR”)
Translation: if C2 is greater than 6 and less than 10, return “VERY GOOD". Otherwise, return “POOR ".
To return B1+10 when A1 is "red" or "blue" you can use the OR function like this:
=IF (OR (A1”red” or A1”blue”) B1+10,B1)
Translation: if A1 is red or blue, return B1+10, otherwise return B1.




 
 
  
  
  


  
  
  


  
 
 
  
  


  



