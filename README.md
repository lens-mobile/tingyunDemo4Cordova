# tingyunDemo4Cordova
## 1.配置依赖
### 1)打开platform/android/目录下的build.gradle，在buildscript和allprojects添加听云仓库
```
buildscript {
    repositories {
        google()
        jcenter()
        maven { url "http://nexus2.tingyun.com/nexus/content/repositories/snapshots/" }
    }
    allprojects {
    repositories {
        google()
        jcenter()
        maven { url "http://nexus2.tingyun.com/nexus/content/repositories/snapshots/" }
    }
```
在dependencies中添加以下代码：
```
classpath 'com.networkbench.newlens.agent.android:agent-gradle-plugin:2.14.4'
```
### 2)打开platform/android/app/下的build.gradle,添加代码：
```
apply plugin: 'newlens'
```

## 2.初始化听云
## 3.cordova webview嵌码
