# IT 145 Final Project - Zoo AuthenticationSystem

Based on the stated problem statement and the data files provided for authentication and for the different profile roles, I have implemented the following procedure to develop the authorization system: 

1. Created a user-friendly option menu that allows the user the choice to log in with their credentials or log off to exit the program.  

2. Created an input line to prompt the user for a username.

3. Created an input line to prompt the user for a password.

4. Added the existing MD5 hash code to convert the password using a message digest five (MD5) hash.


# Pseudocode:

WHILE user input isn’t exit
    OBTAIN username
    OBTAIN password
    CONVERT password using message digest five (MD5) hash
    COMPARE password against the valid credentials in the credential file.
    IF unsuccessful attempt count < 3
           ADD 1 to unsuccessful attempt count
           PROMPT for password
    ELSE IF unsuccessful attempt count >= 3
           Quit program
ELSE
           CASE role OF
                Zookeeper      : Zookeeper file displayed
                Veterinary         : Veterinary file displayed
                Admin               : Admin file displayed
           ENDCASE
ENDWHILE

The pseudocode was a key element in the success of the zoo authentication system program. 
However, I had to extend the program significantly to ensure proper functionality.  
