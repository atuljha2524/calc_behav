# Addition

Scenario: Adding 2 negaative numbers
  
  Given The calculator is turned on

  When I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  I type in "plus"
  I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  
  Then I see "added negative number" as the result

Scenario: Adding fractions
  
  Given the calculator is on
  
  When I type a positive number
  I type slash
  I type a positive munber
  I type plus
  I type a positive number
  I type slash
  I type a positive munber
  
  Then i see a number slash and a number
  
Scenario: Addition of +ve and -ve number
  
  Given the calculator is on
  
  When I type a positive number
  I type plus
  I type in "bracket open"
  I type in "negative number"
  I type in "bracket close"
  
  Then I see the number may be positive or negative depending on the value of 2 numbers
  
Scenario:
  
  Given (state the initial condition)
  
  When (state the event)
  
  Then (state the effect)
  
