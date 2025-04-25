33071@WAN MINGW64 ~
$ cd C:/Users/33071/iCloudDrive/iCloud~md~obsidian/Markdown\ on\ ipad

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad ((67f4d40...))
$ git checkout -b temporary
Switched to a new branch 'temporary'

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git log
commit 67f4d40acc90c6951856d74fe5f21f37e6fce150 (HEAD -> temporary)
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 17:10:03 2024 +0800

    sync test

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ cp C:/PersonalDevelopment/DeepLearningNotes/* .
cp: -r not specified; omitting directory 'C:/PersonalDevelopment/DeepLearningNotes/Hobbies'
cp: -r not specified; omitting directory 'C:/PersonalDevelopment/DeepLearningNotes/Subjects'

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ cp^C

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ cp -ri C:/PersonalDevelopment/DeepLearningNotes/* .
cp: overwrite './Git-learning.md'? y
cp: overwrite './Hobbies/Cooking/烹饪课堂（姜jiao瘦）.md'? y
cp: overwrite './Hobbies/Cooking/菜品.md'? y
cp: overwrite './Library-book-searching.md'? y
cp: overwrite './Markdown学习.md'? y
cp: overwrite './Recent Schedule.md'? y
cp: overwrite './SSH.md'? y
cp: overwrite './Subjects/大物.md'? y
cp: overwrite './Subjects/Images/IMG_0374.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0375.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0369.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0371.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0372.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0373.jpeg'? y
cp: overwrite './Subjects/Images/IMG_0370.jpeg'? y
cp: overwrite './Subjects/电路实验/电路元件特性曲线的伏安测量法和示波器观测法.md'? y
cp: overwrite './Subjects/电路实验/戴维南定理验证（10.8，第三次）.md'? y
cp: overwrite './Subjects/电路实验/调谐电路功效的研究.md'? y
cp: overwrite './Subjects/电路实验/交流阻抗等效参数的测量.md'? y
cp: overwrite './basic-coding.md'?
cp: overwrite './大学物理.md'? y
cp: overwrite './科目一.md'? y

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git add .
warning: in the working copy of 'Hobbies/Cooking/烹饪课堂（姜jiao瘦）.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Hobbies/Cooking/菜品.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/大物.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/电路实验/交流阻抗等效参数的测量.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/电路实验/戴维南定理验证（10.8，第三次）.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/电路实验/电路元件特性曲线的伏安测量法和示波器观测法.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/电路实验/调谐电路功效的研究.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'Subjects/电路元件特性曲线的伏安测量法和示波器观测法.md', LF will be replaced by CRLF the next time Git touches it

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git commit .
warning: in the working copy of 'Subjects/电路元件特性曲线的伏安测量法和示波器观测法.md', LF will be replaced by CRLF the next time Git touches it
[temporary cb4e61e] right clone
 10 files changed, 952 insertions(+)
 create mode 100644 Git-learning.md
 create mode 100644 "Hobbies/Music/Guitar/music score/\347\210\261\344\271\220\344\271\213\345\237\216.mscz"
 create mode 100644 Library-book-searching.md
 create mode 100644 "Markdown\345\255\246\344\271\240.md"
 create mode 100644 Recent Schedule.md
 create mode 100644 SSH.md
 create mode 100644 "Subjects/\347\224\265\350\267\257\345\205\203\344\273\266\347\211\271\346\200\247\346\233\262\347\272\277\347\232\204\344\274\217\345\256\211\346\265\213\351\207\217\346\263\225\345\222\214\347\244\272\346\263\242\345\231\250\350\247\202\346\265\213\346\263\225.md"
 create mode 100644 basic-coding.md
 create mode 100644 "\345\244\247\345\255\246\347\211\251\347\220\206.md"
 create mode 100644 "\347\247\221\347\233\256\344\270\200.md"

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git log
commit cb4e61e9cf23989d88f8c996e9412b863e8ea07d (HEAD -> temporary)
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 19:19:32 2024 +0800

    right clone

commit 67f4d40acc90c6951856d74fe5f21f37e6fce150
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 17:10:03 2024 +0800

    sync test

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git branch
  obsidian
* temporary

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git log --oneline --graph
* cb4e61e (HEAD -> temporary) right clone
* 67f4d40 sync test

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (temporary)
$ git checkout obsidian
Switched to branch 'obsidian'

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (obsidian)
$ git merge temporary
Merge made by the 'ort' strategy.
 Git-learning.md                                    | 126 ++++++++++
 ...0\261\344\271\220\344\271\213\345\237\216.mscz" | Bin 0 -> 20288 bytes
 Library-book-searching.md                          |  30 +++
 "Markdown\345\255\246\344\271\240.md"              | 257 +++++++++++++++++++++
 Recent Schedule.md                                 |  10 +
 SSH.md                                             |   0
 ...231\250\350\247\202\346\265\213\346\263\225.md" |  22 ++
 basic-coding.md                                    | 240 +++++++++++++++++++
 ...244\247\345\255\246\347\211\251\347\220\206.md" |  82 +++++++
 "\347\247\221\347\233\256\344\270\200.md"          | 185 +++++++++++++++
 10 files changed, 952 insertions(+)
 create mode 100644 Git-learning.md
 create mode 100644 "Hobbies/Music/Guitar/music score/\347\210\261\344\271\220\344\271\213\345\237\216.mscz"
 create mode 100644 Library-book-searching.md
 create mode 100644 "Markdown\345\255\246\344\271\240.md"
 create mode 100644 Recent Schedule.md
 create mode 100644 SSH.md
 create mode 100644 "Subjects/\347\224\265\350\267\257\345\205\203\344\273\266\347\211\271\346\200\247\346\233\262\347\272\277\347\232\204\344\274\217\345\256\211\346\265\213\351\207\217\346\263\225\345\222\214\347\244\272\346\263\242\345\231\250\350\247\202\346\265\213\346\263\225.md"
 create mode 100644 basic-coding.md
 create mode 100644 "\345\244\247\345\255\246\347\211\251\347\220\206.md"
 create mode 100644 "\347\247\221\347\233\256\344\270\200.md"

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (obsidian)
$ git status
On branch obsidian
nothing to commit, working tree clean

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (obsidian)
$ git log
commit c289e53187db1f3ddd5ba833119caedebe00c679 (HEAD -> obsidian)
Merge: 8a3ec3f cb4e61e
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 19:23:26 2024 +0800

    Merge branch 'temporary' into obsidian to make the right clone

commit cb4e61e9cf23989d88f8c996e9412b863e8ea07d (temporary)
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 19:19:32 2024 +0800

    right clone

commit 8a3ec3f9a0ddd73b338592047f57318df7320301
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 18:46:00 2024 +0800

    a wrong clone from typora to obsidian

commit 67f4d40acc90c6951856d74fe5f21f37e6fce150
Author: YUDI WAN <3307159743@qq.com>
Date:   Wed Oct 23 17:10:03 2024 +0800

    sync test

33071@WAN MINGW64 ~/iCloudDrive/iCloud~md~obsidian/Markdown on ipad (obsidian)
$ cd C:/PersonalDevelopment/DeepLearningNotes

33071@WAN MINGW64 /c/PersonalDevelopment/DeepLearningNotes (main)
$ cp -r C:/Users/33071/iCloudDrive/iCloud~md~obsidian/Markdown\ on\ ipad/* .

33071@WAN MINGW64 /c/PersonalDevelopment/DeepLearningNotes (main)
$ git remote
origin

33071@WAN MINGW64 /c/PersonalDevelopment/DeepLearningNotes (main)
$ git push
Enumerating objects: 23, done.
Counting objects: 100% (23/23), done.
Delta compression using up to 20 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (19/19), 22.57 KiB | 2.82 MiB/s, done.
Total 19 (delta 6), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (6/6), completed with 3 local objects.
To github.com:tfeathers0/Learning_notes.git
   8fd4709..76d2c6e  main -> main

33071@WAN MINGW64 /c/PersonalDevelopment/DeepLearningNotes (main)
$

![image-20241023193101460](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20241023193101460.png)![image-20241023193107517](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20241023193107517.png)![image-20241023193124009](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20241023193124009.png)![image-20241023193131260](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20241023193131260.png)![image-20241023193140310](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20241023193140310.png)