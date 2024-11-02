# showing-the-BDD-Scenario-for-Searching-a-Product-based-on-Availability
Scenario: Searching products by availability
  Given the following products
    | name      | category | available |
    | ToyCar    | Toys     | true      |
    | BoardGame | Games    | false     |
  When I search for products that are available
  Then I should see 1 available product
