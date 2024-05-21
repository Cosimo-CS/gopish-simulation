# GoPhish Simulation

## About this repository

This repository contains resources and configurations for a phishing simulation project created using GoPhish, designed specifically for educational purposes within the context of a cybersecurity training program. The goal of this project is to help students and professionals understand the mechanics of phishing attacks and develop skills to defend against them.

**Disclaimer:** This project is intended solely for educational use. It is strictly prohibited to use any of the materials or information provided in this repository for illegal or unethical activities. The author disclaims any responsibility for misuse of the content provided herein. By using this repository, you agree to comply with all applicable laws and regulations regarding cybersecurity and ethical conduct.


-----------------------------------------------------------------------

## Learning objectives

- Understanding how phishing works.
- Creating 2 e-mails and link them to allow 2FA.
- Downloading, installing and configuration of GoPhish.


## Mail creation

For this simulation I first tried to do it via Gmail but due to google's restrictions I wasn't able to validate my email sending tests. So I ‘got around’ the problem and chose to do it via outlook because outlook's SMTP allows mail to be sent via GoPhish.

### **1.** Outlook Mail creation

Let's start with the basics and create an email on the outlook site. Right [here](https://signup.live.com/signup?cobrandid=ab0455a0-8d03-46b9-b18b-df2f57b9e44c&id=292841&contextid=1CC4B350E7BE96A8&opid=3F232567E0CF3455&bk=1715950893&sru=https://login.live.com/login.srf%3fcobrandid%3dab0455a0-8d03-46b9-b18b-df2f57b9e44c%26id%3d292841%26cobrandid%3dab0455a0-8d03-46b9-b18b-df2f57b9e44c%26id%3d292841%26contextid%3d1CC4B350E7BE96A8%26opid%3d3F232567E0CF3455%26mkt%3dFR-BE%26lc%3d2060%26bk%3d1715950893%26uaid%3d6dca15265d26498e90412654e5a08821&uiflavor=web&lic=1&mkt=FR-BE&lc=2060&uaid=6dca15265d26498e90412654e5a08821)

Of course, in a real case, the ill-intentioned person will try to create an e-mail that is as authentic as possible in relation to the subject of the e-mail and the groups of people targeted. (ex: support@facebook[.]com)

After that you can directly create another e-mail.  We will use it to allow the 2FA access which will give us access to the password applications feature to make GoPhish working.

### **2.** 2FA 

Once your 2 emails have been created, go to your mailbox and, in the top right-hand corner, click on the initials of the account and then click to my microsoft account. Then go to the security tab, insert your credentials (safety first :-) )


![alt text](/img/2FA-1.png)

![alt text](/img/2FA-2.png)

You will fall into this page and you can click on "Manage the way that I log in"

![alt text](/img/2FA-3.png)

You will enter into a new page and there you can allow the 2FA. In this simulation, I've chosen to link the 2 email addresses I've created and to link another backup address with one of my colleagues, just in case the 2 email addresses ask for a confirmation code when you connect (which would be annoying because you'd block yourself ;-) ).

### **3.** Password application

Once you have activated the 2FA on the same page where you made it, the ‘Application password’ option will appear, but before creating it we will first install GoPhish.

![alt text](/img/2FA-4.png)

To summarise, we have created 2 email addresses, each with dual authentication enabled. Let's move on to the next step!

## GoPhish part

### **1.** Download and installation.

We're now going to install GoPhish on the PC.

[Here](https://getgophish.com/) is the official link where you can download it (depending on your OS)

After downloading it, you can choose where you want to place it in your pc and you dezip the file.

You can go into the unzipped file and look for the .exe file.

![alt text](/img/gophish-exe.png)

The first time you launch it, it is normal for Windows security to signal that it is not a reliable program. You can trust it and then a terminal will appear giving you the information you need to connect to your GoPhish portal.

- In blue: URL to have access to the portal
- In red: User + Password

![alt text](/img/Gophish.png)

### **2.** GoPhish setup

Keep the terminal open and go to your browser and inster the following address: https://127.0.0.1:3333 to have access to your portal.

Use the credentials that they gave you. In this case it's:

- Username: admin
- Password: 33edc65b82cae77a

![alt text](/img/gophish-welcome.png)

After entering the credentials you can directly update your password and put a stronger one.

![alt text](/img/dashboard.png)

### **3.** Sending profiles setup

### **4.** Landing Pages setup

### **5.** Email Templates setup

### **6.** Users and Groups setup

### **7.** Campaigns setup

## Final test
