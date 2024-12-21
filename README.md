# LSTM: Long Short-Term Memory

 Introduces gates (input, forget, and output) to manage information flow, solving the vanishing gradient problem.

![image](https://github.com/user-attachments/assets/82d5e89a-135a-421b-b894-82c9c7809d01)

Forget Gate: The forget gate decides which information from the previous cell state should be discarded. It takes the previous hidden state and the current input as input and outputs a value between 0 and 1 for each element in the cell state. A value of 1 means "keep this information," while a value of 0 means "forget this information."

Input Gate(Adding): This gate within the LSTM cell controls how much of the new information (from the current input) should be stored in the cell state.

Candidate Value(Update): This is a proposed update to the cell state.  It's calculated based on the current input and the previous hidden state.   
The candidate value represents the potential information that could be added to the cell state.  

Output Gate: Controls which information from the cell state is used to compute the current output.  

![image](https://github.com/user-attachments/assets/1b713834-bc1a-4224-8ed1-27e90e784ee3)

Mathematical Intuition

![image](https://github.com/user-attachments/assets/2b7ed4a7-26f8-4a0a-b306-265d370715da)


# Implementation

![image](https://github.com/user-attachments/assets/f403f64e-0aae-49e1-92ba-582cf534651c)

![image](https://github.com/user-attachments/assets/3923effe-f1bc-4d35-8ac6-898551f277ba)


