**[manjaro]**  
=====
manjaro是当前流行的linux发行版之一，它是由archlinux发展而来，用户友好的linux发行版，滚动更新，采用AUR仓库。    
        
        
**源**
=====
**1.排列镜像源，升级系统**      
```sudo pacman-mirrors -c China         
sudo pacman -Syyu```  
**2.加 Arch 国内源**    
sudo vi /etc/pacman.conf  
[archlinuxcn]       
SigLevel = Optional TrustedOnly     
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/$arch       
**3.导入GPG Key**    
```sudo pacman -S archlinuxcn-keyring```  
**4.之后可以从库中找到更多的软件了**   
如chrome、sougoupinyin、netease-loud-music
***
**中文输入法**   
据说欧洲人习惯不用输入法，因此不自带输入法，更没有中国本地化的中文输入法  
**以下以搜狗输入法为例**      
1、安装搜狗拼音、fcitx-im、fxitx-configtool(图形化界面）   
```pacman -S fcitx fcitx-sogoupinyin fcitx-im fcitx-configtool```   
2、修改（创建）配置文件`~/.xprofile`     
***
```export GTK_IM_MODULE=fcitx  
   export QT_IM_MODULE=fcitx   
   export XMODIFIERS="@im=fcitx"```   
    
