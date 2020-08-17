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
