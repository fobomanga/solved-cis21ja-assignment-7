Download Link: https://assignmentchef.com/product/solved-cis21ja-assignment-7
<br>
Modify the code of assignment 5 so that the program is made of procedures. The resulting code should still do the same work as assignment 5: add 2 unsigned, 16-bit integers and print the sum as a numeric text string.

<strong>Details</strong>Take the code of assignment 5 and divide it into the following 4 procedures.

<ol>

 <li>A readInput procedure that uses <u>the stack</u> to pass data.</li>

</ol>

The procedure prompts the user for a 16-bit integer and keeps prompting until there is a valid input.  The procedure:

<ol>

 <li>has 2 input arguments: the address of the prompt string and the address of the error string (for “input out of range” error)</li>

 <li>returns a valid user input</li>

</ol>




<ol start="2">

 <li>An adding procedure that uses <u>the stack</u> to pass data.</li>

</ol>

The procedure adds the 2 numbers, passes back the sum through its address, and returns a boolean to show whether the sum is valid. The procedure:

<ol>

 <li>has 3 input arguments: the 2 input numbers and the address of the sum. The sum is passed back through the address</li>

 <li>returns a boolean to show valid or not valid sum</li>

 <li>A printOutput procedure that uses <u>registers</u> to pass data.</li>

</ol>

The procedure converts the sum to a numeric text string and uses writeString to print the text string. The procedure:

<ol>

 <li>accepts 3 input arguments: the sum, and the address of the text explanation string and the address of the numeric text string</li>

 <li>has no return value</li>

</ol>




<ol start="4">

 <li>A main procedure that coordinates the calling of the 3 previous procedures. The main procedure:</li>

 <li>calls the readInput procedure twice, once for each user input</li>

 <li>calls the adding procedure and checks the boolean return value</li>

 <li>calls the printOutput procedure if the sum is valid</li>

 <li>loops to ask the user to continue or end</li>

</ol>

<strong> </strong>

<strong>Additional requirements</strong>

<ul>

 <li>Document your program to get full credit.</li>

 <li>Create 3 additional variables in the .data section for the 2 user input and the sum. These should all be <u>16-bit</u></li>

 <li>Use 16-bit registers for calculation (the adding procedure)</li>

 <li>Make sure the procedures pass data either through the stack or through registers as described above. 2pts per procedure are for using the right way to pass data.</li>

 <li>For the 2 procedures that pass data through the stack, the code should clear out the stack frame completely after the procedure call is done. 1 pt per procedure is for clearing out the stack correctly.</li>

 <li>Except for the main procedure, no other procedure should access variable names in .data directly. Only use data that are passed through the stack or register.</li>

</ul>




<strong>Testing</strong>

Test your result adequately: with valid and invalid input, with valid and invalid sum. Your program output should be the same as with assignment 5.