# mhz_cxf-c1f-Vulnhub-Walkthrough
mhz_cxf: c1f Vulnhub Walkthrough

**Description**
A piece of cake machine
You will learn a little about enumeration/local enumeration , steganography.
This machine tested on Virtualbox , so i'm not sure about it with Vmware
This works better with VirtualBox rather than VMware.

***Name: mhz_cxf: c1f***
***Date release: 24 Apr 2020***
***Author: mhz_cyber & Zamba***
***Series: mhz_cxf***

So let's begin hacking!!
**Step 1: Scan the machine**
> nmap -A -p- <IP_address_of_your_machine>

![Screenshot](1.png)

From the scan we can see that, port 22 and 80 are open. Let's explore port 80.

**Step 2: Go to machine's IP in web browser**
![Screenshot](2.png)

This doesn't help us much! Let's try bruteforcing the IP with dirb.

**Step 3: Bruteforce the IP with dirb**
> dirb http://<IP_address_of_your_machine> -X .txt

We are looking only for files containing .txt extension
![Screenshot](3.png)

From this step we got a file called notes.txt, let's take a look at the page.
>http://<IP_address_of_your_machine>/notes.txt

![Screenshot](4.png)



