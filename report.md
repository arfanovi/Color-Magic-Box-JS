
What is switch-case break?
The switch-case break is a keyword in programming used to exit a switch-case block.

How is it used?
It is typically placed after each case block in a switch statement to terminate the switch-case block.

When to use it?
You use switch-case break when you want to execute a specific case and then exit the switch block immediately, 
without executing the subsequent cases.


Switch: It's like checking your mood.
Cases: These are your options based on your mood.
Execution: Do something depending on your mood.
Default: If you don't feel any specific way, do this.

So, switch-case helps your program decide what to do based on different conditions, just like you pick a toy based on your mood!




const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question("Menu:\n1. Play Game\n2. View High Scores\n3. Settings\n4. Exit\nEnter your choice:", function(choice) {
    switch (parseInt(choice)) {
        case 1:
            console.log("Starting the game...");
            break;
        case 2:
            console.log("Displaying high scores...");
            break;
        case 3:
            console.log("Opening settings...");
            break;
        case 4:
            console.log("Exiting the program...");
            break;
        default:
            console.log("Invalid choice! Please select a valid option.");
    }
    rl.close();
});


Import readline module for user interaction.
Create interface for reading user input.
Prompt user with menu and await input.
Handle user input using switch statement.
Execute actions based on user's choice.
Handle invalid input with default case.
Close the readline interface after processing.
