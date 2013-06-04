---
layout: post
title: "Command Line Basics"
date: 2013-06-04 00:07
comments: true
categories: 
---

Today I will write about the absolute basics I learnt some time ago, which I use without thinking about as well as some I always forget and hope to remember after writing about them here ;)

###Where are we and what do we have inside?

<pre><code>$ pwd</code></pre>
pwd = print working directory  
This shows the complete path from your root to the directory you are currently in. 

<pre><code>$ ls
</code></pre>
ls = list  
Will list all the files in your current directory. 

<pre><code>$ ls -l
</code></pre>
ls -l = list long  
Will show very detailed information about each file. Information I needed to care about so far were the rights the user had for this specific file. r (read), w (write), x (execute)

###Let's start moving
<pre><code>$ cd
</code></pre>
cd = change directory  
Definitely one of my favorite commands. I think it is so nice to cd and just move from one place to the other. :)  
If you only type <code>cd</code>, it will bring you to your home directory. 

For the next examples let's imagine you are in: /Users/username/workspace

<pre><code>$ cd ..
</code></pre>
Will get you to the previous directory.   
For example /Users/username/workspace -> /Users/username

<pre><code>$ cd fun_project
</code></pre>
/Users/username/workspace -> /Users/username/workspace/fun_project

<pre><code>$ cd fun <i> (then press tab)</i>
</code></pre>
This will autocomplete to: <code>cd fun_project</code>
You can press tab at anytime and it will autocomplete the name. If you have two projects starting with fun you can press tab two times and it will show you all the directories starting with fun. 

Last one with <code>cd</code>. You can go to any directory, it doesn't need to be related to the one you are currently working in. Some examples: 
<pre><code>$ cd ~ -> home
$ cd ~/Downloads 
$ cd ~/Desktop/fotos
</code></pre>

###Creating and moving files or directories

<pre><code>$ mkdir TESTFOLDER
</code></pre>
md = make directory  
This will create a new folder in the current directory with the name testfolder.

<pre><code>$ mv
</code></pre>
mv = move  
You can use this command to move a file or to simply rename it.

<pre><code>$ mv OLDNAME NEWNAME
</code></pre>
In this case you are simply renaming

<pre><code>$ mv FILE NEWDIRECTORY/
</code></pre>
In this case you are moving the file to the NEWDIRECTORY directory

<pre><code>$ mv FILE NEWDIRECTORY/fun.jpg
</code></pre>
In this case you are moving and renaming the file. (In this case a jpg)

<pre><code>$ cp
</code></pre>
cp = copy  
Copying works pretty much the same way as moving, the only difference is that you keep the original file at the original place. For example you download a picture and then copy it somewhere, the same picture will also stay in your Download folder.  
<u>Note:</u> If you want to move or copy directories you have to use additional commands

###Deleting
<pre><code>$ rm UGLYPIC.jpg
</code></pre>
rm = remove a file (jpg) called uglypic

<pre><code>$ rm -r USELESSFOLDER
</code></pre>
rm -r = remove a folder called uselessfolder including all the files inside. If you try only rm for a folder you will get the warning the this is a directory and you need to use the -r additionally. 

###Very useful commands to help you remember... something :)

<pre><code>$ man</code></pre>
man = manual  
This will open the manual for any command. For example <code>man ls</code> will show you how you can list files and which additional commands you can combine ls with.   
Once inside the manual you can navigate using the arrow keys and to leave this book of wisdom you obviously have to type <code>q</code>. 

<pre><code>$ history | grep SOMECOMMAND
</code></pre>
This will search your history of commands, when and how you used SOMECOMMAND  
So far we used <code>ls</code> several times. Try it out with <code>history | grep ls</code>

<u>Bonus:</u> tab  
Tab is awesome!  
For two reasons 1) It takes your typing away as you can use it to auto complete. 2) This way you also verify that what you are looking for really exists, if this makes sense ;)



