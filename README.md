# SoftEngineering-FinalExam



Bachelor of Science in Computing

Software Engineering

 Year 2022-23 / Semester 2


Internal Examiner:	Wei Ren
Internal Moderator:	Wenhao Fu
External Examiner:	Maria Barry 
Date:	24/04/2023
Duration:	2 Hours
Time:	10:00-12:00
Exam Weighting:	60%
Exam Delivery:	Computer


Instructions

a)	This paper contains 1 section with 1 question.
b)	You must attempt all parts of the question.
c)	All questions are marked out of 100.
d)	Please write all answers on the script provided.
e)	Clearly number all questions.
f)	This is an open-book exam.


Please do not turn over this page until instructed to do so. The use of programmable or text storing calculators is expressly forbidden. Please note that where a candidate answers more than the required number of questions, the examiner will mark all questions attempted and then select the highest scoring ones. 



Question 1

Please answer the question based on the following scenario: You are managing a software development team that has been invited by “Dorset Bank” to develop an operating system for their ATM machines. The ATM machines should allow clients to withdraw money at any time and deposit cash or checks. Additionally, the machines should display the client's account balance. You have 4 weeks to do this project.


a)	Select a development method for this project and provide the reason for your choice, (e.g. waterfall development method, agile development method, etc.).
Taking into consideration the nature of this project, the best approach in order to deliver the OS for ATM machines within the initial deadline would be applying waterfall development method to the project. That way, the development team will have a clear vision of what requirements need to be completed every week. Moreover, the development team will be able to help each other in case one of the team members is falling behind in their tasks.
[14 marks]

b)	Provide a comprehensive list of the steps involved in the software development process.

Below is a list containing the steps required in order to fully deliver Dorset Bank – ATM machines OS.
- Define what requirements are necessary in order to develop ATM machines OS.
- Decide which are the best technologies to integrate this project. 
- Organize requirements priority to be implemented according to the project scope and deadline.
- Start the development of the application
- Run tests for every function implemented (dummy data)
- Connect the new OS to the already existent Bank database
- Run more tests with real data.
- Deploy the application to production level
- Deliver the final product to the customer

 [5 marks]










c)	Write a requirement document based on the client's previous requirements, including functional requirements, interface requirements infrastructure requirements.
This project is a rather simple application to implement. However, it will be handling sensitive data such as card numbers, bank account balance, and other sensitive personal data. Therefore, security will be a key factor when developing this OS. Considering Dorset Bank already has their own database where they store their customers bank accounts details, the development team main focus is to develop a user-friendly interface for this operating system as well as to connect the new ATM machines OS to the bank’s database. 

Infrastructure Requirements
-	Back-End (Connecting to database server and creation of functions and interfaces for balance and cash withdraw/deposit) - C# 
-	Front-End (Connecting to back-end interfaces) – HTML, CSS, Bootstrap.

Functional Requirements

-	Users can access their bank account as long as they have their physical card with them along with its pin.
-	Users can withdraw money from their bank accounts.
-	Users can deposit cash or checks in their bank account.
-	Users can check their balance on the screen.

Interface Requirements
-	Welcome screen with instructions on how to use the ATM machines.
-	Authentication Screen.
-	Main Menu Screen with options. (withdraw, deposit cash, deposit check, and balance)
-	Task completion Screen confirming the transaction was successful to the users.


[25 marks]





















d)	Create a Use Case Diagram.

 
[6 marks]

e)	Create a Gantt Chart to manage development process.
 
[10 marks]










f)	Provide an example code snippet, in any programming language, that includes the class name, function name, and any other necessary variables, to demonstrate how to achieve the goals of this project. You do not need to include the implementation details of the functions. Please show class diagrams or template code.
Below is a very simple example of how the classes in this operating system will work.

Private double balance;

Private static void double Withdraw(double amount, double balance){
PrintL.system(“Enter amount you want to withdraw”);
	If(amount <= balance)
{
Balance -= amount;
} else
{
PrintL.system(“Sorry, insufficient balance.Try a different amount”);
}
}

As we can see, there will be conditions that will keep the OS from 
 

[20 marks]

g)	Provide a detailed explanation of the validation and verification process that should be followed to ensure the successful completion of this project.
In order to validate the customer bank account credentials, the development team should integrate a two steps verification before the user can withdraw or deposit any money in their accounts. First step verification would be the physical card which the bank provided to that specific customer. After inserting the card into the ATM machine, the software will send a request to the bank database. If the card credentials exist within the database, the second step verification will be prompted. The customer will then, be asked to enter his card pin in order to proceed to the cash functions.
Once the customer is authenticated, they will be able to perform withdraws, deposits or check their account balance. Depending on what the customer decides to do, the software will send another request to the server. If all the conditions to withdraw or deposit cash are met, e.g. (enough money in the bank account, etc.), the ATM machine OS will send a POST method to the database in order to update its contents.
[15 marks]

h)	Create a repository on GitHub and upload your answers to it. Please note that the answers on GitHub will not be considered for marking, so it is essential to submit all your answers to Moodle before the exam deadline.
[5 marks]



[Total 100 marks]
