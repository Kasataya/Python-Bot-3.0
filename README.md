# Python-Bot-3.0
#1      #                   Creating text file(s)

        #   1. every time a user inputs his first and last name a text file is created with the title (First_Last.text)

user_first = input("Enter your first name: ")
user_last = input("Enter your Last name: ")
file_name = user_first + user_last + '.txt'

        #   2. file is outomatically added to the folder within the code
        
file = open(file_name, 'wt') # with 'wt' access mode if file already exists with the same name, than the creation of that file will be denied


#2      #                   text file information

        #   1. add different input statements within the text file created
user_adress = input("What U.S state do you currently reside in: ")
user_school = input("What school or university do you currently attend: ")
user_major = input("What mojor are you pursueing in college or hope to pursue after school: ")


file.write(" Hello, I am " + user_first + ' ' + user_last + '.')
file.close()



# After step 1 & 2 have been delt with, we currently have a code that creates different text files regarding each user

#3      #                   Folder organization
        #   1. Every time a file is in the process of being created this part of the code will iterate through already existing files making sure that
        #       someone is incapable of creating two files with the same name.
        #   2. The first and last name are compared withing files to make sure the same information is not created twice

#4      #                   Udating files instead of deleting them
        #   1. This part of the code makes sure that once someone inserts his first and last name an already existing file is accessed and updated  instead of creating a seperate file
