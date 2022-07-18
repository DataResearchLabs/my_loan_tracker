<img align="left" src="https://github.com/DataResearchLabs/my_loan_amortization/blob/main/img/application_icon.png" width="64px">

# My Loan Tracker (MLT) 
[![License: CC0](https://img.shields.io/badge/License-MIT-red)](LICENSE "MIT License by DataResearchLabs (open source)")
![current_build Office_365](https://img.shields.io/badge/Excel_Version-Office_365-yellow)
[![Latest Release](https://img.shields.io/badge/Latest_Release-5.01.44308-blue)](https://github.com/DataResearchLabs/my_loan_amortization/tree/main/download)
[![YouTube](https://img.shields.io/badge/YouTube-DataResearchLabs-brightgreen)](https://www.youtube.com/DataResearchLabs/featured)

## 1 - Overview
* "My Loan Tracker" is loan repayment scheduler enabling you to plan, track, and adjust how much you're paying each period.  You can schedule routine "pre-payments to principle" on top of the regular period payments to reduce the total interest paid out and the lifespan of the loan.  You can even track the occasional one-off extra pre-payments.
* The tool is simple to use.  All the formulas are done for you. Just fill out the six Loan Parameters in yellow boxes at the upper left corner of the spreadsheet, and everything else will be auto-calculated.  You can alter the paramters to try out different scenarios.  You can even go type in "one-off" pre-payments down in the schedule for accurate change tracking.
* View the Graphs tab to see a standard "Loan Amortization Chart" depicting remaining balance, principle, and interest paid at any given point in the life of the loan.  There is also a "Payment Type" graph comparing total interest as originally scheduled versus after pre-payments have been applied.  


## 2 - Quick Start Guide

### 2.1 - Legend
The general rule is that you only type into light yellow cells, and only on the first worksheet "Amortization Schedule".<br>
Everything else is a calculated cell.
<br>
<img src="https://github.com/DataResearchLabs/my_loan_amortization/blob/main/img/02_01_legendX.png" width=700>
<br><br>

### 2.2 - "The Inputs" = Just 6 Loan Parameters
To use this spreadsheet, you just need to fill out the minimum set of parameters on the "Amortization Schedule" worksheet as follows (cross reference screenshot fields to the right):
<img align="right" src="img/02_02_loan_parametersX.png" width="300">
1. **Original Loan Amount**: The total loan amount (principal) that you are borrowing and will need to pay back
2. **Annual Interest Rate**: The loan interest rate															
3. **Loan Period in Years**: The length of time in years to payoff the loan assuming no pre-payments to principal are made.  Typical values are
15-year and 30-year, but we've added 40-year too if they come about.
4. **Number of Payments Per Year**: This is typically 12 for monthly payments.
5. **Date of First Payment**: Enter the year, month and day that payments will start.  I typically prefer setting the day to the first ("1").
6. **Extra Payment / Early Principal**: This value is optional.  Leave it at $0.00 to stick with the original loan terms and length.  However, if you want to pay off the loan early and reduce total interest you can try out different values to pre-pay each period to understand the impact (example: pre-paying $500 a period might save 10.5 years off the loan and save $150,000 in interest to the bank...savings you can put to use elsewhere.  Play with this value to better understand your loan and various scenarios for paying it off faster.
<br><br>

### 2.3 - "The Outputs" = Loan Summary Box + Amortization Schedule
There are three sections on the "Amortization Schedule" worksheet shown below.<br>
* **Section #1** is the "**Loan Parameters**" you just entered in the previous section.  Notice that the "Payment per Period" has been calculated for you (i.e. - the Monthly payment).
* **Section #2** is the "**Loan Summary**" with the original terms including total interest paid out over the life of the loan, the total cost of the loan (principal + interest), the total number of payments, the payoff time in years, and the final payoff date.
* **Section #3** is the "**Amortization Schedule**" showing you each payment's date, beginning balance, scheduled payment (interest + principal), total payment (including any extra principal pre-payment you enter in the yellow box), the remaining balance on the loan, the cumulative principal paid and the cumulative interest paid on the loan.
<img src="img/02_03_main_page_sectionsX.png">
<br>

### 2.4 - "Pre-Payment to Principal" / Early Payoff
There are two ways of entering extra payments in this spreadsheet: (1) as a Loan Parameter, and (2) directly down in the amortization schedule as a one-off.
* **Bullet #1** below is where you enter a regular extra payment (to principal) that you want to occur with every scheduled payment.  In the example below, an extra $125.00 will be applied to principal every month.  You can see the $125 repeating down in the amortization schedule above and below bullet #2.  This reduces the total life of the loan by 5.42 years and 65 payments in cells I10 and I11.
* **Bullet #2** is where you enter unique one-time payments that are not scheduled.  In the example below, the user made a one-time extra payment of $500 on November 1 because she received a spot bonus at work and wanted to apply that to her mortgage principal.
* _**Pro Tip #1:** If you have already been paying your mortgage for some time and just started using this spreadsheet to track, this is where you would manually enter all of your pre-payments (type the values in over the formulas) to precisely model your current mortgage histories if you varied from the regular payments._
* _**Pro Tip #**: The way I use these two pre-payment approaches is by entering the minimum pre-payment amount I know I can hit every month (the $125 in example below at bullet #1). But then every month I try to pre-pay more and just over-type the formula in the "Extra Payments" column at bullet #2._
* **Bullet #3** shows how the Loan Summary section "lights up" after pre-payments are detected.  Notice the 
"w/Pre-Payments" column is no longer grayed out because the values changed.  Notice the "Total Savings" column with green values indicating how much money you saved by not paying interest and how much time you reduced on the life of the loan.
* **Bullet #4** shows the impact of paying extra principal above the regular scheduled amount.  For example, the remaining balance dropped by about $750 and the cumulative principal jumped from $1,127 to $1,881.
<img src="img/02_04_pre_payment_to_principalX.png">
<br>

### 2.5 - "Payment Tracking"
* **Bullet #1** in the screenshot below is a drop-down box labeled "Most Recent Payment Date".  This drop-down contains dates of all loan payments.  Use it to select the current pay period and popup the loan status data shown in the next bullet.
* **Bullet #2** shows the tracking data window that appears upon selecting the most recent payment date.  The left column is titled "Paid Thus Far" and the right column is "Balance Remaining".  Use these columns to see how many payments, years, and dollars are completed thus far versus the balance remaining.
<img src="img/02_05_payment_trackingX.png">
<br><br>

## 3 - "Open Source"
### 3.1 - This Product is Open Source
There was going to be a Free edition and a Standard edition (for $4.99).  However, Google Sheets strips the Microsoft Excel password protection thereby enabling anyone to view the formulas and edit the workbook, effectively bypassing the security.
<br><br>
**I do have one request**:  If you benefit from using this product and can afford it, please visit the Etsy site below and make a purchase.  Think of it as donating $4.99 to help me out.  It is optional though, no obligation.
|Location | URL |
|:----------------------------------|:----------------------------------|
|Purchase (Donate) from Etsy: | https://www.etsy.com/shop/DataResearchLabs|
|Download for free from GitHub: | https://github.com/dataresearchlabs/my_loan_tracker|


### 3.2 - How to "Unlock" the Spreadsheet (for editing / to view formulas)
1. Download or purchase a copy of the spreadsheet
2. Open the file in XL  and click the "Amortization Schedule" tab
3. Click menu items "Home"  >  "Format"  >  "Unprotect Sheet"
4. Because this open source, leave the password blank...the worksheet is simply unlocked
<br><br>


## 4 - Additional Training
For aditional training and related materials, please visit my YouTube site at: https://www.youtube.com/c/DataResearchLabs/featured														


