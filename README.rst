GIT - Pre-Commit check for certain words
----------------------------------------

:Name: Douglas Mariz <douglasviviane@gmail.com>

About
-----
GIT pre-commit hook for checking the existence of certain words/phrases/functions 
in the code to be committed. 

How to install
--------------
To install hook, copy pre-commit file to your project .git/hooks/pre-commit:

    $ cp pre-commit .git/hooks/pre-commit;
    $ chmod +x .git/hooks/pre-commit;
    $ cp commit.msg .git/hooks/commit.msg;
    $ chmod + x .git/hooks/commit.msg;

The hook comes with the "die", "print_r" and "var_dump" functions as the strings to 
be checked prior to the commit. You can add more strings to be checked if you wish 
by modifying the checks array