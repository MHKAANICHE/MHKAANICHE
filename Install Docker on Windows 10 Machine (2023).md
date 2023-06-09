<h3>Blog: How to install Docker on windows 10 machine </h3>
<h4> May 27th 2023 </h4>


To install Docker on you Windows 10 machine, you would visit the official website [https://www.docker.com/](https://www.docker.com/)
and then download "Docker Desktop Installer" file (636.608 kb), start installation process ( that would freez your desktop for 90 min approxiamtevly ).

Then you will be asked to restart your machine (that will took much longer that expected, approximatevely 30 min ).
Happy at this point to see docker icone on your desktop, and by lunching the program, you will face an error message : 
 "wsl update x64 not supported by this processor".
 
 ![Install docker/Error message Windows 10.png](https://raw.githubusercontent.com/MHKAANICHE/MHKAANICHE/main/Install%20docker/Error%20message%20Windows%2010.PNG)
 
Frustrated you would google this error message and you find a github thred [https://github.com/microsoft/WSL/issues/8184](https://github.com/microsoft/WSL/issues/8184), where your dev peer 
are crying from pain to solve the same issue (same error posted for several processor configurations). 

Several solutions are proposed, but they seems insatable ( windows 10 would reconfigurate the kernel ) and you will end up losing time, passion and interest
in your path to enter the wonderful world of Dockerhub. 

I suggest the following process, that would save your time, by tackling the problem at it's root :  Docker is a Linux virtual environment (this our key).
So you would gently install Ubuntu on your windows 10 from WSL.
Run you Command prompt as administrator and enter the followin command : 
wsl --install -d Ubuntu

![Install docker/Ubuntu installation.png](https://raw.githubusercontent.com/MHKAANICHE/MHKAANICHE/main/Install%20docker/Ubuntu%20installation.PNG)

Once it's done you will be asked to create a user name ( regex condition - must be lowercase letter ) and then you will enter your password ( the cursor would not 
move, don't panic), once you confirm your password (again!) your installation will be accomplished.

![Install docker/install ubuto user.png](https://raw.githubusercontent.com/MHKAANICHE/MHKAANICHE/main/Install%20docker/install%20ubuto%20user.PNG)

Now you are running within a Windows Subsystem and your are a happy developer ( I hope !), you can pursue Docker installation on your subsystem by following the instruction for Linus installation. 
[https://docs.docker.com/engine/install/ubuntu/](https://docs.docker.com/engine/install/ubuntu/)

<h2>final take away :</h2> 
once your container is ready ( you can imagine that you are running a container of an image installed on virtual machine hosted on Windows subsystem ! ) Ouch !!!!  


