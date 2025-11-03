# Python Keylogger Project

## Objective

The Python Keylogger Project is an ethical simulation designed to explore Python scripting, automation, and network protocol handling. The project creates a convincing fake command prompt interface that reads your computer's components, displays fake trees, ipconfig information, and files to simulate an ordinary CMD prompt. By taking advantage of threading, the keylogger is immediately able to record keystrokes to ensure logging begins as soon as the executable launches. The program reads the log file contents nested within a folder not typically visited, and emails them periodically to a portfolio Gmail account using SMTP over port 587. Emails are sent every 3 to 7 seconds to mimic sporadic behavior and reduce detectability.

A built-in termination key (Right Control) allows the program to be fully stopped at any time. A separate disclaimer window is displayed at the very beginning to alert the user of this programs deceptive nature, and provides the step for terminating the hidden purpose of this program.

### Skills Learned

* Python scripting and automation  
* Network protocol handling  
* Stealthy logging and periodic email transmission  
* Ethical considerations in cybersecurity tool development  

### Tools Used

* Python programming language  
* SMTP protocol for email transmission  
* Threading for concurrent keystroke logging  
* Fake command prompt interface for user deception  

## Showcase
### User Experience
Upon starting up the executable, we are presented with two windows;
- Disclaimer window revealing the hidden functionality of this program
- Fake driver update to increase deception<br/><br/>
<img width="606" height="437" alt="disclaimer" src="https://github.com/user-attachments/assets/7e522b05-ddf6-472d-a4f2-6ea0dd918783" />
<img width="602" height="434" alt="fake_update_with_abort" src="https://github.com/user-attachments/assets/d874a0f5-255e-4a27-9724-f86256282779" /><br/>
<sup> Please note only the PC components are accurate; the rest is usually uncommon knowledge to the average person. It's supposed to look real.</sup><br/><br/>

In the background, the keylogger is immediately started silently utilizing threading. Host and network information are pulled first, and logged to a file in a location that is not often checked on their local machine. Then, each time a user presses a key, the name and timestamp of the key pressed is recorded and appended to the file.=
<img width="1317" height="1365" alt="keylogging_file" src="https://github.com/user-attachments/assets/7f331fb9-09c2-4fc0-af95-d798866c0dc3" /><br/><br/>


A periodic email sender function reads the log file and transmits its contents to my portfolio Gmail account. To mimic sporadic behavior and reduce detectability, emails are sent every 3 to 7 seconds.

<img width="1050" height="1128" alt="periodic_email" src="https://github.com/user-attachments/assets/bc8d6376-fa21-4d43-9ea5-1ecdbcb0c68a" /><br/><br/>

### Source code
main function 

<img width="918" height="206" alt="main_py" src="https://github.com/user-attachments/assets/e405925e-203d-404f-8181-8ce7f704a115" /><br/><br/>

immediately start keylogging function in the background with threading

<img width="664" height="529" alt="keylogger_keystroke_listeners" src="https://github.com/user-attachments/assets/18ef26da-3e4b-4ab0-99a3-718af49a0391" /><br/><br/>

periodic email sender

<img width="1179" height="367" alt="periodic_email_sender" src="https://github.com/user-attachments/assets/41c889fc-79b2-4354-b4cf-7c45c116a665" /><br/><br/>

send email using smtp over port 587

<img width="567" height="394" alt="send_email_snippet" src="https://github.com/user-attachments/assets/7aec2d07-2053-4d39-86d2-50a410112384" /><br/><br/>

we can compile the project with this command line
- a
- b
- b

<img width="938" height="63" alt="command_line_create_exe" src="https://github.com/user-attachments/assets/1e0cfbd4-6632-4415-952b-bb883466dc45" /><br/><br/>

in turn, we can see the disclaimer mentioned above, 
