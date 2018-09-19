# -ssh

1、第一步：创建账号、邮箱

     git config --global user.name "hrong"
     git confit --global user.email "hrong@git.com"
     
  查看账号跟邮箱是否创建好 
  
     git config --global user.name  /git config --global user.email
  
2、检查是否有ssh   

    cd ~/.ssh
  
  >若报错  类似这样的：  cd: /c/Users/Administrator/.ssh: No such file or directory 说明无ssh
  </br>生成秘钥  ssh-keygen -t rsa -C "hrong@git.com"   若不设置密码，直接三个回车
  
  >若无报错
  </br>ls 
  </br>可以看到有.pub为后缀的文件名，说明已经有ssh了
  
3、 查看ssh
  >cat id_rsa.put
  
4、添加ssh  
  打开gitlab，在设置内，添加ssh（cat查看到的ssh）就可以了
  
  
