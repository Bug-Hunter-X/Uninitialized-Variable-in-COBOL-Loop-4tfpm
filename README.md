# Uninitialized Variable in COBOL Loop

This repository demonstrates a common error in COBOL programs: using uninitialized numeric variables. The `bug.cob` file shows code that calculates a total within a loop but fails to initialize the `WS-TOTAL` variable, leading to unpredictable results. The `bugSolution.cob` shows the corrected version.

## Bug Description
The provided COBOL code calculates a sum using a loop. However, the `WS-TOTAL` variable is not initialized before the loop starts.  This results in the program adding to a potentially random value, leading to incorrect results.

## Bug Solution
The solution involves explicitly initializing `WS-TOTAL` to 0 before starting the loop. This ensures that the summation starts from the correct value and yields accurate results.