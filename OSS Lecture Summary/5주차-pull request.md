# ๐ ๊นํ๋ธ ์ฐ๋ ๋ฐ ์๊ฒฉ ๋ฑ๋ก
## ๋ก์ปฌ ์ ์ฅ์๋ฅผ ์๊ฒฉ ์ ์ฅ์์ ์ฐ๊ฒฐํ๊ธฐ
์๋ก์ด ๋ก์ปฌ ์ ์ฅ์๋ฅผ ์์ฑํ๊ณ  ์๊ฒฉ ์ ์ฅ์๋ฅผ ์ฐ๊ฒฐํ์ฌ ๋ณด์.

์ฐ์  ์ ๋ก์ปฌ ์ ์ฅ์๋ฅผ ์์ฑํ ํ README.md ํ์ผ์ ๋ง๋ค์ด ์ถ์  ๋ฑ๋ก, ์ปค๋ฐํ๋ค.
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w
$ git init
Initialized empty Git repository in C:/OSS/git/05w/.git/

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ echo "# gitstudy05" >> README.md

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git add README.md

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git commit -m "first commit"
[main (root-commit) aa746c8] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```
<br/>

์ด์  ์๊ฒฉ ์ ์ฅ์์ ์ฐ๊ฒฐํด ๋ณด๊ฒ ๋ค.  
์๊ฒฉ ์ ์ฅ์์ ์ฐ๊ฒฐํ๋ ค๋ฉด ๋ค์๊ณผ ๊ฐ์ด **add ์ต์**์ ์ฌ์ฉํด์ผ ํ๋ค.  

**$ git remote add ์๊ฒฉ์ ์ฅ์๋ณ์นญ ์๊ฒฉ์ ์ฅ์URL**

```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git remote add origin https://github.com/kanujoa/gitstudy05_test.git     # ์์ ์ ์๋ฒ ์ฃผ์๋ฅผ ์๋ ฅํ๋ค.(origin์ ๋ณ์นญ์ผ๋ก ์ค์ ํจ.)

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git remote -v     # ์๊ฒฉ ์ ์ฅ์ ๋ชฉ๋ก ํ์ธ
origin   https://github.com/kanujoa/gitstudy05_test.git (fetch)
origin   https://github.com/kanujoa/gitstudy05_test.git (push)

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git remote show origin     # 'git remote show ์๊ฒฉ์ ์ฅ์๋ณ์นญ'์ ์๊ฒฉ ์ ์ฅ์์ ์์ธํ ์ ๋ณด๋ฅผ ์ถ๋ ฅ์์ผ์ค๋ค.
* remote origin
  Fetch URL: https://github.com/kanujoa/gitstudy05_test.git
  Push  URL: https://github.com/kanujoa/gitstudy05_test.git
  HEAD branch: main
  Remote branch:
    main new (next fetch will store in remotes/origin)
  Local ref configured for 'git push':
    main pushes to main (local out of date)
```
<br/><br/>


# ๐ ์๋ฒ ์ ์ก
## push: ์๋ฒ์ ์ ์ก
โ๏ธ **push**: ์๊ฒฉ ์ ์ฅ์๋ก ์ปค๋ฐ๋ ํ์ผ๋ค์ ์๋ก๋ํ๋ ๋์์ด๋ค.  

โถ๏ธ ์์ ์ ๋ก์ปฌ ์ ์ฅ์๋ฅผ '๋ฐฑ์'ํ๋ ์ฉ๋๋ก ์๊ฒฉ ์ ์ฅ์๋ฅผ ์ฌ์ฉ ๊ฐ๋ฅํ๋ค.
<br/><br/>

git remote -v ๋ช๋ น์ด๋ฅผ ์ด์ฉํด ์๋ก๋๊ฐ ๊ฐ๋ฅํ ์๊ฒฉ ์ ์ฅ์๊ฐ ๋ฑ๋ก๋์ด ์๋ ๊ฒ์ ํ์ธํ๋ค.   
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git remote -v
origin  https://github.com/kanujoa/gitstudy05_test.git (fetch)
origin  https://github.com/kanujoa/gitstudy05_test.git (push)
```
<br/>

push ๋ช๋ น์ด๋ฅผ ์ฌ์ฉํด ํ์ฌ main ๋ธ๋์น๋ฅผ origin ์๋ฒ๋ก ์ ์กํ๋ค.
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 223 bytes | 55.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kanujoa/gitstudy05_test.git
 * [new branch]       main -> main
