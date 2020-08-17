# Addition

Scenario: Adding 2 negative numbers
  
  Given The calculator is on

  When I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  I type in "plus"
  I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  I type equals to
  
  Then I see "added negative number" as the result

Scenario: Adding fractions
  
  Given the calculator is on
  
  When I type a positive number
  I type slash
  I type a positive number
  I type plus
  I type a positive number
  I type slash
  I type a positive number
  I type equals to
  
  Then i see a number slash and a number
  
Scenario: Addition of positive and negative number
  
  Given the calculator is on
  
  When I type a positive number
  I type plus
  I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  I type equals to
  
  Then I see the number may be positive or negative depending on the value of 2 numbers
  
Scenario: Addition of decimal number
  
  Given the calculator is on
  
  When I type a decimal number
  I type a plus operator
  I type a decimal number
  I type equals to
  
  Then I may get decimal number
  up to 2 decimal places
  
Scenario: Typing the operator more than once
  
  Given the calculator is on
  
  When I type an integer
  I type a plus operator
  I type a plus operator
  I type an Integer
  I type equals to
  
  Then the operator buffer updates to the last operator
  I typed and I see the addition of two
  integer
