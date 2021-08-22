# Assembly
code for MSP430 run with IAR.

    This project is an example for the diffrent use of the Timer in msp430g2553.h micro controller.
    for use it well you need to connect 1 and 2 PORT as describe:
        - P2.0 + P2.1 to pull-up button
        - P2.3 to pull-down button  (you can connect to a pull-up as well but then change the confoguration on the code)
        - P2.2 to an external scope
        - P2.4 to an external signal generator (PWM signal only)
        - make sure you connect the scope and the generator to the GRN in voltage 0v
        - P1 all pins to LCD screen 16x2
        - P2.5 + P2.6 + P2.7 to the LCD control pins, E + RS + R/W Respectively
    download in active aplication mode, and the program will demonstrat diffrent use of the Timer:
    after you press restart:
         - press P2.0 - the the msp will count up to 0xff if hex by at one-second intervals and show the current count on the LCD
         this function demonstrat the countinues mode of the timer
         - press P2.1 - the the msp will generate a PWM signal of 1 KHZ frequency and change the duty-cycle at 20% Cyclically
         this function demonstrat the output mode of the timer (generate signals)
         - press P2.1 - the the msp will read the frequency of the external signal generator (PWM signal only) and present the frequency
         of the external signal on the LCD screen
         this function demonstrat the capture mode of the timer (capture an external or internal PWM  signals)
        
      enjoy!
      for more info leave a comment.
        
