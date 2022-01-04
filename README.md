# Expense-Tracker

## REFERENCES

https://reactjs.org/docs/hooks-reference.html

https://docs.speechly.com/tutorials/react/

https://github.com/speechly/speechly/blob/main/libraries/react-client/docs/modules/_index_d_.md

https://v4.mui.com/

https://www.youtube.com/watch?v=sP7ANcTpJr8

## Speechly Config

#### https://gist.github.com/adrianhajdin/aa28f5c4928d05fe55aae37d83dc98d2
  category_income = [
    Business
    Investments
    Extra income
    Deposits
    Lottery
    Gifts
    Salary
    Savings
    Rental income
]
category_expense = [
    Bills
    Car
    Clothes
    Travel
    Food
    Shopping
    House
    Entertainment
    Phone
    Pets
    Other
]
*create_transaction [Create|Finish|Save] {transaction}
*cancel_transaction [Cancel|Delete|Remove|Clear] {transaction}
*add_category [Set|Change] category {to} [$category_expense|$category_income](category)
*add_category {[i mean|i meant|i said]} {the} ![category {[is|of]} | [$category_expense|$category_income](category)]
*add_date [Set|Change|Add] date {[to|for]} $SPEECHLY.DATE(date)
*add_date {[i mean|i meant|i said]} {[{the} date is|for]} $SPEECHLY.DATE(date)
*add_amount [Set|Change] amount {to} $SPEECHLY.NUMBER(amount) {dollars}
*add_amount {[i mean|i meant|i said]} {{the} amount {[is|of]}} $SPEECHLY.NUMBER(amount) {dollars}
*add_expense {Add} {an} expense ![{[for|of]} $SPEECHLY.NUMBER(amount) {dollars} | {in} | {category} | [$category_expense|$category_income](category) | {[for|in]} $SPEECHLY.DATE(date)]
*add_expense $SPEECHLY.NUMBER(amount) {[dollar|dollars]} expense {in} ![{category} | [$category_expense|$category_income](category)] {[for|in]} $SPEECHLY.DATE(date)
*add_income {Add} {[{an} income|{a} balance]} ![{[for|of]} $SPEECHLY.NUMBER(amount) {dollars} | {in} | {category} | [$category_expense|$category_income](category) | {[for|in]} $SPEECHLY.DATE(date)]
*add_income $SPEECHLY.NUMBER(amount) {[dollar|dollars]} [income|balance] {in} ![{category} | [$category_expense|$category_income](category)] {[for|in]} $SPEECHLY.DATE(date)
