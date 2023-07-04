0x06. Regular expression
========================

RegexDevOps

*    By: Sylvain Kalache
*    Weight: 1
*    Project will start Jul 4, 2023 6:00 AM, must end by Jul 5, 2023 6:00 AM
*    Checker was released at Jul 4, 2023 12:00 PM
*    An auto review will be launched at the deadline

### Concepts

_For this project, we expect you to look at this concept:_

*   [Regular Expression](https://intranet.alxswe.com/concepts/29)

Background Context
------------------

For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the `//`:

    sylvain@ubuntu$ cat example.rb
    #!/usr/bin/env ruby
    puts ARGV[0].scan(/127.0.0.[0-9]/).join
    sylvain@ubuntu$
    sylvain@ubuntu$ ./example.rb 127.0.0.2
    127.0.0.2
    sylvain@ubuntu$ ./example.rb 127.0.0.1
    127.0.0.1
    sylvain@ubuntu$ ./example.rb 127.0.0.a
    

Resources
---------

**Read or watch**:

*   [Regular expressions - basics](https://intranet.alxswe.com/rltoken/6VeaVMaugIxcFAwA27TBdQ "Regular expressions - basics")
*   [Regular expressions - advanced](https://intranet.alxswe.com/rltoken/rntjh3-3S86zt0Qy28L10w "Regular expressions - advanced")
*   [Rubular is your best friend](https://intranet.alxswe.com/rltoken/RGkVuw1lZ_hoCCbLsiOAhg "Rubular is your best friend")
*   [Use a regular expression against a problem: now you have 2 problems](https://intranet.alxswe.com/rltoken/Vwm8lpMUGa4x_FBtlyUQ8g "Use a regular expression against a problem: now you have 2 problems")
*   [Learn Regular Expressions with simple, interactive exercises](https://intranet.alxswe.com/rltoken/XsQ6rzS1uy-E6bnswUqIKg "Learn Regular Expressions with simple, interactive exercises")

Requirements
------------

### General

*   Allowed editors: `vi`, `vim`, `emacs`
*   All your files will be interpreted on Ubuntu 20.04 LTS
*   All your files should end with a new line
*   A `README.md` file, at the root of the folder of the project, is mandatory
*   All your Bash script files must be executable
*   The first line of all your Bash scripts should be exactly `#!/usr/bin/env ruby`
*   All your regex must be built for the Oniguruma library

### Quiz questions

**Great!** You've completed the quiz successfully! Keep going! (Show quiz)

Tasks
-----

### 0\. Simply matching School

mandatory

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/ec65557f0da1fbfbff6659413885e4d4822f5b1d.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230704T192620Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e76eb3ca6467e2755ac3c9917591dbb39a90f977a3e6fa542c4c3d316b8b6347)

Requirements:

*   The regular expression must match `School`
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method

Example:

    sylvain@ubuntu$ ./0-simply_match_school.rb School | cat -e
    School$
    sylvain@ubuntu$ ./0-simply_match_school.rb "Best School" | cat -e
    School$
    sylvain@ubuntu$ ./0-simply_match_school.rb "School Best School" | cat -e
    SchoolSchool$
    sylvain@ubuntu$ ./0-simply_match_school.rb "Grace Hopper" | cat -e
    $
    

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `0-simply_match_school.rb`

 Done? Help Check your code Get a sandbox

### 1\. Repetition Token #0

mandatory

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/e7db3c377d46453588fc84f3a975661d142fee91.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230704T192620Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=190902fcf16b936206a95ba657dfad87b3058e71474baec0844a40b7d522483b)

Requirements:

*   Find the regular expression that will match the above cases
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `1-repetition_token_0.rb`

 Done? Help Check your code Get a sandbox

### 2\. Repetition Token #1

mandatory

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/c59ff11db195d5cf17d1790a5141ae2f234786d2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230704T192620Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=992deb8fcbc9e966e25684732cc06820063986e9a74a502de434169e5afaaf48)

Requirements:

*   Find the regular expression that will match the above cases
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `2-repetition_token_1.rb`

 Done? Help Check your code Get a sandbox

### 3\. Repetition Token #2

mandatory

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/3b6bf4aeca6a0c2de584e7f5d68d11eef57ce205.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230704T192620Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=336f1c826e5dd2538fc72a2d16b0198836c467635ceb5916c58d51fc6e1638c4)

Requirements:

*   Find the regular expression that will match the above cases
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `3-repetition_token_2.rb`

 Done? Help Check your code Get a sandbox

### 4\. Repetition Token #3

mandatory

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/f8dbcb9cf5ae569a8645027dc46e81cb372ce28e.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230704T192620Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8e93f3fc0c6131d06852d97bf9635174cfb7099cd1de42e25fa6eb4d4c2b222c)

Requirements:

*   Find the regular expression that will match the above cases
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method
*   Your regex should not contain square brackets

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `4-repetition_token_3.rb`

 Done? Help Check your code Get a sandbox

### 5\. Not quite HBTN yet

mandatory

Requirements:

*   The regular expression must be exactly matching a string that starts with `h` ends with `n` and can have any single character in between
*   Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method

Example:

    sylvain@ubuntu$ ./5-beginning_and_end.rb 'hn' | cat -e
    $
    sylvain@ubuntu$ ./5-beginning_and_end.rb 'hbn' | cat -e
    hbn$
    sylvain@ubuntu$ ./5-beginning_and_end.rb 'hbtn' | cat -e
    $
    sylvain@ubuntu$ ./5-beginning_and_end.rb 'h8n' | cat -e
    h8n$
    sylvain@ubuntu$
    $
    

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `5-beginning_and_end.rb`

 Done? Help Check your code Get a sandbox

### 6\. Call me maybe

mandatory

This task is brought to you by a professional advisor [Neha Jain](https://intranet.alxswe.com/rltoken/GqwvXAvTXR_JXqyTvZ4AzQ "Neha Jain"), Senior Software Engineer at LinkedIn.

Requirement:

*   The regular expression must match a 10 digit phone number

Example:

    sylvain@ubuntu$ ./6-phone_number.rb 4155049898 | cat -e
    4155049898$
    sylvain@ubuntu$ ./6-phone_number.rb " 4155049898" | cat -e
    $
    sylvain@ubuntu$ ./6-phone_number.rb "415 504 9898" | cat -e
    $
    sylvain@ubuntu$ ./6-phone_number.rb "415-504-9898" | cat -e
    $
    sylvain@ubuntu$
    

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `6-phone_number.rb`

 Done? Help Check your code Get a sandbox

### 7\. OMG WHY ARE YOU SHOUTING?

mandatory

![](https://intranet.alxswe.com/images/contents/sysadmin/projects/78/shouting.jpg)

Requirement:

*   The regular expression must be only matching: capital letters

Example:

    sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb "I realLy hOpe VancouvEr posseSs Yummy Soft vAnilla Dupper Mint Ice Nutella cream" | cat -e
    ILOVESYSADMIN$
    sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb "WHAT do you SAY?" | cat -e
    WHATSAY$
    sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb "cannot read you" | cat -e
    $
    sylvain@ubuntu$
    

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `7-OMG_WHY_ARE_YOU_SHOUTING.rb`

 Done? Help Check your code Get a sandbox

### 8\. Textme

#advanced

This exercise was prepared for you by [Guillaume Plessis](https://intranet.alxswe.com/rltoken/2Rwwb9pSGKXSp3b3BcqkAw "Guillaume Plessis"), VP of Infrastructure at TextMe. It is something he uses daily. You can thank Guillaume for his project [on Twitter](https://intranet.alxswe.com/rltoken/Vz-iLl3_Of797s9TsjCxJQ "on Twitter").

For this task, you’ll be taking over Guillaume’s responsibilities: one afternoon, a TextMe VoIP Engineer comes to you and explains she wants to run some statistics on the TextMe app text messages transactions.

Requirements:

*   Your script should output: `[SENDER],[RECEIVER],[FLAGS]`
    *   The sender phone number or name (including country code if present)
    *   The receiver phone number or name (including country code if present)
    *   The flags that were used

You can find a [\[log file here\]](http://intranet-projects-files.s3.amazonaws.com/holbertonschool-sysadmin_devops/78/text_messages.log).

Example:

    $ ./100-textme.rb 'Feb 1 11:00:00 ip-10-0-0-11 mdr: 2016-02-01 11:00:00 Receive SMS [SMSC:SYBASE1] [SVC:] [ACT:] [BINF:] [FID:] [from:Google] [to:+16474951758] [flags:-1:0:-1:0:-1] [msg:127:This planet has - or rather had - a problem, which was this: most of the people on it were unhappy for pretty much of the time.] [udh:0:]'
    Google,+16474951758,-1:0:-1:0:-1
    $
    $
    $ ./100-textme.rb 'Feb 1 11:00:00 ip-10-0-64-10 mdr: 2016-02-01 11:00:00 Receive SMS [SMSC:SYBASE2] [SVC:] [ACT:] [BINF:] [FID:] [from:+17272713208] [to:+19172319348] [flags:-1:0:-1:0:-1] [msg:136:Orbiting this at a distance of roughly ninety-two million miles is an utterly insignificant little blue green planet whose ape-descended] [udh:0:]'
    +17272713208,+19172319348,-1:0:-1:0:-1
    $
    $ ./100-textme.rb 'Feb 1 11:00:00 ip-10-0-64-11 mdr: 2016-02-01 11:00:00 Sent SMS [SMSC:SYBASE1] [SVC:backendtextme] [ACT:] [BINF:] [FID:] [from:18572406905] [to:14022180266] [flags:-1:0:-1:-1:-1] [msg:136:Far out in the uncharted backwaters of the unfashionable end of the western spiral arm of the Galaxy lies a small unregarded yellow sun.] [udh:0:]'
    18572406905,14022180266,-1:0:-1:-1:-1
    $
    $
    $ ./100-textme.rb 'Feb 1 11:00:00 ip-10-0-64-11 mdr: 2016-02-01 11:00:00 Sent SMS [SMSC:SYBASE1] [SVC:backendtextme] [ACT:] [BINF:] [FID:] [from:12392190384] [to:19148265919] [flags:-1:0:-1:-1:-1] [msg:99:life forms are so amazingly primitive that they still think digital watches are a pretty neat idea.] [udh:0:]'
    12392190384,19148265919,-1:0:-1:-1:-1
    $
    
    

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x06-regular_expressions`
*   File: `100-textme.rb`

 Done? Help Check your code Get a sandbox

