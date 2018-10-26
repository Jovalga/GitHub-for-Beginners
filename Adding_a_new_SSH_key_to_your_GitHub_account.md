# Adding a new SSH key to your GitHub account

**Steps**

1.- Generate a key in the terminal.
	
	ssh-keygen
	Generating public/private rsa key pair.
	Enter file in which to save the key (/home/alvaro/.ssh/id_rsa): /home/alvaro/Escritorio
	/home/alvaro/Escritorio already exists.
	Overwrite (y/n)? y
	Enter passphrase (empty for no passphrase): 
	Enter same passphrase again: 




2.- Now we going to the path

	alvaro@DoctorPlutonio:~$ cd ~
	alvaro@DoctorPlutonio:~$ cd .ssh
	alvaro@DoctorPlutonio:~/.ssh$ ls
	id_rsa  id_rsa.pub  known_hosts
	alvaro@DoctorPlutonio:~/.ssh$ 
	cat id_rsa.pub


3.- We copy the key 

	We go to the settings of the git page
	Search SSH and GPG keys
	we go to the New SSH key button
	and copy the key in the box key
	Press Add SSH key button


