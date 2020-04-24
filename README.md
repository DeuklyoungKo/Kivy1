# Kivy Test

>## How to use conda
        conda install android

>## Virtual with Anaconda

* ### Anaconda virtual
        conda create -n Home python=3.7
        conda info --envs
        conda env remove -n Home

* ### Run virtual
        cd D:\Kivy\1\Home
        .\Scripts\activate

        conda activate Home
        conda deactivate

***
> ## Kivy Sample 
        python .\share\kivy-examples\demo\showcase\main.py

***
> ## Buildozer 

Link : [Kivy Buildozer](https://kivy.org/doc/stable/guide/packaging-android.html#buildozer, "Kivy Buildozer")   
Link : [Buildozer](https://github.com/kivy/buildozer, "Buildozer")

        sudo apt install python-pip
        pip install buildozer

        buildozer init

        # edit the buildozer.spec, then
        buildozer android debug deploy run

        buildozer android clean

        sudo apt-get install zlib1g-dev
        pip install Cython

        sudo apt install default-jre
        sudo apt install openjdk-8-jre-headless
        sudo apt install default-jre
        sudo apt install default-jdk
        sudo apt-get install unzip

        download Command line tools only at https://developer.android.com/studio

        # To set PATH
        export PATH=/home/ubuntu/.buildozer/android/platform/android-sdk/tools:/home/ubuntu/.buildozer/android/platform/android-sdk/tools/bin:$PATH
        source ~/.bashrc

        # To downgrade to openjdk-8-jre
        https://askubuntu.com/questions/1133216/downgrading-java-11-to-java-8


* ### To test 
        sdkmanager --list

        For those who struggled with installing Android Command Line Tools for Appium on Windows 10/x64 just do as following:

        Download latest Command line tools from android i.e. commandlinetools-win-6200805_latest.zip    
        Unzip the downloaded file   
        Create directory for storing commandline tools somewhere on your disk, with following path included: android/cmdline-tools/latest Basically when You unzip this Cmd line tools, just rename tools directory to latest and make sure You put this latest folder in android/cmdline-tools directory somewhere on your disk
        Create ANDROID_HOME environment variable for directory that stores the cmdline tools directory location like: C:\YourLocationWhereYouStoreTheDirectory\android\cmdline-tools\latest
        Create new entry in Path environment variable as %ANDROID_HOME%\bin

* ### Error : ModuleNotFoundError: No module named '_ctypes'
        # in Ubuntu
        sudo apt install libffi-dev 

        # in Redhat, Fedora
        sudo apt install libffi-devel


* ### Error : Could not find tools.jar. Please check that /usr/lib/jvm/java-8-openjdk-amd64 contains a valid JDK installation.
        https://blusky10.tistory.com/368


* ### CommandNotFoundError: Your shell has not been properly configured to use 'conda activate'.
        source ~/anaconda3/etc/profile.d/conda.sh
        conda activate Home


# Etc log

        curl –O https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh

        sha256sum Anaconda3-2020.02-Linux-x86_64.sh

        sudo chmod -R 775 anaconda3/
        sudo chown -R ubuntu.ubuntu anaconda3/


        vi ~/.bashrc
        source ~/.bashrc


***
***
# Mark Down Sample

## To emphasize text
* *single asterisks* - 기울임체
* _single underscores_ - 기울임체
* **double asterisks** - 굵은글씨체
* __double underscores__ - 기울임체/굵은글씨체
* ***triple underscores*** - 기울임체/굵은글씨체
* ~~cancelline~~ - 취소줄        

        *single asterisks* - 기울임체
        _single underscores_ - 기울임체
        **double asterisks** - 굵은글씨체
        __double underscores__ - 기울임체/굵은글씨체
        ***triple underscores*** - 기울임체/굵은글씨체
        ~~cancelline~~ - 취소줄

***
## Table
| 이름   | 설명  | 나이 |
| ----- | ---- | --- |
| 김태완  | 아빠  | 40 |
| 임선영  | 엄마  | 30 |
| 김민수  | 아들  | 2  |
        | 이름   | 설명  | 나이 |
        | ----- | ---- | --- |
        | 김태완  | 아빠  | 40 |
        | 임선영  | 엄마  | 30 |
        | 김민수  | 아들  | 2  |


* 리스트1
- 리스트2
- 서브 리스트1
* 서브리스트 2
* 서브리스트 2
* 서브리스트 2 
- 리스트3 
- 리스트3 
1. 순차 리스트1 
2. 순차 리스트2

***
## Table
### 테이블 구성
  * [1장](#chapter-1)
  * [2장](#chapter-2)
  * [3장](#chapter-3)

###### 1장 <a id="chapter-1"></a>
1장의 내용은.....

###### 2장 <a id="chapter-2"></a>
2장의 내용은.....

###### 3장 <a id="chapter-3"></a>
3장의 내용은.....

***
## Image
![Minion](http://ticketimage.interpark.com/Movie/still_image/V16/V1600651p_01.gif)   
![Alt text](https://i.pinimg.com/originals/04/83/d4/0483d4c162e86dc06f3fc86fbb5e2cee.jpg "Moon River")   
<img src="https://i.pinimg.com/236x/df/ca/5d/dfca5d5b8d028fe109ecf95f320a9cd7--cool-posters-sci-fi-movies.jpg" width="236px" height="470px" title="px(픽셀) 크기 설정" alt="The Time Machine"></img>   
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTjWdatOOPqznooi5w9rSgMO7vuyYSfqpQBhvQ4agJw_CVwhtVl&usqp=CAU" width="40%" title="px(픽셀) 크기 설정" alt="The Wonderful Wizard of Oz"></img>
***
## To change line
* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.___\\ 띄어쓰기
이렇게

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.   
이렇게

***
## To delete downloaded file
* ### 다운받은 모든 패키지 삭제
        sudo apt-get clean
* ### 다운받은 패키지 중에 옛버전만 삭제
        sudo apt-get autoclean
* ### 다운받은 패키지 중에 설치에 필요없는 패키지만 삭제
        sudo apt-get autoremove