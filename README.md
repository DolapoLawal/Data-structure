BEGIN
    distinct_elements ← empty array
    sum ← 0
    
    FOR each element x in Set 1 DO
        IF x is not in distinct_elements THEN
            Append x to distinct_elements
            sum ← sum + x
        END IF
    END FOR
    
    FOR each element y in Set 2 DO
        IF y is not in distinct_elements THEN
            Append y to distinct_elements
            sum ← sum + y
        END IF
    END FOR
    
    Print sum as output
END

distinct_elements = [3, 1, 7, 9, 2, 4]
sum = 13


Start
Define a function called "dot_product" with the following parameters:
a. v1: array of real numbers
b. v2: array of real numbers
c. n: size of the arrays v1 and v2
d. Returns the scalar product of v1 and v2
Initialize ps = 0
For i = 1 to n, do the following:
a. ps = ps + (v1[i] * v2[i])
End function
Define a function called "is_orthogonal" with the following parameters:
a. v1: array of real numbers
b. v2: array of real numbers
c. n: size of the arrays v1 and v2
d. Returns a boolean value indicating whether the vectors are orthogonal or not
Initialize a variable "ps" to store the scalar product of v1 and v2
Call the "dot_product" function with the following arguments:
a. v1
b. v2
c. n
If ps = 0, return true (vectors are orthogonal)
Else, return false (vectors are not orthogonal)
End
