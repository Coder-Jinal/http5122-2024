# Front-End Web Development
Course Code: HTTP 5122

Academic Year: 2025-2026

This course delivers the fundamentals of computer programming and introduces the tools for creating interactive web pages using the JavaScript programming language.

# Links
https://javascript.info/

# Images
![JavaScript Code Sample](JS.png)


> **Note**: This course lays the groundwork for front-end development with JavaScript, a crucial skill for creating dynamic and interactive web applications.

# Code Example: 

Simple JavaScript code for calculating the account balance and upadate the account details after making a deposit or withdrowing

var CustomerDetails = 
{
    LastName: "Patel",
    BrachNumber: 123,
    accountBalance: 500.25,
    interestRate: 1.03,
    multipleAccounts: true,
    makeDeposit: function (depositAmount) {
        CustomerDetails.accountBalance = CustomerDetails.accountBalance + depositAmount;
        return "Thank You. Your account balance is now: $" + CustomerDetails.accountBalance.toFixed(2);
    },
    makeWithdrawal: function (withdrawalAmount) {
        CustomerDetails.accountBalance = CustomerDetails.accountBalance - withdrawalAmount;
        return "Thank You. Your account balance is now: $" + CustomerDetails.accountBalance.toFixed(2);
    },
    addInterest: function () {
        var interestAmout;
        if (CustomerDetails.multipleAccounts === true) {
            interestAmout = CustomerDetails.interestRate + 0.005;
        }
        else{
            interestAmout = CustomerDetails.interestRate;
        }
        CustomerDetails.accountBalance = CustomerDetails.accountBalance * interestAmout;
        return "Thank You. Your current balance is now: $" + CustomerDetails.accountBalance.toFixed(2);
    }
};
console.log(CustomerDetails.makeDeposit(200));
console.log(CustomerDetails.makeWithdrawal(75));
console.log(CustomerDetails.addInterest());
