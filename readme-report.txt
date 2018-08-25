The arduino script inside "Updated_codes/my_Generator_control_Adafruit" folder is able to start the engine and run it with a setting to throttle from terminal. You just have to install one library: "AdafruitPWMDriver?" inside the arduino IDE.

Don't start the engine without tether or load!!!!!!

Next to do is to measure the current output and finish the feedback loop. My idea is to tie the current sum out of the batteries to 0 with a PID loop and believe in the magic. Dr. Brooke's idea is to do it heuristically: turn up the throttle little by little if the current out of batteries are positive and turn it down by a lot if the current ever go negative.

Go with his idea first. If it works, great; if not, just change the controller object in my script to use a different mechanism.
