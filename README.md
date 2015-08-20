Push Notifications Demo for Android
-----------------------------------

# Refrence

    More details at http://tokudu.com/2010/how-to-implement-push-notifications-for-android

# Tip

    1) clone AndroidPushNotificationDemo

        $ https://github.com/tokudu/AndroidPushNotificationsDemo.git

    2) 转换成AndroidStudio可以运行的版本（默认clone下来只能使用eclipse运行）

        Eclipse工程转到studio的过程参考如下博客：
        http://www.cnblogs.com/ct2011/p/4183553.html

        注：其中在build.gradle这个文件中，修改版本要针对你自己安装的studio版本，
            不要完全按照这个博客来，比如我的sdk编译版本：
            Android/Project -> Gradle Scripts -> build.gradle

            修改如下：
            buildscript {
                repositories {
                    mavenCentral()
                }
                dependencies {
                    //classpath 'com.android.tools.build:gradle:0.12.+'
                    classpath 'com.android.tools.build:gradle:1.2.3'
                }
            }

            android {
                //compileSdkVersion 8
                //buildToolsVersion "20.0.0"
                compileSdkVersion 22
                buildToolsVersion "22.0.1"

                ...........
            }

        另：
            修改了默认的订阅主题:
            将tokudu/设备id  ->   levis

# 仓库改名

    # update the remote url in your local repository :
    $ git remote set-url origin git@github.com/yyjinlong/PushAndroid.git
