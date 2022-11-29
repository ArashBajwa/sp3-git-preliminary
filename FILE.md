1. git clone <remote-url><br>
2. [Edited example.txt]<br>
3. git add example.txt<br>
4. git commit -m “C0”<br>
5. git branch -M master **HEAD->master**<br>
6. git branch bug-fix<br>
7. [Edited example.txt]<br>
8. git commit -a -m “C1”<br>
9. [Edited example.txt]<br>
10. git commit -a -m “C2”<br>
11. git checkout bug-fix **HEAD->bug-fix**<br>
12. [Edited example.txt]<br>
13. git commit -a -m “C3”<br>
14. [Edited example.txt]<br>
15. git commit -a -m “C4”<br>
16. git branch bug-fix-experimental<br>
17. git merge master -m “C5”<br>
18. git add example.txt<br>
19. git commit -a -m "C5 (merge conflict)"<br>
10. [Edited example.txt]<br>
11. git commit -a -m “C6”<br>
12. git checkout bug-fix-experimental **HEAD->bug-fix-experimental**<br>
13. [Edited example.txt]<br>
14. git commit -a -m “C7”<br>
15. [Edited example.txt]<br>
16. git commit -a -m “C8”<br>
17. [Edited example.txt]<br>
18. git commit -a -m “C9”<br>
19. git checkout master **HEAD->master**<br>
20. [Edited example.txt]<br>
21. git commit -a -m "C10"<br>
22. git checkout bug-fix **HEAD->bug-fix**<br>
23. git merge bug-fix-experimental -m “C11”<br>
24. git add example.txt<br>
25. git commit -a -m "C11 (merge conflict)"<br>
26. [Edited example.txt]<br>
27. git commit -a -m “C12”<br>
28. git checkout master **HEAD->master**<br>
29. git merge bug-fix -m “C13”<br>
30. git add example.txt<br>
31. git commit -a -m "C13 (merge conflict)"<br>
32. git push -u origin master<br>
33. git checkout bug-fix **HEAD->bug-fix**<br>
34. git push -u bug-fix<br>
35. git checkout bug-fix-experimental **HEAD->bug-fix-experimental**<br>
36. git push -u bug-fix-experimental<br>