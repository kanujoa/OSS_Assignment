# π λ³ν©
**- λ³ν©(ν©μΉκΈ°): λΆλ¦¬λ λΈλμΉλ₯Ό ν λΈλμΉλ‘ ν©μΉλ μμ**

βοΈ μλ λ³ν©: μμͺ½ νμΌμ μΌμΌμ΄ λΉκ΅νλ©° λ°λ μ μ μ°Ύμμ μ μ©ν΄μΌ νλ€.
<br/>

βοΈ **κΉμΌλ‘ μλ λ³ν©**: μλ³Έμ κΈ°μ€μΌλ‘ λ νμΌμ λ³κ²½ μ΄λ ₯μ λΉκ΅νλ€. 
- κΉμ λ³ν©μ λΈλμΉλ₯Ό κΈ°μ€μΌλ‘ νλ€. λΆλ¦¬λ κ°κ°μ λΈλμΉμμ μμ λ μ¬ν­μ νλμ λΈλμΉλ‘ λ³ν©νλ―λ‘ λ³ν©νκ³ μ νλ λΈλμΉλ κ°μ λ‘μ»¬ μ μ₯μμ μμ΄μΌ νλ€.
- κΉμ΄ λͺ¨λ  μ½λμ λ³ν©μ μλ²½νκ² μ²λ¦¬ν  μλ μλλ° 'μΆ©λ' μν©μμλ μ½λμ λ³ν©μ μλμΌλ‘ λ°μνμ§ λͺ»νλ€.
<br/>

βοΈ **Fast-Forward λ³ν©**   
- λΉ¨λ¦¬ κ°κΈ° λ³ν©μ μΌλ°μ μΌλ‘ νΌμ κ°λ°ν  λ μ¬μ©!
- νΌμ κ°λ° μμλ λΈλμΉκ° μμ±λ μ»€λ°μ λ°λΌ μμ°¨μ μΌλ‘ λΆκΈ°λκ³  μ½λ μμ λ μμ°¨μ μΌλ‘ ν  λκ° λ§μ. μ΄λ¬ν μμ°¨μ  μ»€λ°μ λ§μΆμ΄ λ³ν©μ μ²λ¦¬νλ λ°©λ²μ΄ Fast-Forward
  λ³ν©μ!
<br/>

βοΈ **3-way λ³ν©**
- μ¬λ¬ κ°λ°μμ νμμΌλ‘ μμνλ κ²½μ° λλΆλΆ 3-way λ³ν©μ μ¬μ©νλ€.
- λ λΈλμΉμμ κ³΅ν΅ μ‘°μ μ»€λ°μ μλμΌλ‘ μ°Ύμ μ£Όλ©° κ³΅ν΅ μ‘°μ μ»€λ°μ κΈ°μ€μΌλ‘ λΈλμΉλ₯Ό λ³ν©νλ€. 
- λ³ν©μ μ±κ³΅μ μΌλ‘ μλ£ν νμλ μλ‘μ΄ μ»€λ°μΈ λ³ν© μ»€λ°μ μΆκ°λ‘ νλ μμ±νλ€.
<br/><br/><br/>


# μ€μ΅ 1
1. μ μ₯μ mgctλ₯Ό μμ±νμ¬ λΈλμΉ mainμμ 1κ°μ μ»€λ°(aaa ν μ€λ‘ νμΌ h.py μμ±) λ¨Όμ  μμ±  
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό
$ git init mgct     # μ μ₯μ mgct μμ±
Initialized empty Git repository in C:/OSS/git/10μ£Ό/mgct/.git/

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό
$ cd mgct     # μ μ₯μ mgctλ‘ μ΄λ

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ echo aaa > h.py     

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git add .

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git commit -m 'Add aaa'     # μ»€λ°
[main (root-commit) 13395b8] Add aaa
 1 file changed, 1 insertion(+)
 create mode 100644 h.py
```
<br/>

2. λΈλμΉ devp μμ± ν μ΄λν΄μ νμΌ h.py μμ (111 μΆκ°) ν μ»€λ°
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git checkout -b devp     # λΈλμΉ devpλ₯Ό μμ± ν μ΄λ
Switched to a new branch 'devp'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (devp)     # λΈλμΉ devpλ‘ μ΄λν¨.
$ echo 111 >> h.py     # νμΌ h.pyμ λ΄μ© μΆκ°

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (devp)
$ git commit -am 'Add 111'     # μ»€λ°
[devp 33f9db7] Add 111
 1 file changed, 1 insertion(+)
```
<br/>

