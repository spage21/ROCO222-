# ROCO222 Lab Journal, 
Sam Page, Student num: 10528757
I worked in a pair with Alix Germany (shared most of the pictures)

# Lab 1, Learning to use Ubuntu and Git

# Basic Linux commands

**1- ls**
lists all files and folders in your current directory

**2- cd**
lets you change directory, got into other folders you can use "cd .." to go back a folder.

**3- mkdir** 
used to create a new folder or subfolder. "rmdir" will remove any empty directory

**4- sudo**
basically an override command. put sudo before something to force it.

**5-cp**
stands for copy and paste. first determine the file you want to copy and type the destination location to paste the file.

_$ cp (file name) (location you want to paste too)_

**6- rm**
remove. its a command used to delete your file or even your directory. you can use -f if the file needs root permission to be removed. 

_$ rm myfile.txt_

**7- apt-get**
this command is to install, remove and upgrade any package. apt advanced packaging tool. the 
apt-get command will help you install software. its a powerful command line which can perform installation, upgrade and even remove software.

_$ sudo apt-get update_

**8-grep**
if you need to find a file but cant remember its exact location or path grep will help you solve this problem.

_$ grep user /etc/password_

**9- cat**
it will show you text inside your file.

_$ cat Cmakelists.txt_

**10- poweroff**
sometimes you need to power off directly from the terminal this command will need a sudo before it to work.

_$ sudo poweroff_

**11- pwd** 
to know what directory youre in type pwd in the terminal

**12- df**
the df command is used to see the availble disk space in each of the partitions of your system in KB if you want to see it in mbs type "df -m"

**13- zip and unzip**
zip is a command used to compress files into a zip archive. unzip is used to extract files from a zip archive.


# What is Markdown ?

-Markdown is a way to style text on the web. you can control the display of the document. you can format the words as bold or italic, add images etc....Mostly markdown is just regular text with a few non-alphabetic characters like # and *. you can use markdown is most places around git hub, like gists comments in issues and pull requests and files with ".md" and ".markdown" extentions

using a single '#' all the words after it will become a heading

using two * before and after words makes them all bold

using one _ before and after words puts them in italics

using two ~ before and after words puts a line through them. (though I cant seem to get it to work)


# Notes on GitHub
saving markdown document using commits and github.
first open terminal and type  _git init_ then navigate into the directory using _Cd_ and _ls_ after making changes to a markdown document  write _git status_ and you can see the files that you have changed. to save these files type _git add_ then the file name. once youve added all the files you want to save type _git commit_ and an appropriate message then _ctrl X_ and _Y_ and then hit the enter key. After this is type _git log_ to check the commit has been made successfully.

# Lab 2, Building a DC motor.

Using the kit provided I began building a DC motor out of a cork, a couple of magnets, some copper tape and wire. The cork would act as a core for the DC motor and with two pins in each end it meant that it could spin pretty easily when supported between two paper clips. Next we added two pieces of copper tape to one end of the cork. these two surfaces would act as commutators for the motor. Then we would cut two pieces of multicore wire and use them as brushes. After screwing a couple of paper clips into the wooden base we used them to support 2 magnets on either side of the cork (our motor core). 

need pictures.

# Problems with the motor
- The motor we built ended up working but not very well. The brushes were pretty unreliable because they provided little contact against the commutator.
- We also had no supports for the wires making it difficult for the brushes to maintain contact with the communtator
- The cork used for the core of the motor was pretty small, which meant we could only get a small amount of copper wire around it. due to this reason we also couldnt add too many different coils of wire.
- We used the paperclips to support the magnets, this was pretty unstable and at times the magnets would get stuck to the core if it got to close.

# Improvements we made
We proceeded to think of some idea's to help improve the motors overall function

**Changes to the Core**

- We wanted to get a new core that would have a higher magnetic permability than cork, as in theory this would create a stronger magnetic field and make the motor spin better. Ideally we wanted to use something like Iron because of its high permability, however finding a suitable sized piece of iron became quite difficult so instead we used a small wooden rolling pin. Although the permability was probably around the same as the cork our new core was much larger. This meant we could get more coils of wire around it. The handles at the end also helped us support the motor.

**Changes to the Structure**

- Using the laser cutter we designed and cut out a new base and support structure out for card for our motor. we designed it all on solid works and measured it precisely. We designed it so that all the pieces of card slotted together, although we did re-enforce them with the glue gun.
- We made mounts for the 4 magnets because our core was quite long we seperated all 4 magnets so we would have a stronger field over the length of the core. The mounts were 4 pieces of card that we would press together. two piece of card had holes in where the magnet would sit. Each magnet was about as thick as two pieces of card. once we held the magnets in place we pressed all the pieces of card together and sealed them shut with some tape and bit of glue.
- At either end of the core we had a rectangular piece of card with a hole remove from the centre. we used this to support the rolling pin core. Using sand paper we had to sand down the ends of the rolling pin a little bit to get them to slot into the holes. The handles on the end of the rolling pin were wider at the edges then got thinner, this was good as we only sanded it down so that the widest part was just able to fit through the hole in the card. This hopefully means that the core wont come off very easily.
  
**Changes to the wire and coils**

- The supports we made to hold the magnets in place were tall enough that we could also use them to support the wires running to the brushes. instead of using multicore wire touching against some copper tape as our brush-commutator system we thought we could get a bigger contact surface area if we attached the wire directly too some more copper tape and use them as the brushes instead.
- 

# Lab 3,
to add the encoder into our motor design we printed off another piece of card about the same width and height as the two that supported each end of the motor core. We also printed off a small disc with a section removed from the edge. The first bigger piece we stuck onto the edge of the base near one end of the rolling pin. This would be where we would mount the encoder. A short distance infront of this piece of card was the end of the rolling pin we stuck the small disc onto the end of the rolling pin handle this meant that as the motor rotated so would the small disc. With the encoder mounted near by we could use it to accurately measure when the motor had done 1 rotation. 

# Lab 4, 
Controlling the DC motor, with motor shield and using arduino to program it.

# Lab 5,
Programming a stepper motor to function usuing
- **Full-step**,
The motor is operated with only one phase on at a time, this therefore uses the least amount of power
- **Double-step**,
The motor has 2 phases on at a time this provides better torque and speed peformance than full-step but uses twice the power. 
- **Half-step**,
Is a combination of Double-step and Full-step first just one phase will be on then a combination of two phases will be on then just one again. This creates a smoother transition between steps.
- **Micro-step**,
Micro-stepping involves gradually increasing and decreasing the current across two of the coils so that the tranistion between steps is really smooth. This however reduces speed and torque quite a lot.


# Lab 6 and 7

**Designing and Building the robot arm**

first we set up the servos by attaching them to pieces of cardboard. We used the 'mapping' function in arduino to control the movement of the servo so that it was proportional to the value coming off of the potentialomete. Once we were happy with this we proceeded to move onto building our arm. In solid works we designed various pieces that would make up our arm which we aimed to export and 3D print. We designed the arm so that it would have 3 degrees of motion. This means there would be 1 servo at the base controlling with direction the arm would face. We positioned the second servo pretty much on the base too but this time it was on its side so that it would move the arm up and down at an angle. The third servo we positioned about half way up the arm which served almost like the elbow joint of a human arm. Giving us another degree of movement up and down. We left the plastic at the end of the arm a certain shape as we wished to slot different things into it but never got round to it. 
















