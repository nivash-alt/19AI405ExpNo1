<h1>ExpNo 1 :Developing AI Agent with PEAS Description</h1>
<h3>Name: Nivash P</h3>
<h3>Register Number/Staff Id: 212225230203</h3>


<h3>AIM:</h3>
<br>
<p>To find the PEAS description for the given AI problem and develop an AI agent.</p>
<br>
<h3>Theory</h3>
<h3>Spam Mail detection system:</h3>
<p>PEAS is a framework used in Artificial Intelligence to describe the components of an intelligent agent. It helps define how an AI system interacts with its environment to achieve its goals.
PEAS stands for:
P – Performance Measure: Defines how the success of the AI agent is evaluated. 
E – Environment: The surroundings in which the AI agent operates. 
A – Actuators: The devices or mechanisms used by the agent to perform actions. 
S – Sensors: The devices used to collect information from the environment. 
The PEAS model is widely used in designing intelligent systems such as robots, self-driving cars, virtual assistants, medical diagnosis systems, and game-playing agents.</p>
<hr>
<h3>PEAS DESCRIPTION:</h3>
<table>
  <tr>
    <td><strong>Agent Type</strong></td>
    <td><strong>Performance</strong></td>
     <td><strong>Environment</strong></td>
    <td><strong>Actuators</strong></td>
    <td><strong>Sensors</strong></td>
  </tr>
    <tr>
    <td><strong>Spam Mail Detection System</strong></td>
    <td><strong>Accurately detect spam emails and reduce false predictions.</strong></td>
     <td><strong>Email Inbox</strong></td>
    <td><strong>Move spam emails to the Spam folder or delete them.</strong></td>
    <td><strong>Incoming emails, sender details, email content.</strong></td>
  </tr>
</table>
<hr>
<H3>DESIGN STEPS</H3>
STEP 1: Identifying the Input:                                                                                  
Email content, sender information, subject, attachments, and keywords.                                                                                                                       
                                                                                                                  
STEP 2: Identifying the Output:                                                               
Classify the email as Spam or Not Spam (Ham).                                                   
                                                                                                              
STEP 3: Developing the PEAS Description:                                                                
PEAS description is developed based on the Performance Measure, Environment, Actuators, and Sensors of the AI agent.                                       
                                                                                                                      
STEP 4: Implementing the AI Agent:                                                                                                         
Analyze the incoming email using a Machine Learning model, detect spam patterns, and automatically move spam emails to the Spam folder while allowing genuine emails into the Inbox.                                       

STEP 5: Measuring the Performance Parameters:                                                                                     
For every correctly classified email, the performance is incremented. For every wrongly classified email (false positive or false negative), the performance is decremented. The system performance is evaluated using Accuracy, Precision, Recall, and F1-Score.                                             
Python Implementation:
```
import random
emails = {
    "Email 1": random.choice(["Spam", "Not Spam"]),
    "Email 2": random.choice(["Spam", "Not Spam"])
}
performance = 0
print("Initial Emails")
for email, status in emails.items():
    print(f"{email}: {status}")
print("\nSpam Mail Detection Agent Started...\n")
for email in emails:
    print(f"Agent checking {email}")
    performance -= 1      # Checking cost
    if emails[email] == "Spam":
        print("Sensor: Spam email detected.")
        print("Action: Moving email to Spam folder...")
        performance += 10
        print("Email moved successfully.")
    else:
        print("Sensor: Genuine email detected.")
        print("Action: Keeping email in Inbox.")
        performance += 5
    print(f"Current Performance: {performance}\n")
print("Final Email Status")
for email, status in emails.items():
    print(f"{email}: {status}")
print("\nFinal Performance:", performance)
```
Output:

<img width="443" height="697" alt="Screenshot 2026-07-25 093157" src="https://github.com/user-attachments/assets/9a7fc0a6-0963-490b-a92c-c253a3f73a7d" />
Result:
The PEAS description implementation is Successful
