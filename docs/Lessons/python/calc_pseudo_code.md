## Tkinter Calculator Pseudo Code

Variables I think I need:
  
  * Current_value - what's currently in the entry box
  * Current-sub-total - result of whatever I've done up to now.
  * Current Operation - adding, subtract, multiply, divide
  
Initialize:

  * Put a zero in the entry box and current sub total and current value
  * Set current operation to Addition
  

Event Loop:

  * If a number is clicked:
      * Becomes the right most digit of entry_box and current_value
  * If + is clicked
      * add current-value to current-sub-total
      * clear entry box and set current-value to 0
      * set current-operation to addition
  * If = is clicked 
      * if current-operation is addition
          * add current-value to current-sub-total
          * display current-sub-total#tagcheck
#tagcheck
