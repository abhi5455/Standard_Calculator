# Calculator

## A Calculator Made Using Java Swing Package

### Algorithm:

1. Create a class makeCalc that extends JFrame and implements ActionListener.

2. Declare instance variables:
   - String array str containing the calculator button labels.
   - JButton array b for calculator buttons.
   - JTextField instances jtxt1 and jtxt2 for displaying input and result.
   - double variables n, m, result for numeric calculations.
   - char variable op for storing the operator.
   - Deque<String> Q to store operands and operators. (Creating a DoubleEnded Queue)
   - int flag for tracking state.

3. Create a constructor makeCalc():
   a. Set up the JFrame with appropriate properties.
   b. Initialize and configure the JTextFields jtxt1 and jtxt2.
   c. Create and configure calculator buttons, adding them to the JFrame.
   d. Set the JFrame visible.

4. Implement the actionPerformed(ActionEvent e) method:
   a. Get the source button from the event.
   b. Extract the text from the button.
   c. Handle button actions based on the button text:
      - If "C" is pressed, clear the text fields and the Queue.
      - If "<" is pressed, remove the last character from both text fields.
      - If "=" is pressed:
         - Add the last operand to the Queue.
         - Evaluate the expression stored in the Queue and display the result.
      - If an operator button is pressed, add the current operand and operator to the Queue.
      - If a numeric button is pressed, update the text fields accordingly.

5. Implement the main method:
   a. Create an instance of the makeCalc class.

6. Run the program.

