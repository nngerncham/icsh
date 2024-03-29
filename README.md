In this README file, I'd like to share the references that I used for completing this project and the "good-to-know" things about my shell or problems I found along the way.

I'll go through this Milestone by Milestone.

--------------------------
GOOD-TO-KNOWS AND PROBLEMS
--------------------------
- Milestone5 
    - With my implementation, the shell IS made to have a pause after using redirection for accuracy issues
- Milestone6 
    - External commands CAN and WILL run in the background. However, it causes the shell to basically commit suicide after terminating/finishing.
        - Only happens if the terminated child is run in the background for some reason.
        - Somehow doesn't happen to foreground children, as far as I've tested.
    - jobs now works.
        - However, I couldn't figure out a way to delete terminated jobs or change the state of the process so it might always end up as "running".
    - fg doesn't work.
    - bg also doesn't work. 
    - Most of the codes for Milestone 6 are in jobcont.cpp and they look almost like psuedo codes.

---------
REFERENCE
---------
-- MILESTONE 1&2 --
- getting blank lines (for empty commands): https://www.geeksforgeeks.org/how-to-use-getline-in-c-when-there-are-black-lines-in-input/
- splitting strings (for how I implemented my echo): https://www.geeksforgeeks.org/how-to-split-a-string-in-cc-python-and-java/

-- MILESTONE 3 --
- converting a C++ string into a C string (char *): https://stackoverflow.com/questions/11821491/converting-string-to-cstring-in-c 
- turning a string into char ** (for execvp because I used strings): https://stackoverflow.com/questions/28712552/c-using-execvp-with-string-array/28713130

-- MILESTONE 4 -- 
- sending signals to the child process from a signal handler: https://stackoverflow.com/questions/13351851/killing-a-child-process-from-a-signal-handler
- talking with Justin where he shared his conversation with Aj.Sunsern
- talking with Aj.Sunsern

-- MILESTONE 5 --
- The program is designed to have a delay when redirecting.
- returning to using stdin and stdout after using dup2(): https://stackoverflow.com/questions/11042218/c-restore-stdout-to-terminal

-- MILESTONE 6 -- 

-- MILESTONE 7 -- 
- changing color of the terminal to look nicer: https://stackoverflow.com/questions/2616906/how-do-i-output-coloured-text-to-a-linux-terminal
- getting the username of a user: https://gist.github.com/krishna0512/5e5f8761a24ea850f0bd

Me after finishing this project: <br />
![froggo](../assets/frogjump.gif?raw=true)