```
<br/>

์๋ก๋ ๊ฒฐ๊ณผ๋ฅผ ์๋ฒ ์ ์ฅ์์์ ํ์ธํ๋ค. ๋ค์๊ณผ ๊ฐ์ด gitstudy05.md๊ฐ ์๋ฐ์ดํธ ๋์ด ์๋ ๊ฒ์ ํ์ธ ๊ฐ๋ฅํ๋ค.
<br/><br/><br/>


# ์๋์ผ๋ก ๋ด๋ ค๋ฐ๊ธฐ
## clone: ๋ณต์ 
โ๏ธ **clone**: ๊ธฐ์กด ์ ์ฅ์๋ฅผ ์ด์ฉํ์ฌ ์๋ก์ด ์ ์ฅ์๋ฅผ ์์ฑํ๋ ๋ฐฉ๋ฒ ์ค ํ๋

โถ๏ธ clone ๋ช๋ น์ด๋ฅผ ์ฌ์ฉํ๋ฉด ์ด๊ธฐํ init ๋ช๋ น์ด ์ธ์ ์๊ฒฉ ์๋ฒ ์ ์์ ํ์ํ ์ถ๊ฐ ์ค์ ์ ์๋์ผ๋ก ์ํํ๊ณ  ์๋ฒ์ ์ฐ๊ฒฐ ์ค์ ์ ๋ง์น ํ ์๋ฒ ์์ ์๋ ๋ชจ๋  ์ปค๋ฐ๋ ์ฝ๋ ์ด๋ ฅ๋ค์ 
   ํ ๋ฒ์ ๋ด๋ ค๋ฐ๋๋ค.
<br/><br/>

์๋ก์ด ํด๋๋ฅผ ๋ง๋ค์ด ์๊น gitstudy05_test ์ ์ฅ์๋ฅผ cloneํด ๋ณด๊ฒ ๋ค.
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w_clone
$ git clone https://github.com/kanujoa/gitstudy05_test.git     # clone ๋ช๋ น์ด์ ์ ์ฅ์ ์ฃผ์๋ฅผ ๊ฐ์ด ์ ์ด์ฃผ๋ฉด ๋๋ค.
Cloning into 'gitstudy05_test'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```
<br/><br/>

## pull: ์๋ฒ์์ ๋ด๋ ค๋ฐ๊ธฐ
โ๏ธ **pull**: ์๊ฒฉ ์ ์ฅ์์ ๊ฐฑ์ ๋ ๋ด์ฉ์ ์ถ๊ฐ๋ก ๋ด๋ ค๋ฐ๊ธฐ ์ํ์ฌ ์ฌ์ฉํ๋ ๋ช๋ น์ด์ด๋ค.

โถ๏ธ pull ๋ช๋ น์ด๋ฅผ ์ฃผ๊ธฐ์ ์ผ๋ก ์ฌ์ฉํ๋ฉด ์ต์  ์ปค๋ฐ ์ ๋ณด๋ก ๋ก์ปฌ ์ ์ฅ์๋ฅผ ์ ์งํ  ์ ์๋ค.
<br/><br/>

์ค์ต์ ์ํด ์๋ณธ ๋ก์ปฌ ์ ์ฅ์๋ก ์ด๋ํ๋ค.
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w_clone
$ cd ..

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git
$ cd 05w

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ code server.htm     # server.htm์ด๋ผ๋ ํ์ผ์ ๋ง๋ค์ด VSCode๋ก ํธ์งํ๊ธฐ
```
<br/>

๋ค์๊ณผ ๊ฐ์ด ์ฝ๋ ๋ด์ฉ์ ์์ฑํ๋ค.
![image](https://user-images.githubusercontent.com/99963066/204382871-2136ac1a-b690-4414-a8c6-e6dd153a2dac.png)
<br/>

```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git add server.htm     # server.htm์ SA์ ์ฌ๋ฆฌ๊ธฐ

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git commit -m "good day"     # ์ปค๋ฐํ๊ธฐ
[main 8fd17da] good day
 1 file changed, 2 insertions(+)
 create mode 100644 server.htm

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git push origin main      # ์๋ฒ๋ก push ํ๊ธฐ(์ด๋ก์จ gitstudy05_test์ server.htm ํ์ผ์ด ์ถ๊ฐ๋๋ค.)
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 113.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kanujoa/gitstudy05_test.git
   aa746c8..8fd17da  main -> main
