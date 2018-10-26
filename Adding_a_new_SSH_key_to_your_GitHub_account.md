# Adding a new SSH key to your GitHub account

**Steps**

1.- Generate a key in the terminal.
	
	$ ssh-keygen
	Generating public/private rsa key pair.
	Enter file in which to save the key (/home/alvaro/.ssh/id_rsa): /home/alvaro/Escritorio
	/home/alvaro/Escritorio already exists.
	Overwrite (y/n)? y
	Enter passphrase (empty for no passphrase): 
	Enter same passphrase again: 




2.- Now we'll go to the path:

	$ alvaro@DoctorPlutonio:~$ cd ~
	$ alvaro@DoctorPlutonio:~$ cd .ssh
	$ alvaro@DoctorPlutonio:~/.ssh$ ls
	id_rsa  id_rsa.pub  known_hosts
	$ alvaro@DoctorPlutonio:~/.ssh$ 
	cat id_rsa.pub


3.- We have to copy the key (the content inside id_rsa.pub): 

	- We go to the settings, in the GitHub web.
	- Search SSH and GPG keys.
	- We go to the New SSH key button and copy the key in the box.
	- Press Add SSH key button.