3. λ€μ λΈλμΉ mainμμ νμΌ h.py μμ (bbb μΆκ°) ν μ»€λ°
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (devp)
$ git checkout main     # main λΈλμΉλ‘ μ΄λνλ€.
Switched to branch 'main'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ echo bbb >> h.py      # νμΌ h.pyμ λ΄μ© μΆκ°

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ cat h.py     # h.pyμ νμΌ λ΄μ© νμΈ
aaa
bbb

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all     # λͺ¨λ  μ μ₯μμμμ μ»€λ° μ΄λ ₯ ν μ€λ‘ λ³΄κΈ°
* 33f9db7 (devp) Add 111
* 13395b8 (HEAD -> main) Add aaa

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git commit -am 'Add bbb'     # μ»€λ°
[main a288fec] Add bbb
 1 file changed, 1 insertion(+)

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all     
* a288fec (HEAD -> main) Add bbb     # main λΈλμΉμμ μ»€λ°μ μ§νν¨μΌλ‘μ¨ devpμμ μ§νν μ»€λ°λ³΄λ€ μμλκ° μλ κ²μ νμΈ
| * 33f9db7 (devp) Add 111
|/
* 13395b8 Add aaa
```
<br/><br/>


# μ€μ΅ 2
1. main λΈλμΉμμ devpλ₯Ό 3-way λ³ν©, μΆ©λ λ°μ νμΈ
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git merge devp     # merge λͺλ Ήμ΄λ₯Ό μ¬μ©ν΄ main λΈλμΉμμ devpλ₯Ό λ³ν©νλ €κ³  ν¨.
Auto-merging h.py
CONFLICT (content): Merge conflict in h.py
Automatic merge failed; fix conflicts and then commit the result.

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main|MERGING)
$ cat h.py     # h.py νμΌ λ΄μ©μ νμΈν΄ λ³΄λ©΄ main λΈλμΉμμμ bbbλΌλ λ΄μ©κ³Ό devp λΈλμΉμμμ 111 λ΄μ©μμ
aaa            # μΆ©λμ΄ λ°μν κ²μ νμΈν  μ μλ€.
<<<<<<< HEAD
bbb
=======
111
>>>>>>> devp
```
<br/>

2. λ³ν© μ μΆ©λν λ΄μ©μΈ 111κ³Ό bbbλ₯Ό λͺ¨λ νμΌ λ΄μ©μΌλ‘ λ°μμν¨λ€.
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main|MERGING)
$ code h.py     # VSCodeλ₯Ό μ΄μ΄ μ΄λ»κ² λ³ν©ν  κ±΄μ§λ₯Ό κ²°μ νλ€.
```

![image](https://user-images.githubusercontent.com/99963066/204138502-9a6bf55e-1c92-4670-83af-fa1044c1d295.png)

```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main|MERGING)
$ git commit -am '3-way merge'     # 3-way λ³ν©μ νμμΌλ―λ‘ λ³ν© μ»€λ° λ©μμ§λ₯Ό μμ±νκ³  μ»€λ°ν΄ μ€λ€.
[main 08f3d40] 3-way merge

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all     # μ»€λ° μ΄λ ₯μ νμΈνμ¬ λ³ν©μ΄ μ λλ‘ λμλμ§ νμΈνλ€.
*   08f3d40 (HEAD -> main) 3-way merge
|\
| * 33f9db7 (devp) Add 111     # bbbμ 111μ΄ λͺ¨λ λ°μμ΄ λμ΄ λ³ν©μ΄ λ κ²μ νμΈν  μ μλ€.
* | a288fec Add bbb
|/
* 13395b8 Add aaa
```
<br/><br/>

# μ€μ΅ 3
λ€μ main λΈλμΉμμ μμμ νλ€.

1. λΈλμΉ devpκ° mergedμΈμ§λ₯Ό νμΈ ν λΈλμΉ devpλ₯Ό μ­μ 
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch
  devp
* main     # νμ¬ λΈλμΉλ mainμ΄λ€.

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch --merged      # λ³ν©λ λΈλμΉ νμΈ
  devp     # devp λΈλμΉλ λ³ν© μνμ΄λ€.
* main     # νμ¬ λΈλμΉλ mainμ΄λ€.

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch -d devp      # -d μ΅μμ μ¬μ©νμ¬ devp λΈλμΉλ₯Ό μ­μ νλ€.
Deleted branch devp (was 33f9db7).
```
<br/>

