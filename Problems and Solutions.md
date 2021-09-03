# HelloGitHub

Here I will be listing all the errors and problems I got through in my journey at mastering Git and Github:

                                    BECAUSE WITHOUT ERRORS, PROBLEMS, OBSTACLES ; ONE CANNOT LEARN, RETAIN, MASTER ANYTHING.
                                    SO YOU HAVE TO INDENTIFY PROBLEMS, FIND ITS SOLUTION, GET EXPERIENCE AND MASTER ANYTHING
 
 1) Prob 1: bash: cd: too many arguments
    
    Explain 1: 
              
               So, this type of problem comes when you have to cd to a dir with name having space in it.    
               So to locate to this type of dir we have to tell to the terminal the {firstname lastname} is not two dir s 
               since having space in between two texts make it understand that they are two different strings(here directories)
               so since two directories cannot be opened at once. It shows an error showing a message that 
               bash: cd: too many arguments
        
    Solution 1: 
                
                So we have to make the terminal understand that where we are locating is not two strings(dirs)
                So we have to specify the that it is one dir, which can be done by using single qoutes, double qoutes,
                or using \before the space.
                eg. cd 'first last' OR cd "first last" OR cd first/ last (see \ is before space)
                
                
 2) Prob 2: Made my local dir(folder) that too root directory a repository
    
    Explain 2:
               
               So after watching my first Git and Github tutorial ( Course ) he just showed me working on repository and Git directly.
               Now since I was a beginner and that too without any knowledge of terminal whether it be command prompt, Gitbash, Ubuntu etc.
               The course was just only about Git and Github (that too basic level) regardless of the fact that the tutorial was great and
               covered major commands. But it was made keeping in mind that the viewer knows about basic terminals and their basic commands.
               .
               And there I get to know about git init command. So I used it on my 4 dir s (including one being root directory).
               Now since i was practicing I felt that this course was not enough for me to master Git and Github.
               And I choose to enrol in a Udemy Course to master Git and Github. This course made me understand the basics, terminals, Git
               , Github, differences between Git and Github. what are directories, repositories, difference between dir and repos
               There I got to know that git init is used to convert a dir into repo. 
               ,
               Also the educator taught me that we SHOULD NOT USE git init command so easily. Since it can be disastrous if a root dir
               is made to a repo. 
               Then a thought came to my mind that I had been playing with the git init command.
        
     Solution 2: So the solution is in 4 Steps.
     
                  Step1 : Identify all your repositories in your machine.
                          This can be done using " find / -name ".git" which is find command
                          .
                          Now here all the .git files with "permission denied" message are the default repositories of the machine
                          which you DO NOT NEED TO TOUCH
                          Only the .git files which do not have that message are the ones you have made so there you can find the dir
                          you have mistakenly converted to a repository.
                  
     ![Example of repos](https://user-images.githubusercontent.com/24730417/131468051-6966a5b6-10d3-4072-85d0-75b150276446.png)
                 
                  Step2 : Locate to that dir
                     
                  Step3 : Check if you have corrected landed on your dir by using git status command. since only repos would identify 
                          it as a command.
                                           
                  Step4 : Remove the .git 
                          only .git (which is hidden) in a dir can make it a repo. So removing it will make it undo that mistake of making it repo
                          You can do it by
                                rm -rf .git
                          Then again check by git status command and it will not identify that command
               
               
             
            
        