```
<br/>

๋ค์ ๋ณต์  ์ ์ฅ์๋ก ๊ฐ๋ณด์.  
๋ณต์  ์ ์ฅ์์๋ ์์ง first commit ์ด ์ปค๋ฐ ํ๋๋ง ์๋ ๊ฒ์ ํ์ธํ  ์ ์๋ค.  
์ด๋ฒ์๋ ์๊ฒฉ ์ ์ฅ์์์ ๊ฐฑ์ ๋ ์ ์ปค๋ฐ ์ ๋ณด๋ฅผ ๊ฐ์ง๊ณ  ์จ๋ค.
<br/>

**'git pull'** ๋ช๋ น์ด๋ฅผ ์ฌ์ฉํ๋ฉด ์๊ฒฉ ์ ์ฅ์์ ๊ฐฑ์ ๋ ๋ก์ปฌ ์ ์ฅ์์ ์ปค๋ฐ ์ ๋ณด์ ๋น๊ตํ์ฌ ๊ฐฑ์ ํ๋ค.  
๋ค์ ๋ณต์ ๋ ์ ์ฅ์์์ log ๋ช๋ น์ด๋ฅผ ์คํํ๋ฉด first commit, good day ์ด๋ ๊ฒ 2๊ฐ์ ์ปค๋ฐ์ด ๋จ๋ ๊ฒ์ ํ์ธํ  ์ ์๋ค.
<br/><br/><br/>


# ๐ ์๋์ผ๋ก ๋ด๋ ค๋ฐ๊ธฐ
## fetch
โ๏ธ **fetch(ํ์น)**: ์๊ฒฉ ์ ์ฅ์์์ ์ฝ๋๋ฅผ ์๋์ผ๋ก ๋ด๋ ค๋ฐ๋ ์์์ ํ๋ค. ๋ค์๊ณผ ๊ฐ์ ์ฝ๋๋ฅผ ์์ฑํ์ฌ ์คํํ  ์ ์๋ค.  
โถ๏ธ **git fetch ์๊ฒฉ์ ์ฅ์URL**
<br/>

```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ code server.htm     # VSCODE๋ฅผ ์ผ์ ์๋ ์ฌ์ง๊ณผ ๊ฐ์ด ์ฝ๋๋ฅผ ์์ ํ๋ค.
```
<br/>

![image](https://user-images.githubusercontent.com/99963066/204474732-b4404e52-b721-462f-a7dd-54be752e8693.png)
<br/>

```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git commit -am "look sky"     # ์์ ๋ ํ์ผ์ ์คํ์ด์ง ์์ญ์ ๋ฑ๋ก๊ณผ ๋์์ ์ปค๋ฐํ๋ค.
[main 420e411] look sky
 1 file changed, 2 insertions(+), 1 deletion(-)

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ git push origin main     # push ๋ช๋ น์ด๋ฅผ ์ด์ฉํด ์ปค๋ฐ๋ ์์  ๋ด์ฉ์ ์๊ฒฉ ์ ์ฅ์๋ก ์ ์กํ๋ค.
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 366 bytes | 91.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kanujoa/gitstudy05_test.git
   8fd17da..420e411  main -> main
```
<br/>

๋ค์
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w (main)
$ cd ..     # ํด๋๋ฅผ ์ด๋ํ๋ค.

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git
$ cd 05w_clone     # 05w_clone ์ ์ฅ์(๋ณต์  ํด๋)๋ก ์ด๋ํ๋ค.

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w_clone (main)
$ git fetch     # fetch ๋ช๋ น์ด๋ฅผ ์ด์ฉํด ์ปค๋ฐ์ ๋ด๋ ค๋ฐ๋๋ค.
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 346 bytes | 16.00 KiB/s, done.
From https://github.com/kanujoa/gitstudy05_test
   8fd17da..420e411  main       -> origin/main
```
<br/>

ํ์น ํ ์๊ฒฉ ์ ์ฅ์์ ์ปค๋ฐ ๋ด์ฉ์ ์ดํด๋ณด๋ฉด ์ปค๋ฐ ๋ก๊ทธ๊ฐ ๋์ค๋ ๊ฒ์ ํ์ธํ  ์ ์๋ค.  
pull ๋ช๋ น์ด์ ๋ค๋ฅด๊ฒ fetch ๋ช๋ น์ด๋ฅผ ์คํํ ํ์๋ ์ปค๋ฐ์ด ์ถ๊ฐ๋ ๊ฒ์ ํ์ธํ  ์ ์๋ค.
<br/><br/><br/>


# ๐ merge ๋ช๋ น์ด๋ก ์๋ ๋ณํฉ
ํ์น๋ ๋ฐ์ดํฐ๋ฅผ ๋ด๋ ค๋ฐ๊ธฐ๋ง ํ  ๋ฟ ์๋ ๋ณํฉํ์ง ์๋๋ค. ๋ด๋ ค๋ฐ์ ์ปค๋ฐ์ ๋ก์ปฌ ์ ์ฅ์์ ์ ์ฉํ๋ ค๋ฉด ๋ณํฉ ๋ช๋ น์ ์คํํด์ผ ํ๋๋ฐ, ์ด๋ merge ๋ช๋ น์ด๋ฅผ ์ฌ์ฉํ๋ค.  
```bash
๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w_clone (main)
$ git merge origin/main     # ์์ ์๊ฒฉ ๋ธ๋์น ๋ณํฉ

๋๋น@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/05w_clone (main)
$ git log     # ๋ก๊ทธ๋ฅผ ํ์ธํ์ฌ ๋ค์ ๋ก์ปฌ ์ ์ฅ์์ ๋ก๊ทธ ๊ธฐ๋ก์ ํ์ธํ๋ค.
commit 420e411b83781c643ee7bd85229136c790821aef (HEAD -> main, origin/main)
Author: yubeenso <youbin0105@gmail.com>
Date:   Tue Nov 29 17:19:13 2022 +0900

    look sky     

commit 8fd17da66b985e1bb3d3e5e4aa899a8b73ab8945
Author: yubeenso <youbin0105@gmail.com>
Date:   Tue Nov 29 06:18:34 2022 +0900

    good day

commit aa746c8ad10d909137794a55da2495905b0f8aa4
Author: yubeenso <youbin0105@gmail.com>
Date:   Tue Nov 29 00:23:30 2022 +0900

    first commit
```
