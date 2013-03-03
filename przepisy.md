int main() {
  printf(''witaj świecie\n")
}
```c
kborkowska@p137-11:~$ ls~/.ssh/
bash: ls~/.ssh/: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/studpoz/kborkowska/.ssh/id_rsa): 
Created directory '/home/studpoz/kborkowska/.ssh'.
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/studpoz/kborkowska/.ssh/id_rsa.
Your public key has been saved in /home/studpoz/kborkowska/.ssh/id_rsa.pub.
The key fingerprint is:
27:67:0b:e9:7f:56:de:44:49:bc:69:00:e4:0d:cf:52 kborkowska@p137-11
The key's randomart image is:
+--[ RSA 2048]----+
|          .+.E.  |
|          . *. o |
|           o +o +|
|         .  .  =.|
|        S +   .. |
|       . * .  . .|
|        . .  o o |
|         .  o . .|
|          .o     |
+-----------------+
kborkowska@p137-11:~$ cat~/.ssh/id_rsa.pub
bash: cat~/.ssh/id_rsa.pub: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC16F5O2H89IDYeZozl3xhz+8y7BQHHEAVcZsBYByx4AMpOCgM8X6EakTkoqOn31A59h62ykkZntVCw9Hppm8CAS9CoGYWw5n6XT6p4Nut8Q+eZ4MK2C4iGvMH5nWYU/2fst26dndAKu7VMlEkB+DPrSgOQ4LxqYoibx4X9LLajXv2QTsQxsaCQQ/d+32by44+0ZVYXvPgFLToO1koEMUolq4kNH/53GV3tZ04vIn84cgmyAkvShSBSswCt/q8K0SZH5rhOa/1M2cMGy06gzy9hGPlFTkZP4VvHbk7FFoNUClvW4AfJ8G7sxPRLczn0vdr+klcxLWZoMYRAmQecOlvz kborkowska@p137-11
kborkowska@p137-11:~$ 
kborkowska@p137-11:~$ ~$cd tmp/
~: command not found
kborkowska@p137-11:~$ cd..
cd..: command not found
kborkowska@p137-11:~$ cd temp
bash: cd: temp: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ git clone git@github.com:kamilkab82/ti.git
Cloning into 'ti'...
The authenticity of host 'github.com (207.97.227.239)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? ^C
kborkowska@p137-11:~$ nano readme
kborkowska@p137-11:~$ git@github.com:kamilkab82/ti.git
bash: git@github.com:kamilkab82/ti.git: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ git@github.com:kamilkab82/ti.git
bash: git@github.com:kamilkab82/ti.git: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ git clone git@github.com:kamilkab82/ti.git
Cloning into 'ti'...
The authenticity of host 'github.com (207.97.227.239)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? y
Please type 'yes' or 'no': yes
Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
remote: Counting objects: 12, done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 12 (delta 1), reused 0 (delta 0)
Receiving objects: 100% (12/12), done.
Resolving deltas: 100% (1/1), done.
kborkowska@p137-11:~$ cd ti
kborkowska@p137-11:~/ti$ git mv JP.md przepisy.md
kborkowska@p137-11:~/ti$ ls
przepisy.md  README.md
kborkowska@p137-11:~/ti$ git push
Everything up-to-date
kborkowska@p137-11:~/ti$ ls
przepisy.md  README.md
kborkowska@p137-11:~/ti$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#  renamed:    JP.md -> przepisy.md
#
kborkowska@p137-11:~/ti$ git commit -m "zmana nazwy"
[master d4cef92] zmana nazwy
 Committer: Kamila Borkowska <kborkowska@p137-11.labpk.inf.ug.edu.pl>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 rename JP.md => przepisy.md (100%)
kborkowska@p137-11:~/ti$ git status
# On branch master
# Your branch is ahead of 'origin/master' by 1 commit.
#
nothing to commit (working directory clean)
kborkowska@p137-11:~/ti$ git push
Counting objects: 3, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 288 bytes, done.
Total 2 (delta 0), reused 0 (delta 0)
To git@github.com:kamilkab82/ti.git
   94cb8da..d4cef92  master -> master
kborkowska@p137-11:~/ti$ ls
przepisy.md  README.md
kborkowska@p137-11:~/ti$ ls
przepisy.md  README.md
kborkowska@p137-11:~/ti$ cd 
kborkowska@p137-11:~$ cd pobrane
bash: cd: pobrane: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~$ ls
Dokumenty  etc	mail  Muzyka  Obrazy  Pobrane  Publiczny  Pulpit  Szablony  ti	tmp  Wideo
kborkowska@p137-11:~$ cd Pobrane 
kborkowska@p137-11:~/Pobrane$ ls
kborkowska@p137-11:~/Pobrane$ ls
Sublime Text 2.0.1.tar.bz2
kborkowska@p137-11:~/Pobrane$ cd Pobrane
bash: cd: Pobrane: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~/Pobrane$ 
kborkowska@p137-11:~/Pobrane$ Sublime Text 2.0.1.tar.bz2
Sublime: command not found
kborkowska@p137-11:~/Pobrane$ jxvf Sublime\ Text\ 2.0.1.tar.bz2 
jxvf: command not found
kborkowska@p137-11:~/Pobrane$ jxvf Sublime\ Text\ 2.0.1.tar.bz2 
jxvf: command not found
kborkowska@p137-11:~/Pobrane$ tar jxvf Sublime\ Text\ 2.0.1.tar.bz2 
Sublime Text 2/
Sublime Text 2/Pristine Packages/
Sublime Text 2/Pristine Packages/Lisp.sublime-package
Sublime Text 2/Pristine Packages/TCL.sublime-package
Sublime Text 2/Pristine Packages/Text.sublime-package
Sublime Text 2/Pristine Packages/Default.sublime-package
Sublime Text 2/Pristine Packages/Java.sublime-package
Sublime Text 2/Pristine Packages/Graphviz.sublime-package
Sublime Text 2/Pristine Packages/User.sublime-package
Sublime Text 2/Pristine Packages/Ruby.sublime-package
Sublime Text 2/Pristine Packages/CSS.sublime-package
Sublime Text 2/Pristine Packages/Groovy.sublime-package
Sublime Text 2/Pristine Packages/SQL.sublime-package
Sublime Text 2/Pristine Packages/Erlang.sublime-package
Sublime Text 2/Pristine Packages/C++.sublime-package
Sublime Text 2/Pristine Packages/D.sublime-package
Sublime Text 2/Pristine Packages/AppleScript.sublime-package
Sublime Text 2/Pristine Packages/Batch File.sublime-package
Sublime Text 2/Pristine Packages/Theme - Default.sublime-package
Sublime Text 2/Pristine Packages/OCaml.sublime-package
Sublime Text 2/Pristine Packages/ASP.sublime-package
Sublime Text 2/Pristine Packages/XML.sublime-package
Sublime Text 2/Pristine Packages/Scala.sublime-package
Sublime Text 2/Pristine Packages/Textile.sublime-package
Sublime Text 2/Pristine Packages/ActionScript.sublime-package
Sublime Text 2/Pristine Packages/Language - English.sublime-package
Sublime Text 2/Pristine Packages/Lua.sublime-package
Sublime Text 2/Pristine Packages/Go.sublime-package
Sublime Text 2/Pristine Packages/RestructuredText.sublime-package
Sublime Text 2/Pristine Packages/C#.sublime-package
Sublime Text 2/Pristine Packages/Perl.sublime-package
Sublime Text 2/Pristine Packages/Markdown.sublime-package
Sublime Text 2/Pristine Packages/Vintage.sublime-package
Sublime Text 2/Pristine Packages/Color Scheme - Default.sublime-package
Sublime Text 2/Pristine Packages/Python.sublime-package
Sublime Text 2/Pristine Packages/Objective-C.sublime-package
Sublime Text 2/Pristine Packages/R.sublime-package
Sublime Text 2/Pristine Packages/Matlab.sublime-package
Sublime Text 2/Pristine Packages/Diff.sublime-package
Sublime Text 2/Pristine Packages/JavaScript.sublime-package
Sublime Text 2/Pristine Packages/ShellScript.sublime-package
Sublime Text 2/Pristine Packages/Regular Expressions.sublime-package
Sublime Text 2/Pristine Packages/LaTeX.sublime-package
Sublime Text 2/Pristine Packages/Haskell.sublime-package
Sublime Text 2/Pristine Packages/Clojure.sublime-package
Sublime Text 2/Pristine Packages/HTML.sublime-package
Sublime Text 2/Pristine Packages/Makefile.sublime-package
Sublime Text 2/Pristine Packages/Rails.sublime-package
Sublime Text 2/Pristine Packages/PHP.sublime-package
Sublime Text 2/Pristine Packages/YAML.sublime-package
Sublime Text 2/Icon/
Sublime Text 2/Icon/16x16/
Sublime Text 2/Icon/16x16/sublime_text.png
Sublime Text 2/Icon/128x128/
Sublime Text 2/Icon/128x128/sublime_text.png
Sublime Text 2/Icon/32x32/
Sublime Text 2/Icon/32x32/sublime_text.png
Sublime Text 2/Icon/48x48/
Sublime Text 2/Icon/48x48/sublime_text.png
Sublime Text 2/Icon/256x256/
Sublime Text 2/Icon/256x256/sublime_text.png
Sublime Text 2/lib/
Sublime Text 2/lib/python26.zip
Sublime Text 2/sublime_plugin.py
Sublime Text 2/sublime_text
Sublime Text 2/PackageSetup.py
kborkowska@p137-11:~/Pobrane$ cd Sublime Text2 
bash: cd: Sublime: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~/Pobrane$ cd S
bash: cd: S: Nie ma takiego pliku ani katalogu
kborkowska@p137-11:~/Pobrane$ cdS
No command 'cdS' found, did you mean:
 Command 'cdb' from package 'tinycdb' (main)
 Command 'cdo' from package 'cdo' (universe)
 Command 'cdi' from package 'cdo' (universe)
 Command 'cdv' from package 'codeville' (universe)
 Command 'cdw' from package 'cdw' (universe)
 Command 'cdp' from package 'irpas' (multiverse)
 Command 'cd5' from package 'cd5' (universe)
cdS: command not found
kborkowska@p137-11:~/Pobrane$ cd Sublime\ Text\ 2
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ./sublime_text
bash: ./sublime_text: Brak dostępu
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ./sublime_text
bash: ./sublime_text: Brak dostępu
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ chmod 755 sublime_text
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ls-l
ls-l: command not found
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ chmod 755 sublime_text 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ls -l
razem 7820
drwxrwxr-x 7 kborkowska studpoz       0 lip 14  2012 Icon
drwxrwxr-x 2 kborkowska studpoz       0 lip 14  2012 lib
-rw-r--r-- 1 kborkowska studpoz    4205 lip 14  2012 PackageSetup.py
drwxrwxr-x 2 kborkowska studpoz       0 lip 14  2012 Pristine Packages
-rw-r--r-- 1 kborkowska studpoz   10838 lip 14  2012 sublime_plugin.py
-rwxr-xr-x 1 kborkowska studpoz 7972576 lip 14  2012 sublime_text
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ >^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ cd ..
kborkowska@p137-11:~/Pobrane$ cd Sublime\ Text\ 2
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ls -l
razem 7820
drwxrwxr-x 7 kborkowska studpoz       0 lip 14  2012 Icon
drwxrwxr-x 2 kborkowska studpoz       0 lip 14  2012 lib
-rw-r--r-- 1 kborkowska studpoz    4205 lip 14  2012 PackageSetup.py
drwxrwxr-x 2 kborkowska studpoz       0 lip 14  2012 Pristine Packages
-rw-r--r-- 1 kborkowska studpoz   10838 lip 14  2012 sublime_plugin.py
-rwxr-xr-x 1 kborkowska studpoz 7972576 lip 14  2012 sublime_text
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ./sublime_text 
joikijpi6yhrt6fgkborkowska@p137-11:~/Pobrane/Sublime Text 2$ joikijpi6yhrt6fg^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ./sublime_text 
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ DGSGS
DGSGS: command not found
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ^C
kborkowska@p137-11:~/Pobrane/Sublime Text 2$ ./sublime_text 
