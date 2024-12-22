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

LSTM:

![image](https://github.com/user-attachments/assets/3923effe-f1bc-4d35-8ac6-898551f277ba)


![image](https://github.com/user-attachments/assets/f7ee6c61-a4e8-4bbd-8560-6c77d1c85e5a)

# GRU- Gated Recurrent Units

GRU: Combines LSTM's gates into update and reset gates, simplifying the architecture.

![image](https://github.com/user-attachments/assets/d3cf79d3-ce82-4693-b81c-56e4a0fdbec9)

Reduced Complexity: LSTMs have two gates (forget and input) to control the flow of information. GRUs, on the other hand, have only two gates:

Reset Gate: Determines how much of the past information should be forgotten.   

Update Gate: Controls how much of the past information should be passed to the next time step.  

This simpler structure makes GRUs easier to train and computationally less expensive.   

Improved Performance: Despite their simpler architecture, GRUs have shown comparable or even better performance than LSTMs in many tasks, particularly in tasks with shorter sequences.

Vanishing Gradients: Like LSTMs, GRUs also help mitigate the vanishing gradient problem, allowing them to capture long-range dependencies in sequential data.

GRU: Comparable to LSTM but faster and smaller in size.

![image](https://github.com/user-attachments/assets/d3d82ca5-edfa-45b4-9c06-2f865ddfd7c7)


![image](https://github.com/user-attachments/assets/114af05f-416f-415d-8e12-0d99f9fc04df)

# Implementation


![image](https://github.com/user-attachments/assets/66b84122-d4df-471c-8fba-77cf33b9d471)


