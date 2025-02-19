# COP2664-1-Lesson-4-Programming-Exercise-4.2
This is a repository link of the COP2664-1 Lesson 4 Programming Exercise 4.2

// This program is designed to to compute the sum of the two integers and see if the values return equal, compute and return the absolute difference of n and 51, accept two integer values and return true if one of them is 20 or if their sum is 20, accept two integer values and return true if one is negative and one is positive, accept two integer values and test if they are both in the range 20..30 inclusive, or they are both in the range 30..40 inclusive.

import Foundation // Imports the Foundation library

// Question 1
func sum(a: Int, b: Int) -> Int { // Defines a function called sum that takes two integer parameters and returns an integer value
  if a == b { // If the two parameters are equal, return double the sum
    return (a + b) * 3 // Returns the doubled sum
  } else { // If the two parameters are not equal, return the sum
    return a + b // Returns the sum
  }
}
print(sum(a: 2, b: 2))
// Question 2
func diff(n: Int) -> Int { // Defines a function called diff that takes an integer parameter and returns an integer value
  if n > 51 { // If the parameter is greater than 51, return the absolute difference
    return (n - 51) * 2 // Returns the absolute difference multiplied by 2
  } else { // If the parameter is less than or equal to 51, return the absolute difference
    return 51 - n // Returns the absolute difference
  }
}
print(diff(n: 53))
// Question 3
func test(x: Int, y: Int) -> Bool { // Defines a function called test that takes two integer parameters and returns a boolean value
  if x == 20 || y == 20 { // If either parameter is equal to 20, return true
    return true 
  } else if x + y == 20 { // If the sum of the parameters is equal to 20, return true
    return true
  } else { // If the parameters do not meet any of the conditions, return false
    return false
  }
}
print(test(x: 20, y: 10))
// Question 4
func test2(x: Int, y: Int) -> Bool { // Defines a function called test2 that takes two integer parameters and returns a boolean value
  if x < 0 && y > 0 || x > 0 && y < 0 { // If either parameter is negative and the other is positive, return true
    return true
  } else if x < 0 && y < 0 { // If both parameters are negative, return true
    return true
  } else { // If the parameters do not meet any of the conditions, return false
    return false
  }
}
print(test2(x: -1, y: 1))
// Question 5
func test3(x: Int, y: Int) -> Bool { // Defines a function called test3 that takes two integer parameters and returns a boolean value
  if x >= 20 && x <= 30 && y >= 20 && y <= 30 { // If both parameters are in the range 20..30 inclusive, return true
    return true
  } else if x >= 30 && x <= 40 && y >= 30 && y <= 40 { // If both parameters are in the range 30..40 inclusive, return true
    return true
  } else { // If the parameters do not meet any of the conditions, return false
    return false
  }
}
print(test3(x: 20, y: 20))
