# Tax-Calculator
This interactive tax calculator estimates your tax burden.Enter income, deductions, and age. It handles basic errors (like non-numeric input) and highlights them with tooltips. Choose your age group from a dropdown. Upon submission, a modal displays the calculated tax based on pre-set brackets.Built with HTML, CSS, and JavaScript for a user-friendly experience.

## References & Requirements
- The tax calculation works based on this formula -
    - Overall income (after deductions) under 8 (≤) Lakhs is not taxed.
        - Ex - if Gross Annual Income + Extra Income - Deductions =  6 Lakhs, no tax
        - if Gross Annual Income + Extra Income - Deductions =  9 Lakhs, tax
    - Income over 8 (>) Lakhs, the amount over 8 Lakhs is taxed at
        - 30% for people with age < 40
        - 40% for people with age ≥ 40 but < 60
        - 10% for people with age ≥ 60
        - Example
            - Age = 34, Income = 40 Lakhs, no deductions, tax = .3 * (40 - 8) = .3 * 32 = 9.6 Lakhs
- Do not restrict the user from entering incorrect values like characters in the number fields
    - Highlight an error icon to the right of the input field (shown as an example in the above image as a circle with `!`). Hovering over it should show the error in a tooltip
    - If no errors are present, don't show the error icon
    - This should be present in all the number fields
- The age dropdown field should have 3 values -
    - <40
    - ≥ 40 & < 60
    - ≥ 60
    - If the user has not entered this value and clicks on submit, show an error icon hovering over which should show that the input field is mandatory
- Error icons should not be visible in the form by default.
- Clicking on submit should show a modal which would show the final values based on the above calculations.

## Features:
- Calculate taxes based on income, deductions, and age brackets.
- Handle invalid input (characters in numbers) with real-time error icons and tooltips.
- Offer a dropdown menu for selecting age range (<40, 40-60, >=60).
- Require age selection with an error indicator for a missing value.
- Display final tax calculations in a modal window upon submit.

## Test Cases
**Case 1: Tooltip is shown when hovering over the question mark icons**

<img width="357" alt="case 1" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/3acee68c-2150-4fae-8fce-db3c7cdf4a02">

**Case 2: Display error icons if the user clicks the submit button without entering input. Error message states "This input field is mandatory"**

<img width="376" alt="case 2" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/29506e5e-d067-4b20-84b7-999e6426906f">

**Case 3: Error icons will appear if characters are entered instead of a number. Error message states "Please enter numbers only."**

<img width="367" alt="case 3" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/7f53eb92-13e9-4375-ac1d-6ed6e08e70af">

**Case 4: Error icons will appear if a negative value is entered. Error message states "Please enter non-negative numbers only"**

<img width="367" alt="case 4" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/b8a5316d-1900-413b-8fdb-67a2238152f2">

**Case 5: Display error icon when all other fields are filled except the age group field. Error message states "This input field is mandatory."**

<img width="367" alt="case 5" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/7ae38fd3-7b60-4cd8-8ec0-9438f591b52a">

**Case 6: If Gross Income +  Extra Income - Total Deductions is ≤ 8 lakhs then no tax is applicable. So overall income will be Gross Income +  Extra Income.**

<img width="353" alt="case 6 (a)" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/c4375987-8d44-4eb8-9009-fed961c6d2f5">
<img width="368" alt="case 6(b)" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/4dfceac6-d81f-4008-b348-b8a940a5a74d"></span>


**Case 7: If Gross Income +  Extra Income - Total Deductions is > 8 lakhs then income tax is applicable based on age group. So overall income will be calculated accordingly.**

*1. Age < 40*

<img width="349" alt="case 7a" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/e4b05669-3e36-4e33-9546-2e3b60103e83">
<img width="340" alt="case 7a1" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/f902a589-2bc4-43cf-8163-d93d03046a64"> 


*2. Age ≥ 40 & < 60*

<img width="349" alt="case 7 b" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/fa859d29-aeb6-4722-a527-4f65d2a273a3">
<img width="340" alt="7 b 1" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/d0234acc-9ab6-4997-970a-9c1830ab77ca">

*3. Age ≥ 60*

<img width="349" alt="case 7 c" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/2bac5f85-c7cb-4273-ae67-9bd915337dc9">
<img width="340" alt="case 7 c 1" src="https://github.com/priyansh201480/Tax-Calculator/assets/140069604/4d48b419-2965-4a77-92c4-56b549ee7ec3">


