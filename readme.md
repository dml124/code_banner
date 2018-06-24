```
                                **           **                                                
                               /**          /**                                                
           *****   ******      /**  *****   /**       ******   *******  *******   *****  ******
          **///** **////**  ****** **///**  /******  //////** //**///**//**///** **///**//**//*
         /**  // /**   /** **///**/*******  /**///**  *******  /**  /** /**  /**/******* /** / 
         /**   **/**   /**/**  /**/**////   /**  /** **////**  /**  /** /**  /**/**////  /**   
         //***** //****** //******//******  /****** //******** ***  /** ***  /**//******/***   
          /////   //////   //////  //////   /////    //////// ///   // ///   //  ////// ///    
```

# code_banner
总结一些程序员常用banner，

## 女神
```py
banner = """
.================================================================.
||                            title                             ||
||       " << g_softname << " v" << g_version << "              ||
|'--------------------------------------------------------------'|
||                                         -- main instructions ||
|'=============================================================='|
||                                .::::.                        ||
||                              .::::::::.                      ||
||                              :::::::::::                     ||
||                              ':::::::::::..                  ||
||                              .:::::::::::::::'               ||
||                                '::::::::::::::.`             ||
||                                  .::::::::::::::::.'         ||
||                                .::::::::::::..               ||
||                              .::::::::::::::''               ||
||                   .:::.       '::::::::''::::                ||
||                 .::::::::.      ':::::'  '::::               ||
||                .::::':::::::.    :::::    '::::.             ||
||              .:::::' ':::::::::. :::::.     ':::.            ||
||            .:::::'     ':::::::::.::::::.      '::.          ||
||          .::::''         ':::::::::::::::'       '::.        ||
||         .::''              '::::::::::::::'        ::..      ||
||      ..::::                  ':::::::::::'         :'''`     ||
||   ..''''':'                    '::::::.'                     ||
|'=============================================================='|
||                                       helianghit@foxmail.com ||
||                                https://github.com/HeLiangHIT ||
'================================================================'
"""
print(banner)

# 动态打印banner
def animate_banner(tick=0.001):
    import time
    for c in banner:
        time.sleep(tick)
        print(c, end="")
```

## 佛主
```py
banner = """
                       _ooOoo_                        
                      o8888888o                       
                      88" . "88                       
                      (| ^_^ |)                       
                      O\  =  /O                       
                   ____/`---'\____                    
                 .'  \\|     |//  `.                  
                /  \\|||  :  |||//  \                 
               /  _||||| -:- |||||-  \                
               |   | \\\  -  /// |   |                
               | \_|  ''\---/''  |   |                
               \  .-\__  `-`  ___/-. /                
             ___`. .'  /--.--\  `. . ___              
           ."" '<  `.___\_<|>_/___.'  >'"".           
         | | :  `- \`.;`\ _ /`;.`/ - ` : | |          
         \  \ `-.   \_ __\ /__ _/   .-` /  /          
   ========`-.____`-.___\_____/___.-`____.-'========  
                        `=---='                       
   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
           佛祖保佑       永不宕机     永无BUG           
"""
print(banner)

# 动态打印banner
def animate_banner(tick=0.001):
    import time
    for c in banner:
        time.sleep(tick)
        print(c, end="")
```

## 文字banner生成
### 网页版
1. 打开网页： http://www.network-science.de/ascii/
2. 输入文字比如`code banner`，选择字体比如graffiti，点击do it! 等待几秒。
3. 输出内容后拷贝：
```
                 .___       ___.                                      
  ____  ____   __| _/____   \_ |__ _____    ____   ____   ___________ 
_/ ___\/  _ \ / __ |/ __ \   | __ \\__  \  /    \ /    \_/ __ \_  __ \
\  \__(  <_> ) /_/ \  ___/   | \_\ \/ __ \|   |  \   |  \  ___/|  | \/
 \___  >____/\____ |\___  >  |___  (____  /___|  /___|  /\___  >__|   
     \/           \/    \/       \/     \/     \/     \/     \/       

```
或者选择3-d生成如下类型banner，设置长度为100，居中
```
                                **           **                                                
                               /**          /**                                                
           *****   ******      /**  *****   /**       ******   *******  *******   *****  ******
          **///** **////**  ****** **///**  /******  //////** //**///**//**///** **///**//**//*
         /**  // /**   /** **///**/*******  /**///**  *******  /**  /** /**  /**/******* /** / 
         /**   **/**   /**/**  /**/**////   /**  /** **////**  /**  /** /**  /**/**////  /**   
         //***** //****** //******//******  /****** //******** ***  /** ***  /**//******/***   
          /////   //////   //////  //////   /////    //////// ///   // ///   //  ////// ///    
```

