# Subtraction

Scenario: When both are fraction

  given calculator is on
  
  when I type an integer
  I type slash
  I type an integer
  I type minus operator
  I type an integer
  I type slash
  I type an integer
  
  then I get an integer slash an integer
  
Scenario: When both are decimal

  given calculator is on
  
  when I type a decimal
  I type a minus operator
  I type a decimal
  
  then I may get decimal up to
  2 decimal places

Scenario: Both the digits are negative

  Given: calculator is on.

  When:Both the digits are negative.

  Then:Add two digits and put minus sign in front of result.

Scenario: One is positive and another is negative number

  Given: calculator is on.

  When: One number is positive and another is negative number.

  Then: Do addition of two digits.
  And the number which is large, put its sign in front of result.
