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
If the website doesn’t have protection (like account lockouts or CAPTCHA), the attacker might eventually guess your password and get in.



Each time, it fills in the login form just like a person would, but much faster — trying thousands of guesses in minutes.
