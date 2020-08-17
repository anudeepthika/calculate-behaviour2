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
  
  When I enter "first number"
  And I press "+" button
  And I enter "next number"
  And I press "+" button
  And I enter "next number"
  And repeat this until you enter last but one number
  And press "=" after entering last number
  
  Then I see the 'added sum" of all the entered numbers

Scenario: Result is too large to display (or overrunning the limits)

  Given I have a calculator that's turned on
  
   When I enter "first number"
  And I press "+" button
  And I enter "next number"
  And I press "+" button
  And I enter "next number"
  And repeat this until you enter last but one number
  And press "=" after entering last number
  
  Then I see the added result in exponential form

Scenario: Numbers can be negative

Scenario: Numbers can be fraction

  Given I have a calculator that's turned on.

  When I enter "first fractional number"
  And I press "+" button
  And I enter "second fractional number"
  And I press "=" button
  
  Then I see the "added sum" as the fractional number
  
Scenario: Number can be irrational

Scenario: Length of each number

Scenario: If number1 or number2 is not entered

  Given I have a calculator that's turned on.
  
  When I enter "first number"
  And I press "+" button
  And then I press "=" button

Then I see an error "enter atleast two numbers".

Scenario: If the number is real/complex

Scenario: If we are inbetween some operation
