# Tugas 1 SEKURO *Programming*

<p>&nbsp;</p>

## Developer:
### 16521369 - Ahmad Rizki

<p>&nbsp;</p>

## Table of Contents
1. [APA ITU GIT & GITHUB](https://www.youtube.com/watch?v=lTMZxWMjXQU&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=1&t=710s)
2. [BEKERJA DENGAN GITHUB](https://www.youtube.com/watch?v=Q3Id0DgcrXY&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=2&t=421s)
3. [GITHUB: BRANCH](https://www.youtube.com/watch?v=k1QXd-8VbPY&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=3&t=723s)
4. [GITHUB: FORK](https://www.youtube.com/watch?v=8rry2ncZmfg&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=4)
5. [BEKERJA DENGAN GIT](https://www.youtube.com/watch?v=e-6OkXRqWaE&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=5)
6. [GIT BRANCH & MERGE](https://www.youtube.com/watch?v=EGl7KxVOyNs&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=6)
7. [GITIGNORE](https://www.youtube.com/watch?v=LK3kX4n-vLM&list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf&index=12)

<p>&nbsp;</p>

## APA ITU GIT & GITHUB
![](github-halovina.png)
GIT adalah salah satu contoh dari ***Version Control System*** atau disebut juga ***revision control system*** atau **source code management**. VCS (Version Control System) adalah sistem yang mengelola perubahan dari sebuah dokumen, program komputer, website, dan kumpulan informasi lain. Perubahan-perubahan tersebut dikelola dalama sebuah folder yang disebut repository/repo dan setiap perubahan perlu dilakukan commit terlebih dahulu.
Beberapa hal mengenai VCS :
- Sebuah sistem yang dapat menyimpan 'rekaman/snapshot perubahan pada source code'
- Memungkinkan bekerja berkolaborasi dengan lebih baik
- Mengetahui siapa yang melakukan dan kapan sebuah perubahan terjadi
- Memungkinkan kita untuk kembali ke keadaan sebelum perubahan (checkout)

GitHub adalah sebuah layanan cloud untuk menyimpan & mengelola project/repo git. Sama seperti pada GIT, github juga dapat dilakukan pembuatan repo, commit, branch, merge, namun semua itu dilakukan secara online. Atau bisa dibilang github adalah sebuah web yang didalamnya menggunakan web

GIT dan GitHub juga dapat dilakukan bersamaan dengan menggunakan push and pull

<p>&nbsp;</p>

## BEKERJA DENGAN GITHUB
![](bagian2.png)
Cara mengelola repository pada GitHub
- Buat akun GitHub terlebih dahulu pada https://github.com/.
- Tekan tanda (+) di bagian kanan atas dan tekan *"New Repository"*
- Isi nama repository beserta deskripsi(opsional), pilih apakah repo akan dipublic atau di private
- Centang *"Initialize this repository with a README"*, jika ingin repository memiliki file README.
- Lalu tekan Create Repository
- Jika didalam repo ingin ditambahkan file, tekan *"Create New FIle"*, 
- Setiap perubahan di dalam repository perlu dilakukan *"commit"* yang history commit akan tersimpan di dalam GitHub

<p>&nbsp;</p>

## GITHUB: BRANCH
Branching adalah membuat cabang dari repositori utama dan melanjutkan melakukan pekerjaan pada cabang yang baru tersebut tanpa perlu khawatir mengacaukan yang utama. Dengan branching memungkinkan 2 orang untuk melakukan kolaborasi dengan mengedit branch yang berbeda, yang kemudian akan disatukan dengan fitur git merge. Cara membuat Git Branch ada 2 cara :
- membuat branch secara langsung pada repository
<br> ![](cara1bag3.png) </br>
- menambah branch saat ingin melakukan commit, *"Create a new branch for this commit and start a pull request."*
<br> ![](cara2bag3.png) </br>

Setiap branch yang telah dibuat, dapat di gabungkan kembali ke branch utama (*master*) dengan melakukan merge dengan syarat tidak adanya konflik antara branch utama dan branch tersebut, atau dalam GitHub juga disebut *pull request*.
<br> ![](bagian-3.png) </br>

History dalam perubahan di repository dapat dilihat dalam sebuah graph di menu *"Insight"* bagian *'Network'*
![](graphbag3.png)

<p>&nbsp;</p>

## GITHUB: FORK
GitHub memungkinkan repository milik orang lain beserta history di dalam repository diduplikat ke dalam repository pribadi kita. Sehingga, kita dapat memodifikasi repo tersebut untuk kita gunakan pada project kita tersendiri, atau kita juga dapat berkontribusi pada repo orang lain dengan mengusulkan perubahan tersebut ke pemilik repo (*pull request*).
<br>![](bagian4.png)</br>

<p>&nbsp;</p>

## BEKERJA DENGAN GIT

![](photos/flowchart.jpg)

<p>&nbsp;</p>

The flowchart represents the overall procedural steps while the program is running. The steps explanation same as written below:

1. In the initial state , the starting ball will go to Team 1 and Team 1 will proceed to Kick-Off
2. The defending team automatically move to defensive position by remote signaling mechanism.
3. One of robots from the attacking team will proceed to move to the attacking area and positions itself within suitable attacking prowess.
4. Next, the passing mechanism will occur as the robot which starts with the ball passes to the robot which mentioned on step 3.
5. Lastly , the shooting mechanism will occur by applying the algorithm to detect suitable area to shoot on the goal.
6. The condition depends on whether the attacking team scores or not.
    - If the team scores , the game will reset to step 1 (with the ball goes to opposite team).
    - If the team doesn't score ,  the game will reset to step 2 (with the ball handled by the goalkeeper of the opposite team).
7. The procedure will never stop if there isn't any form of interruption.

<p>&nbsp;</p>

## GIT BRANCH & MERGE
Our robot movement is handled by publishing `twist` message to the `/cmd_vel` or `/planar_vel` topics. We used two input which is destination pose/coordinate and the odometry of the robot for the movement algorithm. At first, the robot will correct its orientation to face the destination. Then the robot will go to its destination in a straight line. Here are the demonstration,

![](photos/movement2.gif)

<p>&nbsp;</p>

## GIT IGNORE
For our robot ball chaser algorithm, we modified the movement algorithm to make its destination argument set to the ball pose message that we received from the /ball_state topic (message on this topic published from ball_state_pub node). The result is the robot will go to the ball's pose/coordinate. Here are the demonstration,

![](photos/ball_chaser2.gif)

<p>&nbsp;</p>

## Reference <a name = "ref"></a>

- MODUL 1 PROGRAMMING SEKURO Pengenalan Git & GitHub

- Playlist *GIT & GITHUB* Channel Web Programming UNPAS. https://www.youtube.com/playlist?list=PLFIM0718LjIVknj6sgsSceMqlq242-jNf. Accessed on 10 February 2022