2. μλ‘μ΄ λΈλμΉ hotfixλ₯Ό λ§λ€μ΄ μ΄λ ν νμΌ h.py μμ (222 λ΄μ© μΆκ°) ν μ»€λ°
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git switch -c hotfix     # -c μ΅μμ μ¬μ©νμ¬ hotfix λΈλμΉ μμ± ν μ΄λ
Switched to a new branch 'hotfix'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (hotfix)
$ cat h.py     # hotfix λΈλμΉμμμ μ΄κΈ° h.py νμΌ λ΄μ© νμΈ
aaa
bbb
111

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (hotfix)
$ echo 222 >> h.py     # h.pyμ λ΄μ© μΆκ°νκΈ°

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (hotfix)
$ git commit -am 'Add 222'     # μ»€λ° λ©μμ§ μμ± ν μ»€λ°
[hotfix 8f79694] Add 222
 1 file changed, 1 insertion(+)

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (hotfix)
$ git log --oneline --graph --all     # μ»€λ° μ΄λ ₯ νμΈ
* 8f79694 (HEAD -> hotfix) Add 222     # μλ‘ μμ±ν hotfix λΈλμΉμμ Add 222 μ»€λ°μ΄ λ°μν κ²μ νμΈν  μ μλ€.
*   08f3d40 (main) 3-way merge
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa
```
<br/>

3. λ€μ main λΈλμΉμμ λΈλμΉ hotfixλ₯Ό λΉ λ₯Έ ffλ‘ λ³ν©νλ€.
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (hotfix)
$ git checkout main     # main λΈλμΉλ‘ μ΄λνλ€.
Switched to branch 'main'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all     # μ»€λ° μ΄λ ₯μ λ³Έλ€.
* 8f79694 (hotfix) Add 222
*   08f3d40 (HEAD -> main) 3-way merge
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git merge hotfix     # hotfix λΈλμΉλ₯Ό λ³ν©νλ€. μ¬κΈ°μμλ Fast-Forward λ³ν©μ΄ λλ€.
Updating 08f3d40..8f79694
Fast-forward
 h.py | 1 +
 1 file changed, 1 insertion(+)

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all      # μ»€λ° μ΄λ ₯μ νμΈν΄ λ³ν©μ΄ μ λλ‘ λμλμ§λ₯Ό νμΈνλ€.
* 8f79694 (HEAD -> main, hotfix) Add 222     # λ³ν©μ΄ λμ΄ main λΈλμΉμ hotfix λΈλμΉκ° κ°μ μμΉμ μλ κ²μ νμΈν  μ μλ€.
*   08f3d40 3-way merge
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ cat h.py
aaa
bbb
111
222     # main λΈλμΉμμλ 222 λ΄μ©μ΄ μΆκ°λμ΄ μλ κ²μ λ³Ό μ μλ€.
```
<br/>

# μ€μ΅ 4
1. main λΈλμΉμμ μλ‘μ΄ λΈλμΉμΈ featureλ₯Ό λ§λ€μ΄ νμΌ h.pyλ₯Ό μμ (333 λ΄μ© μΆκ°) ν μ»€λ°νλ€.
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git checkout -b feature     # feature λΈλμΉ μμ± ν μ΄λνλ€.

Switched to a new branch 'feature'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ echo 333 >> h.py      # h.pyμ λ΄μ©μ μΆκ°νλ€.

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ git commit -am 'Add 333'     # μ»€λ°μ μ§ννλ€.
[feature 7a40c7c] Add 333
 1 file changed, 1 insertion(+)

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ git log --oneline --graph --all     # μ»€λ° μ΄λ ₯μ νμΈνλ€.
* 7a40c7c (HEAD -> feature) Add 333     # feature λΈλμΉμμ Add 333 λ΄μ©μ μ»€λ°μ΄ μ΄λ£¨μ΄μ§ κ²μ νμΈν  μ μλ€.
* 8f79694 (main, hotfix) Add 222
*   08f3d40 3-way merge
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ git branch      # λΈλμΉ λͺ©λ‘ νμΈ
* feature
  hotfix
  main

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ git branch --merged     # λ³ν©λ λΈλμΉλ₯Ό νμΈ
* feature
  hotfix
  main
