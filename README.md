# password-crack-link

basically
hi
SECRET_PIN = "583"  // The value we are trying to find

// The outer loop represents the first digit (Hundreds place)
FOR digit_1 FROM 0 TO 9:
    // The second loop represents the second digit (Tens place)
    FOR digit_2 FROM 0 TO 9:
        // The inner loop represents the third digit (Ones place)
        FOR digit_3 FROM 0 TO 9:

            // 1. Combine the digits into a "guess" string (e.g., "5", "8", "3" -> "583")
            CURRENT_GUESS = Convert_To_String(digit_1, digit_2, digit_3)

            // 2. Check the guess
            IF CURRENT_GUESS IS EQUAL TO SECRET_PIN:
                PRINT "Found PIN:", CURRENT_GUESS
                STOP THE ENTIRE PROCESS
            
            // OPTIONAL: Print the guess to show the progress
            // PRINT "Trying:", CURRENT_GUESS
