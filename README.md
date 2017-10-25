# テクノロジー（藤原）10/25授業

```
()kogadoom:~/workspace $ [ ! -f ~/.ssh/id_rsa ] && ssh-keygen -t rsa
kogadoom:~/workspace $ 
kogadoom:~/workspace $ 
kogadoom:~/workspace $ [ ! -f ~/.ssh/id_rsa ] && ssh-keygen -t rsa
kogadoom:~/workspace $ ls ~/.ssh
authorized_keys  config  id_rsa  id_rsa.pub  known_hosts
kogadoom:~/workspace $  cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCuywwMaNIML/cq68Ktw7GSe3j45Ln9h1rwAVRT6+d+a7XPcpfceHW8TLTAJrdf7X6TfEkKZUsZvW25Vu4y1sixkhHAYBiZv44dRcMqqvxeC45+6/Rmd6z424ZRB7FnUzkD4Mzb2AMSgNetX4iQ/BOMJfw0rWBapUelEPZshC8XJjI78W4zR08VGozT3EfjF3biCG1Ky3ynhlCECkqmlaDG4C7I86Yf4CfSKu1OsSvp8gursOH6tGwx6YQzn02F7dZTiNdQNMdaLXggtRu394H5L3wioQtpmgMHUYtiPdejofJoR5ktHOm1f+HOo1UIDbJC9Kp49lklQI3Z3kCWtkc18vw3mw0G53qmg6vR0lQllU3NUJaiDVLr2E7BIyS2Zm7Cc2YcxqctM4Z9zyGrywCiAQ9Bt7SujS2c4XUCkYoqLgm50U8iG6ibGRMtt6V6tOV1A7ruTS6S7pZ5hjxa50BnDFBd+aSNmhXmTJG0+cEdz8wl5ROs6VImu2fJ9ddXUuIsvk1JjUkqy8+R95O0c3xEoZbwORexd1j3y1fjP5qHLht1yi9eaw0x5A+LACGD36pxgP7i3ZuSU5lEFvVpuQTCDMle4TTIGIOdyGj54/NYQz7xmDs2ru6uUhJNBU93vAA9kTHEYtGUZynvPvQrW5wLHC/IciLlKIYengrXfWahTw== kd1245397@st.kobedenshi.ac.jp
kogadoom:~/workspace $ ssh -T git@github.com
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
Hi kogatoshi! You've successfully authenticated, but GitHub does not provide shell access.
kogadoom:~/workspace $ ssh -T git@github.com
Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
Hi kogatoshi! You've successfully authenticated, but GitHub does not provide shell access.
kogadoom:~/workspace $ git clone
fatal: You must specify a repository to clone.

usage: git clone [<options>] [--] <repo> [<dir>]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    -n, --no-checkout     don't create a checkout
    --bare                create a bare repository
    --mirror              create a mirror repository (implies bare)
    -l, --local           to clone from a local repository
    --no-hardlinks        don't use local hardlinks, always copy
    -s, --shared          setup as shared repository
    --recurse-submodules[=<pathspec>]
                          initialize submodules in the clone
    -j, --jobs <n>        number of submodules cloned in parallel
    --template <template-directory>
                          directory from which templates will be used
    --reference <repo>    reference repository
    --reference-if-able <repo>
                          reference repository
    --dissociate          use --reference only while cloning
    -o, --origin <name>   use <name> instead of 'origin' to track upstream
    -b, --branch <branch>
                          checkout <branch> instead of the remote's HEAD
    -u, --upload-pack <path>
                          path to git-upload-pack on the remote
    --depth <depth>       create a shallow clone of that depth
    --shallow-since <time>
                          create a shallow clone since a specific time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --single-branch       clone only one branch, HEAD or --branch
    --no-tags             don't clone any tags, and make later fetches not to follow them
    --shallow-submodules  any cloned submodules will be shallow
    --separate-git-dir <gitdir>
                          separate git dir from working tree
    -c, --config <key=value>
                          set config inside the new repository
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

kogadoom:~/workspace $ git clone git@github.com:kogatoshi/lecture-1025.git
Cloning into 'lecture-1025'...
Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.
kogadoom:~/workspace $ git clone git@github.com:kogatoshi/project2-server-app.git
Cloning into 'project2-server-app'...
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
remote: Counting objects: 7, done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 7 (delta 0), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (7/7), done.
kogadoom:~/workspace $ pry
[1] pry(main)> puts"こんにちは"
こんにちは
=> nil
[2] pry(main)> print"こんにちは"
こんにちは=> nil
[3] pry(main)> p "こんにちは"
"こんにちは"
=> "こんにちは"
[4] pry(main)> message = "こんにちは"
=> "こんにちは"
[5] pry(main)> puts message
こんにちは
=> nil
[6] pry(main)> num = 123
=> 123
[7] pry(main)> puts num
123
=> nil
[8] pry(main)> message = "こんにちは"
=> "こんにちは"
[9] pry(main)> puts message.length
5
=> nil
[10] pry(main)> 1234
=> 1234
[11] pry(main)> 1234.class
=> Integer
[12] pry(main)> 1234 .class
=> Integer
[13] pry(main)> name = '古賀'
=> "古賀"
[14] pry(main)> puts

=> nil
[15] pry(main)> puts "#{}さん、こんにちは"
さん、こんにちは
=> nil
[16] pry(main)> puts "#{name}さん、こんにちは"
古賀さん、こんにちは
=> nil
[17] pry(main)> "\nさようなら\n"
=> "\nさようなら\n"
[18] pry(main)> a = 4; b = "9"
=> "9"
[19] pry(main)> a + b
TypeError: String can't be coerced into Integer
from (pry):19:in `+'
[20] pry(main)> a.to_s + b #=
=> "49"
[21] pry(main)> (a.to_s + b).class
=> String
[22] pry(main)> a + b.to_i #=                                                                                                                    
=> 13
[23] pry(main)> (a + b.to_i)
=> 13
[24] pry(main)> (a + b.to_i).class
=> Integer
[25] pry(main)> animals = ["いぬ","ネコ","ぞう"]
=> ["いぬ", "ネコ", "ぞう"]
[26] pry(main)> animals
=> ["いぬ", "ネコ", "ぞう"]
[27] pry(main)> animals[0]
=> "いぬ"
[28] pry(main)> animals[1]
=> "ネコ"
[29] pry(main)> animals[1] = "こうもり"
=> "こうもり"
[30] pry(main)> animals
=> ["いぬ", "こうもり", "ぞう"]
[31] pry(main)> animals[3]
=> nil
[32] pry(main)> animals.push
=> ["いぬ", "こうもり", "ぞう"]
[33] pry(main)> animals.push("くじら")
=> ["いぬ", "こうもり", "ぞう", "くじら"]
[34] pry(main)> animals.pop
=> "くじら"
[35] pry(main)> color[]
NameError: undefined local variable or method `color' for main:Object
from (pry):35:in `__pry__'
[36] pry(main)> color = []
=> []
[37] pry(main)> colors.empty?
NameError: undefined local variable or method `colors' for main:Object
Did you mean?  color
from (pry):37:in `__pry__'
[38] pry(main)> colors.length
NameError: undefined local variable or method `colors' for main:Object
Did you mean?  color
from (pry):38:in `__pry__'
[39] pry(main)> colors = ["赤","青","黄","ピンク"]
=> ["赤", "青", "黄", "ピンク"]
[40] pry(main)> colors.empty?
=> false
[41] pry(main)> colors.length
=> 4
[42] pry(main)> cd ~/workspace/lecture-1025
Error: Bad object path: "~/workspace/lecture-1025"
Failed trying to resolve: "~/workspace/lecture-1025"
Exception: #<SyntaxError: (eval):2: unknown regexp options - lctr>
[43] pry(main)> 
```