```
<br/>

2. λ€μ main λΈλμΉμμ λ³ν©λ λΈλμΉμ λ³ν©λμ§ μμ λΈλμΉλ₯Ό νμΈ
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (feature)
$ git checkout -     # main λΈλμΉλ‘ μ΄λνλ€.
Switched to branch 'main'

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch --no-merged     # main λΈλμΉμμ λ³ν©μ΄ λμ§ μμ λΈλμΉλ feature λΈλμΉμμ νμΈ κ°λ₯
  feature
```
<br/>

3. mainμμ λΈλμΉ featureλ₯Ό 3-way λ³ν©νλ€.
- λ³ν© μ μ΅μ **--no-ff**λ₯Ό λ°λμ μ¬μ©ν΄μΌ νλ€.
- λ³ν© μ μ λ°λμ VSCodeμμ λ³ν© μ»€λ° λ©μμ§λ₯Ό μμ±ν΄μΌ νλ€.

```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git merge feature --no-ff
hint: Waiting for your editor to close the file...
```

![image](https://user-images.githubusercontent.com/99963066/204141585-d0681280-3a41-4a3a-9db8-4a88c8df8799.png)

μμ κ°μ΄ λ³ν© μ»€λ° λ©μμ§ μμ± ν μ μ₯ν ν μ€νν΄μΌ νλ€.

```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git merge feature --no-ff     
Merge made by the 'ort' strategy.
 h.py | 1 +
 1 file changed, 1 insertion(+)     # μ»€λ° λ©μμ§ μμ±μ΄ μλ£ ν VSCodeλ₯Ό λ«μΌλ©΄ μκ³Ό κ°μ λ©μμ§κ° λ¬λ€.

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all     
*   dc9f828 (HEAD -> main) Merge branch 'feature' by 3-way merge     # 3-way λ³ν©μ΄ μλ£λμκ³  λ΄κ° μμ±ν λ³ν© μ»€λ° λ©μμ§λ λ¨λ κ²μ λ³Ό μ μλ€.
|\
| * 7a40c7c (feature) Add 333
|/
* 8f79694 (hotfix) Add 222
*   08f3d40 3-way merge
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa
```
<br/>

4. main λΈλμΉμμ mergeλ λΈλμΉμ mergeλμ§ μμ λΈλμΉλ₯Ό νμΈ ν λ³ν©λ hotfix λΈλμΉλ₯Ό μ­μ νλ€.
```bash
λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch --merged     # λͺ¨λ  λΈλμΉκ° λ³ν©λμ΄ μμμ νμΈν  μ μλ€.
  feature
  hotfix
* main

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git branch -d hotfix     # hotfix λΈλμΉλ₯Ό μ­μ νμλ€.
Deleted branch hotfix (was 8f79694).

λλΉ@DESKTOP-SKBKL14 MINGW64 /c/OSS/git/10μ£Ό/mgct (main)
$ git log --oneline --graph --all
*   dc9f828 (HEAD -> main) Merge branch 'feature' by 3-way merge
|\
| * 7a40c7c (feature) Add 333
|/
* 8f79694 Add 222
*   08f3d40 3-way merge      # hotfix λΈλμΉκ° μ­μ λ κ²μ λ³Ό μ μλ€.
|\
| * 33f9db7 Add 111
* | a288fec Add bbb
|/
* 13395b8 Add aaa
```
<br/><br/>

# μ€μ΅ 5
μμ€νΈλ¦¬λ₯Ό μ΄μ΄μ λΈλμΉ νμΈ ν λ³ν©λ λΈλμΉμΈ featureλ₯Ό μ­μ νλ€.

![image](https://user-images.githubusercontent.com/99963066/204142285-43d8b313-3e66-4c66-8cc3-68fe5ad22595.png)

μ΅μ’ κ²°κ³Όλ λ€μκ³Ό κ°λ€.
![image](https://user-images.githubusercontent.com/99963066/204142311-f659cd84-dfea-4265-ae1c-f7e3acc74645.png)
