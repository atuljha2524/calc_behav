# Multiply

Scenario: Result overflow
  
  Given calculator is on
  
  When I type integer max
  I type * operator
  I type integer max
  I type equals to
  
  Then I see multiplication in string form
  
Scenario: Signs of number
  
  Given calculator is on
  
  When I type a signed number
  I type * operator
  I type a signed number
  I type equals to
  
  Then if one of them is negative I get negative answer
  if both are negative I get positive answer
  if both are positive I get positive answer
  
Scenario: Zero value multiplication
  
  Given calculator is on
  
  When I type a zero
  I type * operator
  I type a number
  I type equals to
  
  Then I get zero
  
Scenario: Multiplication by 1
  
  Given calculator is on
  
  When I type a number
  I type * operator
  I type one
  I type equals to
  
  Then I get same number as an answer

Scenario: Decimal value multiplication
  
  Given calculator is on
  
  When I type a decimal number
  I type * operator
  I type a decimal number
  I type equals to
  
  Then I may get decimal number
  up to 2 decimal places
