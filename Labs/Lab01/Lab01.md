## Lab 01

- Name: Jacob Worst
- Email: worst.5@wright.edu

## Part 1 Answers

1.mkdir DirA
2.mkdir "Dir B"
3.cd "Dir B"
4.DirA is better as a naming convention because its easier to access without having to constantly put "" around Dir B.
5.mv "Dir B" DirB

## Part 2 Answers

1.touch test.txt
  vim test.txt
2. File contents:

```
First line of text.
Second line of text.
Third line of text.
```
used esc and :wq to save the file and leave vim.

## Part 3 Answers

1.cp test.txt .hiddentext.txt
2.ls -lah

## Part 4 Answers

1.adduser bob, my personal account wasn't root so I had to exit and adduser as the root
2.su bob into pwd switches my user to bob and shows me where i am in his directory
3.You cannot, as my user i did cd bob to switch to his directory then touch test.txt and it said permission denied.
4.su bob
5.cd /home
6.Yes because he has permission to write in the directory.
7.su jworst
8.cd /home

## Part 5 Answers

1.addgroup crew
2.adduser bob crew
3.as admin in the users directory, you do chgrp crew DirA
4.su bob
5.cd /home/jworst then cd DirA then touch test2.txt
6.It was successful because DirA is a directory in the crew group and bob is a member of the group.

## Part 6 Answers

1.touch sudowho.txt
2.ls -lah user has rw group has rw and all has r
3.vim sudowho.txt

## Extra Credit

1.sudo adduser sally
  sudo adduser sally crew
  sudo chgrp crew DirB
  su sally
  cd DirB
  touch mydiary.txt
  chmod g-r mydiary.txt
  chmod g-w mydiary.txt
  chmod a-r mydiary.txt
  i did ls -lah at this point and saw the user didnt have r permission
  chmod u+r mydiary.txt
2.You can do this by using sudo vim mydiary.txt
3.Bob can't do it because he doesn't have admin permissions.
