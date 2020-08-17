# Division

Scenario: Division by 0 when operand 1 is any number

  When we enter first non zero operand.
  And we divide it with 0.

  Then it gives infinity as a result.

Scenario: Divide 0 by any number

  When we enter first operand as 0.
  And we divide it with any number.

  Then it gives 0 as a result.

Scenario: Division when both operands are 0

  When both operands are 0 in division.

  Then result is also zero.

Scenario: Recurring decimal case

  When the result of division is recurring.
  That is after decimal large number occurs.

  Then round off after 2 decimal digits.

Scenario: More than one times "/" occurs

  When more than one times / operator occurs in division.

  Then consider one divide operator between two operands.
  And if after / operator no any operand is present.
  Then neglect that / operator.
