Voting System Readme

Overview

This is a simple console-based voting system implemented in C. The system supports the authentication of users, both administrators and students, and allows them to participate in or manage elections. The code is organized into functions, providing modularity and ease of understanding.

Features

1. Admin Panel:
   - Authentication: The admin needs to enter a username ("Admin") and a password ("admiN") to access the admin panel.
   - New Election Initiation: The admin can initiate a new election by providing details such as the year, branch code, total voters, and the number of candidates.
   - Continue Previous Election: The admin can load the details of a previous election from a file.
   - Delete Illegal Vote: The admin can delete a vote by entering the user ID associated with the vote.
   - Ban User IDs: The admin can ban specific user IDs, preventing them from voting in the current election.
   - Result: The admin can view the election results, including the winner and the voting percentages.

2. Student Panel:
   - Authentication: Students need to enter a valid user ID to participate in the election.
   - Validity Check: The system checks the validity of the user ID based on the election parameters.
   - Ban Check: It verifies whether the student's ID is banned or not.
   - Duplicate Vote Check: It ensures that a student can vote only once.
   - Voting Process: Students can cast their votes by selecting a candidate from the list.
   - Exit Option: Students can exit the voting process by entering "0" as the user ID.

3. Election Information:
   - Election details such as the year, branch code, total voters, and the number of candidates are stored in files.
   - Candidate information and voting records are also saved in separate files.

4. Result Calculation:
   - The system calculates and displays the election results, including the winner and voting percentages.

usage:

1. Admin:
   - Run the program.
   - Enter the admin username ("Admin") and password ("admiN").
   - Choose options from the admin panel menu to manage elections.

2. Student:
   - Run the program.
   - Enter a valid user ID to participate in the election.
   - Follow the instructions to cast a vote for a candidate.

File Management

- ElectionInfo.txt: Stores information about the current election, including the year, branch code, total voters, and the number of candidates.
- candidateX.txt: Files for each candidate (X represents the candidate number) storing the candidate's vote count and the roll numbers of students who voted for them.
- Banned.txt: Contains the roll numbers of banned users.
