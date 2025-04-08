# Brute-force-attacks-lab-

To better understand how cyber threats target passwords in applications or systems, I completed a hands-on challenge focused on detecting brute force attacks. This exercise helped me recognize patterns of repeated login attempts and learn how attackers try to break into systems by guessing credentials. It gave me a clearer understanding of how to protect user accounts and why strong password security matters in real-world environments.

### Skills Learned 
- Brute Force Attack Detection- Gained experience identifying repeated failed login attempts across logs and understanding how attackers systematically guess passwords.
-Security Log Analysis- Learned to analyze and interpret authentication logs to detect unusual patterns that indicate malicious behavior.
- Account Lockout Policy Awareness- Learned the importance of configuring lockout thresholds to help prevent unauthorized access attempts.


### How does Brute Force Attacks Work
A brute force attack is when someone tries to break into an account by guessing the password over and over again until they get it right. Think of a brute force attack is like trying every key on a keyring until one finally opens a locked door.
For instance, people have a favorite website they sign into everyday. The login page usually looks like this:

**Reference: Login Page**
![ChatGPT Image Apr 5, 2025, 10_26_47 AM](https://github.com/user-attachments/assets/d18de5b6-c96f-45b1-b1e3-82cbbdf1cb41)

Now a brute force attacker finds this same page and doesn’t know your password . However, they use a computer program that automatically tries a huge list of common passwords — like 123456, qwerty, or letmein — over and over again.
The hacker is preying on users that dont utilile secure complexity passwords. 
If the website doesn’t have protection, the attacker might eventually guess your password and get in.


###Lets Defend lab : What is the IP address of the server targeted by the attacker's brute-force attack?

I will now walk through completing the brute force attack challenge. I utilized the tool wireshark to help me identify a web server that has been damaged. Essentially, Wireshark is like a security camera for network traffic. It lets you see what’s happening behind the scenes when computers talk to each other.

The challenge began with a security alert indicating possible brute force activity in RDP services. I was tasked with confirming whether it was an actual attack and gathering evidence. 

**reference: Wireshark Tool
![image](https://github.com/user-attachments/assets/7a9b45c1-8a0c-4b93-b5db-7f1ce6402b38)


**Statistics 

I opened the packet capture file and began analyzing the Remote desktop protocol traffic. In the "Source" and "Destination" columns, I saw the source IP is 192.168.190.137 (this is the attacker). The destination IP is 51.116.96.181 — this is the system being attacked
This pattern repeats several times.
 **Reference: Source and Destination Column 
![image](https://github.com/user-attachments/assets/fdfdbd2e-d700-4187-8fd0-1920b4940c7a)

 Additionally, the timestamp column showed that the attacker is sending multiple connection requests very quickly, within milliseconds. One of the signs of common brute force attacks is rapidly trying logins.




