# Addition

Scenario: Add two numbers
  
  Given I have a calculator that's turned on.

  When I enter "first number"
  And I press "+" button
  And I enter "second number"
  And I press "=" button
  
  Then I see the "added sum" as the result

Scenario: Add more numbers

  Given I have a calculator that's turned on
  
  When I enter all the numbers by pressing "+" alternatively
  And press "=" after entering last number
  
  Then I see the 'added sum" as the result

Scenario: Result is too large to display (or overrunning the limits)

Scenario: Numbers can be negative

Scenario: Numbers can be fraction

Scenario: Number can be irrational

Scenario: Length of each number

Scenario: If number1 or number2 is not entered

Scenario: If the number is real/complex

Scenario: If we are inbetween some operation
