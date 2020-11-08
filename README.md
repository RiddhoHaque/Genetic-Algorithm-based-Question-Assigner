# Genetic Algorithm based Question Assigner
 Assigns questions randomly to students while using the genetic algorithm to minimize the number of same questions appearing to any pairs of students.

Use Case:
This randomization script typically works for the following use case (Please note that the values
mentioned here are just for example):
Suppose I have three students in my section, whose student ID-s are 2016-3-60-032,
2017-2-60-016 and 2017-2-60-143. I have set 7 questions in my question bank, and want each
of them to be assigned one question from the questions numbered 1 and 2, one from the
questions numbered 3 and 4, and one from the questions 5, 6 and 7. The first thing I would
have to do is copy and paste the ID-s of the students into the file “StudentID.csv”. Then, I would
have to run the script, and follow the instructions given in the screen. The script will first prompt
me to enter the number of questions each student will have to answer. In this use case, that
value is 3. Then the script will ask me to write down the range from which the first question will
have to be assigned to each student. In my case, that range is 1-2, and thus I will enter 1 and 2
on the screen. The script will then prompt me to enter the other ranges one by one, and thus I
shall enter 3 4 and 5 7. Once I’ve specified all the ranges, the script will run and generate the
“Question_List.csv” file. In the above use case, this is how the output file will look once the script
terminates.
Student ID Questions to answer
2016-3-60-32 1-4-6
2017-2-60-16 1-4-7
2017-2-60-143 2-3-5
Limitations (Reading this section is not necessary for using the script):
Usually, I share this csv file with my students in Google Classroom, and upload the Question
bank separately, and ask the students to view the csv file to know which questions they need to
answer. An obvious drawback of this approach is that students can see which of their other
classmates have to answer the same questions as they do. If you want, you can read the
following link ​https://developers.google.com/apps-script/articles/sending_emails to learn how
you can use the data in this csv to send separate emails to each student so that only they know
which questions they have to answer. However, I have not tried this in my own exams, since I
fear that such mails may not reach the students in time, may be forwarded to their spam folder,
or my own gmail account may suffer from temporary blockages due to the unusual traffic. In any
case, students can always reconstruct this table by making a shared google sheet amongst
themselves, making such efforts unproductive. My script attempts to remediate this drawback by
using the Genetic Algorithm to minimize the number of common questions between each pair of
students and the number of common questions between pairs of students who got admitted in
the same (or similar) semesters.Step-by-step Instructions:
A step-by-step instructions on how to run the script is given below :
Step 1:​ Download the files “StudentID.csv” and “Question_Randomizer_V1.exe” attached with
the mail. Save the files in the same folder.
Step 2:​ Copy the student ID-s of the students and paste them onto the file StudentID.csv. Make
sure each ID is in a separate row. The ID-s should be of the format “20XX-X-XX-XXX” (where
the X-s can be replaced by any digit).
Step 3:​ Double click on the file Question_Randomizer_V1.exe . You may need to deactivate
your computer’s antivirus program temporarily in order to run it, in case you have any installed.
Do not worry, the program is completely safe.
Step 4:​ Follow the prompts that appear on the screen. Once you are done giving all the inputs,
the program may take around a minute to finish running. Once it ends, the black window that
had been running will disappear. Open the file “Question_List.csv” , you will find that for each
student, the set of questions that he has to answer has been generated.
Step 5: ​In case you temporarily deactivated your antivirus earlier on, this step is a reminder to
activate it again now!