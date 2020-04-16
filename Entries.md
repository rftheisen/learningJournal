# Learning Goals for the rest of 2020
    1. Pass CEH by May 15th *Scheduled* 
    2. Pass OSCP by August 20th 
    3. Finish Cisco CCNA video series on YouTube by June 1st 
    4. Pass CCNP Enterprise Core by December 11th 
    5. Obtain my BSIT Degree by the end of Fall semester 



# Goal Accomplishment Strategy 
    1. Doing HacktheBox, Tryhackme challenges, reading Mike Walkers book, and completing Practical Ethical Hacking Course 
    2. Find funding to purchase, go through training course on Offensive Security's site, practice bash and powershell skills,
        and use platforms from first goal.
    3. Schedule time in the week to work on recording the content
    4. Complete CBTNuggets course, Read Cisco Press CCNP book, and setup GNS3 lab in VMware esxi and upgrade server memory
    5. Take summer courses and keep doing well in class

# Accomplished:

-  Build hyperconverged home lab by March 20th 
-  Build remote access lab functionality for classes by March 20th


## Setting up and testing Ubuntu Client in GNS3 with nested virtualization: 

- Must upload a VMDK file from client to server when creating the appliance 
    https://www.osboxes.org/ubuntu/#ubuntu-19-04-vmware
- Then you must specify the ISO that is going to be used to book the VM into Ubuntu
- GNS3 has tightvnc integrated for graphical terminal access to the OS
- When using ssh to connect to the router Ubuntu returns an error that indicates an older cipher suite is being used on the router, this prevents successful connection
- Trying telnet worked, we will comeback to the ssh
    https://www.openssh.com/legacy.html
- dsqst found that we needed to use a less secure cipther to connect via Ubuntu so we used this command: 

    ``` ssh -c aes128-cbc ltn@192.168.0.1 ```
- In the industry it would recommended that we upgrade the IOS image on the device to an images with up to date ciphers and methods with SSH 

## Setting up and testing Windows Server 2016 in GNS3: 
- The Windows Server appliance on GNS3s Marketplace does not work properly
- Must get .gns3a code from Github repo, and create your own file.Make sure to give it .gns3a extension
- Download qemu config file straight from appliance import screen
- Once all the file are uploaded make sure you turn on the device :p!
    - I spent far too much time trying to troubleshoot an error message when really I needed to just power the appliance on.


# Teaching Philosophy

For me this job is a calling where I get to help each of you better understand technology, how it fits in this world and how being good with it can increase your ability to help others as well as bring in some extra money in the process. Know that my focus is on empowering you however, it is important for you to know that the road to empowerment is riddled with unique challenges. Here are some of the major ways you can expect to be challenged:

## Accountability 
One of the hardest things to do in the process of learning is making the information meaningful. Think about it! What is the last thing you learned? How did that knowledge help you or someone else? Did it add to a conversation you had? Is it stored somewhere deep in your memory bank? Are you actually using it? 

As I guide and coach you through your learning process you will constantly be asked to share, present and demonstrate your knowledge. Over the years I've found this to work really well in cementing the knowledge in the minds of those who really want to learn. 

Grades are another accountability measure, some students are motivated by a grade as if it is a rank in their favorite video game. This focus can help but shouldn't be your only motivation for learning. I encourage you to learn outside of the bounds of receiving credit. If you are motivated primarily by grades why should you learn anything without receiving credit? I look forward to knowing your answer on this at some point.

Forgive me for this ahead of time but I will challenge your understanding of topics. Many have not been challenged in this way in any area of life and it shows in how they respond. Ill ask the class "Does everyone understand?" At first many nod their heads and keep their hands down fully believing they understand the topic. When I ask directly.... its another story. You want to make sure you understand! In IT you will be challenged on a regular basis and we want you to be able rise to the occasion. Leaders in IT will respect those who are honest and skilled at explaining what they are doing. Honestly, if you don't know why you are doing something you probably shouldn't be doing it. 

## Reflection through writing 
Writing is such an empowering activity and form of expression. When you write you are finalizing thoughts in their most current iteration. I'm not looking for grammatical perfection in your writing but I will be looking at your ability to convey a message, technical accuracy and impact. This will be done through learning journals that you will submit. Don't worry.... I am not asking you to write a dissertation here. 

## Learn-to-teach
If you can teach a topic, you know it! Assuming your teachings are correct of course. This semester each of you will have the opportunity to teach an important Computer Networking concept to the class. Why would I ask such a thing of you? Because I believe in you and the power of teaching as a great learning activity. You will grow in your ability to communicate technical & non-technical concepts through learn-to-teach activities. 

## Identifying major trends 
The ability to identify trends in IT is what makes you an outlier. It's why the industry often talks about the select few that defined and are defining it (Bill Gates, Steve Jobs, Richard Stallman, Linus Torvalds, Ralph Baer, Mark Zuckerberg, Jeff Bezos, Elon Musk, Ada Lovelace, etc...). These outliers had an uncanny ability to identify trends in technology and needs of the people. They all built something that people were going to value in some way and now those tools they built are the digital world we spend much of our time in. We will often have discussions about trends and needs in the world of which I am confident you will be able to meet. In a practical sense this class is built around technology someone else designed that we must now need to know how to use to be employable in the industry they created. 



I hope from reading all this you get somewhat of an idea about how I operate. You will learn even more about me as you come to class. More importantly this is about you growing as a learner, IT professional and member of society. It's going to be a great semester! 