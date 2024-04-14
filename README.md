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

![case 1](https://github.com/priyansh201480/Tax-Calculator/assets/140069604/e2cd5b85-3728-4c47-8870-8b333a2aed23)

**Case 2: Display error icons if the user clicks the submit button without entering input. Error message states "This input field is mandatory"**<br/>
*Image 1:* Default State & *Image 2:* After clicking the submit button for empty fields

![image](https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/646deb3a-2be6-499b-8da7-1cc7e652c2bb)

**Case 3: Error icons will appear if a negative value is entered in the Number fields. These fields only accept 0 or positive numbers. Error message states "Please enter non-negative numbers only"**

<img src="https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/15bd46c9-f922-4518-9b76-0fef9a4518b8" alt="Case 3" width="500"/><br/>

**Case 4: Error icons will appear if characters are entered in the Number fields instead of a number. Error message states "Please enter numbers only."**

<img src="https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/b4467856-a6a6-48f9-b472-e71ff0f2ccdc" alt="Case 4" width="500"/><br/>

**Case 5: Display error icons when all number fields are filled, but the age group is not selected. Error message states "This input field is mandatory."**

<img src="https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/a560ece8-616c-4865-85a4-f5543e2b1738" alt="Case 5" width="500"/><br/>

**Case 6: If Gross Income +  Extra Income - Total Deductions is ≤ 8 lakhs then no income tax is applicable. So overall income will be Gross Income +  Extra Income.**

![image](https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/17dc19b6-1a2e-4714-9f67-7c7837c5f573)

**Case 7: If Gross Income +  Extra Income - Total Deductions is > 8 lakhs then income tax is applicable based on age group. So overall income will be calculated accordingly.**<br/>
*1. Age < 40*

![image](https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/a9188665-8a8b-4268-8f84-26f5f04a2c2b)

*2. Age ≥ 40 & < 60*

![image](https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/90798032-3d62-40bb-ba9a-dd14ce28b2a3)

*3. Age ≥ 60*

![image](https://github.com/KamiyaGaikwad/Tax-Calculator/assets/79163529/a2f0867e-4d9e-4fbc-af15-eb408b1e1b50)