### 本地安装
网页版有时候太慢了，该工具开源，可以下载到本地编译安装。依次执行如下命令安装工具：
```shell
wget ftp://ftp.figlet.org/pub/figlet/program/unix/figlet-2.2.5.tar.gz
tar -zxvf figlet-2.2.5.tar.gz
cd figlet-2.2.5
make && make install
```
> 该工具已解压到目录 [./figlet/](./figlet/) 下，可以直接在里面编译安装。


之后可以执行 `figlet "code banner"` 生成对应的banner如下
```
               _        _
  ___ ___   __| | ___  | |__   __ _ _ __  _ __   ___ _ __
 / __/ _ \ / _` |/ _ \ | '_ \ / _` | '_ \| '_ \ / _ \ '__|
| (_| (_) | (_| |  __/ | |_) | (_| | | | | | | |  __/ |
 \___\___/ \__,_|\___| |_.__/ \__,_|_| |_|_| |_|\___|_|
```
也可以`figlet 'c o d e   b a n n e r'`控制间距：
```
                    _            _
  ___    ___     __| |   ___    | |__     __ _   _ __    _ __     ___   _ __
 / __|  / _ \   / _` |  / _ \   | '_ \   / _` | | '_ \  | '_ \   / _ \ | '__|
| (__  | (_) | | (_| | |  __/   | |_) | | (_| | | | | | | | | | |  __/ | |
 \___|  \___/   \__,_|  \___|   |_.__/   \__,_| |_| |_| |_| |_|  \___| |_|
```
更多使用[查看帮助](http://www.figlet.org/)：
```
Usage: figlet [ -cklnoprstvxDELNRSWX ] [ -d fontdirectory ]
              [ -f fontfile ] [ -m smushmode ] [ -w outputwidth ]
              [ -C controlfile ] [ -I infocode ] [ message ]
```
可以到 http://www.figlet.org/examples.html 参考字体将自己喜欢的字体下载后用于生成固定风格的banner。比如font目录下：
下载字体后可以指定字体`figlet -d ./font -f alligator.flf -w 120 'code banner'`
```
      ::::::::  :::::::: ::::::::: ::::::::::        :::::::::     :::    ::::    :::::::    ::::::::::::::::::::::
    :+:    :+::+:    :+::+:    :+::+:               :+:    :+:  :+: :+:  :+:+:   :+::+:+:   :+::+:       :+:    :+:
   +:+       +:+    +:++:+    +:++:+               +:+    +:+ +:+   +:+ :+:+:+  +:+:+:+:+  +:++:+       +:+    +:+
  +#+       +#+    +:++#+    +:++#++:++#          +#++:++#+ +#++:++#++:+#+ +:+ +#++#+ +:+ +#++#++:++#  +#++:++#:
 +#+       +#+    +#++#+    +#++#+               +#+    +#++#+     +#++#+  +#+#+#+#+  +#+#+#+#+       +#+    +#+
#+#    #+##+#    #+##+#    #+##+#               #+#    #+##+#     #+##+#   #+#+##+#   #+#+##+#       #+#    #+#
########  ######## ######### ##########        ######### ###     ######    #######    #################    ###
```
> 一些比较喜欢的字体： block.flf/bulbhead.flf/computer.flf/alligator.flf/doh.flf/isometric1.flf/isometric2.flf/isometric3.flf/isometric4.flf/larry3d.flf/lean.flf/nancyj-fancy.flf/ogre.flf/pebbles.flf/puffy.flf/roman.flf/small.flf/smkeyboard.flf/tinker-toy.flf/univers.flf

## 图片banner生成





