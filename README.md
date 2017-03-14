# android-tips-tricks-cn

一些很不错的Android开发技巧,这个项目翻译自 [android-tips-tricks](https://github.com/nisrulz/) 去掉了一些我认为不重要的,对我使用过的东东做了评价,同时翻译了一些自己没有注意到的知识点的文章。

###  :heart: star 支持一下

[![GitHub stars](https://img.shields.io/github/stars/cctanfujun/android-tips-tricks-cn.svg?style=social&label=Star)](https://github.com/cctanfujun/android-tips-tricks-cn) [![GitHub forks](https://img.shields.io/github/forks/cctanfujun/android-tips-tricks-cn.svg?style=social&label=Fork)](https://github.com/cctanfujun/android-tips-tricks-cn/fork) [![GitHub watchers](https://img.shields.io/github/watchers/cctanfujun/android-tips-tricks-cn.svg?style=social&label=Watch)](https://github.com/cctanfujun/android-tips-tricks-cn) [![GitHub followers](https://img.shields.io/github/followers/cctanfujun.svg?style=social&label=Follow)](https://github.com/cctanfujun/android-tips-tricks-cn)  
  

欢迎协作

###***了解你的工具***

####***Android Studio***

+ **使用快捷键**
  
  **完整的快捷键指南 :  [MacOSX](https://resources.jetbrains.com/assets/products/intellij-idea/IntelliJIDEA_ReferenceCard_mac.pdf) | [Linux/Win](https://resources.jetbrains.com/assets/products/intellij-idea/IntelliJIDEA_ReferenceCard.pdf)**

+ **使用更有效率的插件**
  1. [KeyPromoter](https://plugins.jetbrains.com/plugin/4455)
      
    快捷键提示插件 -- 试用了一下,就是你点击的时候有些按钮会出来提示框告诉你这个的快捷键是什么以及你使用的次数，还不错，目的就是让你进行键盘流操作。

  1. [String Manipulation](https://plugins.jetbrains.com/plugin/2162)

    提供 Action 转换大小写什么的,感觉想不起来用。
        
  1. [Lines Sorter](https://plugins.jetbrains.com/plugin/5919)

    Add Sort Lines action in Edit menu to sort selected lines or whole file if selection is empty.
  
  1. [Findbugs](https://plugins.jetbrains.com/plugin/3847?pr=idea)

    静态代码审查工具
  
  1. [Sonar Lint](https://plugins.jetbrains.com/plugin/7973)

    也是个代码审查工具，检查可能出现的bug
  
  1. [Checkstyles](https://plugins.jetbrains.com/plugin/1065)

    代码风格管理的插件
  
  1. [ADB Idea](https://plugins.jetbrains.com/plugin/7380)

    增加了例如卸载，重启App的功能
  
  1. [Exynap](https://plugins.jetbrains.com/androidstudio/plugin/8600-exynap)

    这个玩意挺NB的输入个大概就能帮你写代码。其中的bind view 挺好用的。

  1. [Dagger IntelliJ Plugin](https://github.com/square/dagger-intellij-plugin)

    Dagger的可视化辅助工具
  
  1. [JVM Debugger Memory View](https://plugins.jetbrains.com/idea/plugin/8537-jvm-debugger-memory-view)
  
    可以调试JVM的一些细节，讲真我用的不多

+ **在 Android Studio 中使用 Live Templateso**
  
  + `newInstance` - 在Fragment中生成 `newInstance` 方法
  + `Toast` - 生成 `Toast.makeText(context, "", Toast.LENGTH_SHORT).show();`
  + `fbc` - 生成 findViewById
  + `const` - 定义一个 android style int 常量
  + `logd` - 生成 `Log.d(TAG, "");`
  + `logm` - Log 当前方法名称和参数
  + `logr` - Log 当前方法结果
  + `logt` - 当前类生成 log tag
  + `psf` - public static final
  + `sout` - 打印一个字符串到 System.out
  + `soutm` - 打印当前类名和方法到 System.out
  + `soutp` - 打印方法参数和返回值到 System.out
  + `visible` - 设置 view VISIBLE
  + `gone` - 设置 view GONE
  + `noInstance` - private 构造方法

  [Comprehensive list of all Live Templates in Android Studio](https://github.com/keyboardsurfer/idea-live-templates) 这个库有很多的自定义模版

+ **Android Studio 的自动完成**

  Android Studio/IntelliJ 可以帮你自动完成一些代码
  
  + `<expr>.null` 转换成 `if(<expr> == null)`
  + `<expr>.notnull` 转换成 `if(<expr> != null)`
  + `<expr>.var` 转换成 `T name = <expr>`
  + `<expr>.field` 会自动生成一个全局变量 `field = <expr>`
  + `<ArrayExpr>.for` 转换成 `for(T item : <Arrayexpr>)`
  + `<ArrayExpr>.fori` 转换成 `for(int i = 0; i < <Arrayexpr>.length; i++)`
  + `<ArrayExpr>.forr` 转换成 `for(int i = <Arrayexpr>.length - 1; i > 0 ; i--)`

  完整的转换列表参见  **Settings → Editor → Postfix Templates**

+ **使用黑色主题**

  虽然是个人爱好，反正我觉得使用白色主题好瞎眼啊

+ **别使用小字体**

  给你的 Android Studio 选择一个合适的字体，作者推荐使用[Menlo font](https://en.wikipedia.org/wiki/Menlo_(typeface)) 反正我觉得mac的字体就挺好的，在linux上开发已经觉得不顺眼了.

+ **使用一个 code style**
  
  你应该使用一个标准的编码风格，它可以是：
    + [AOSP Codestyle](https://source.android.com/source/code-style.html)
    + [Square IntelliJ Codestyle](https://github.com/square/java-code-styles)
  
  表示在编码风格这一块自己确实有待规范^^

+ **使用 [Embedded Terminal inside Android Studio](https://www.jetbrains.com/help/idea/2016.2/working-with-embedded-local-terminal.html)**

+ **使用 Memory/Network/CPU Monitor 检测你的 code/app**

+ **[配置 Android Studio](https://medium.com/google-developer-experts/configuring-android-studio-4aa4f54f1153#.rq0z6qlaq)**
  
  这个可以看下,文章提到的我是早就配置过了

####***模拟器***

  + [Genymotion](https://www.genymotion.com/) 曾经我最喜欢的模拟器，貌似收费了，现在x86的模拟器也挺快的了。
  + [Intel Emulator bundled in SDK Manger](https://developer.android.com/studio/run/emulator.html)

####***[Vysor](http://www.vysor.io/)***
  
  简单说就是显示你连上的真机,也就在你做演示的时候有些用处，而且我一连上手机就自己跳出来，各位自己使用评价吧！

####***[DeskDock](https://play.google.com/store/apps/details?id=com.floriandraschbacher.deskdock.free)***
    
  不但能展示还可以控制你的Android设备.[免费版本](https://play.google.com/store/apps/details?id=com.floriandraschbacher.deskdock.free) 可以使用电脑鼠标, [收费版本](https://play.google.com/store/apps/details?id=com.floriandraschbacher.deskdock.pro) 可以使用电脑键盘. 你可以手不离开键盘进行测试.

  -

###***编码时候的更优选择***

  + **使用 OkHttp 替代 HttpUrlConnect**

  HttpUrlConnect 有一些bug [quite some bugs](https://android-developers.blogspot.in/2011/09/androids-http-clients.html). [Okhttp](https://square.github.io/okhttp/) 优雅的解决了他们. [[Reference Link]](https://corner.squareup.com/2013/05/announcing-okhttp.html)

  + **按照如下方式使用本地 `aar` [[Stackoverflow Ref](http://stackoverflow.com/a/28816265/2745762)]**
  ```gradle
        dependencies {
           compile(name:'nameOfYourAARFileWithoutExtension', ext:'aar')
         }
        repositories{
              flatDir{
                      dirs 'libs'
               }
         }

  ```

  + **使用 [Pidcat](https://github.com/JakeWharton/pidcat) 获得更好的阅读体验**
  
  这个不错，不过我没找到一个命令参数表，就只关注我想要关注的 log
    
  + **使用版本控制系统(VCS) 例如 [Git](https://git-scm.com/)**

  + **使用 [ClassyShark](https://github.com/google/android-classyshark)**

  可以分析Android Apk很不错

  + **使用 [Stetho](https://github.com/facebook/stetho)**
  
  Facebook 出品，非常不错的工具，可以在 Chrome 中看到网络请求，调试数据库和SharePreference,和 Okhttp搭配使用更好，我配合urlconnection使用不生效，原因不明。
  

  + **使用 [Battery Historian](https://github.com/google/battery-historian)**

  使用"bugreport"分析耗电

  + **总是使用固定的版本号 例如 "24.2.0"**

    版本依赖时候避免使用 `+`
      + 防止api变更.
      + 编译的时候不会请求网络检查版本.

  + **使用 [Handler 替代 TimerTask](http://www.mopri.de/2010/timertask-bad-do-it-the-android-way-use-a-handler/)**
  
  这篇文章可以看一下，作者说在一些设备上 Timer 不工作但是原因不明，作者说的使用 Handler 替代 Timer 确实是对的，我们商店有一段时间anr很多，后来发现和Timer相关。
  
  + **[Google Play 的开发者账户不要使用你的个人邮箱](https://www.reddit.com/r/Android/comments/2hywu9/google_play_only_one_strike_is_needed_to_ruin_you/)**
  
  + **使用 Vectors 替代 PNG**

  如果你 **确实** 要用png, 可以使用 [TinyPNG](https://tinypng.com) 压缩.

  + **使用 proguard**

  ```gradle
      android {
        ...
        buildTypes {
            release {
                minifyEnabled true
                proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
            }
        }
    }
  ```
  
  + **使用 shrinkResources**

  ```gradle
      android {
        ...
        buildTypes {
            release {
                shrinkResources true
                minifyEnabled true
                ...
            }
        }
      }
  ```
  
  shrinkResources 是把你没用到的文件用一个很小的文件替换，我觉得要是你发现了那个文件确实没啥用，你还是删除了吧。

  + **[模拟 app 在后台被杀死](https://twitter.com/Jahnold/status/759775495655333888),  在终端运行**
  
  `adb shell am kill`

  + **参考 [降低 gradle 内存又加快构建](https://medium.com/@skaliakoudas/decreasing-build-times-by-decreasing-gradle-memory-requirements-7fcafc6d98ea#.otnm0ofb6)**
  
  译文见[降低 gradle 内存又加快构建](http://tanfujun.com/2017/03/13/%E9%99%8D%E4%BD%8E-gradle-%E5%86%85%E5%AD%98%E5%8F%88%E5%87%8F%E5%B0%91%E6%9E%84%E5%BB%BA%E6%97%B6%E9%97%B4-%E8%AF%91/)  
  
  ```gradle
      Gradle memory >= Dex memory + 1Gb
  ```

  + **使用 ndk 的时候注意自己分割 abi**
  
  ```gradle
      defaultConfig {
          ...

          ndk {
            abiFilters "armeabi", "armeabi-v7a", "mips", "x86"
          }
        }

      //Split into platform dependent APK
        splits {
          abi {
            enable true
            reset()
            include 'armeabi', 'armeabi-v7a', 'mips', 'x86' //select ABIs to build APKs for
            universalApk false //generate an additional APK that contains all the ABIs
          }
        }

        // map for the version code
        project.ext.versionCodes = ['armeabi': 1, 'armeabi-v7a': 2, 'mips': 5, 'x86': 8]

        // Rename with proper versioning
        android.applicationVariants.all { variant ->
          // assign different version code for each output
          variant.outputs.each { output ->
            output.versionCodeOverride =
                project.ext.versionCodes.get(output.getFilter(com.android.build.OutputFile.ABI), 0) *
                    1000000 +
                    android.defaultConfig.versionCode
          }
        }
  ```

  + **学习一些架构例如 MVP 或者 Clean架构**

  + **尝试理解 TDD (测试驱动开发)**

  + **强制重新下载 dependencies**

  ```gradle
      ./gradlew --refresh-dependencies
  ```
  + **gradle 中跳过某个task**

      下面的例子是跳过 `javaDoc` 这个任务

      ```gradle
      ./gradlew clean build -x javaDoc
      ```
  
  + **为每个子项目的脚本配置同名 gradle 构建文件**

      settings.gradle 中设置

      ```gradle
      rootProject.children.each{
        it.buildFileName = it.name + '.gradle'
      }
      ```

      **[更多的Gradle技巧](https://github.com/shekhargulati/gradle-tips)**

  + **记住 DRY**
    
  DRY = Do not Repeat Yourself

  + **[按照功能分包](https://medium.com/the-engineering-team/package-by-features-not-layers-2d076df1964d)**
  
  一开始我们也是按照层去分包的，很坑爹。按照功能分可能你不是很好区分在哪个功能中，不过也比你按照层区分要好找很多。

  + **[学习依赖原理](http://crushingcode.co/the-curious-case-of-dependency-conflicts/)**

     有利于你学习解决一些依赖冲突. [官方参考](https://docs.gradle.org/current/dsl/org.gradle.api.artifacts.ResolutionStrategy.html)

  + **给你没发布的版本使用不同包名**
  
  ```gradle
        android {
            buildTypes {
                debug {
                    applicationIdSuffix '.debug'
                    versionNameSuffix '-DEBUG'
                }

                release {
                    // ...
                }
            }
        }
  ```

  + **[找出并解决你的内存泄露](http://blog.nimbledroid.com/2016/09/06/stop-memory-leaks.html)**

  + **[小心使用 `@android:color/transparent`](https://android.jlelse.eu/android-dev-tip-3-99da754151ad#.clbqzz3zh)**

  + **[遵循标准的资源命名](http://jeroenmols.com/blog/2016/03/07/resourcenaming/)**

  + **build.gradle 中使用自定义任务**

  Android使用Gradle构建，这实际上可以很容易做些自动化的东西。[实用的 Gradle 脚本](https://www.reddit.com/r/androiddev/comments/3ig3gm/show_us_your_gradle_tasks)

  + **给你的Android项目使用合适的 .gitignore, [Check it here](/android.gitignore)**

  + **[使用 LeakCanary 分析你的app](https://github.com/square/leakcanary)**

  + **使用 Android Studio 2.3 加速 gradle 构建+**
      
    + 切换到 gradle 3.3

        执行下面的代码升级你的 gradle wrapper

        ```bash
        ./gradlew wrapper --gradle-version 3.3 --distribution-type all
        ```
    
    + 全局 `gradle.properties` 如下设置

        ```
        android.enableBuildCache=true
        ```
    
    这个命令我测试了，不好使啊！直接改wrapper里面引用就行。

  + **停止 gradle 构建进程**

    ```bash
        ./gradlew -stop
    ```
    
  + **开启 gradle 自动下载sdk**

      全局`gradle.properties`如下设置

    ```
      android.builder.sdkDownload=true
    ```

    > 实验性功能 [[Bug Ref]](https://code.google.com/p/android/issues/detail?id=212309)

  + **`jcenter()`和 `mavenCentral()`不用同时依赖`**

  JCenter 是 MavenCentral 的超集. [[参考]](https://twitter.com/molsjeroen/status/791606774210199553)

  + **这样清除 gradle 缓存**

    + `~/.gradle/caches/` 删除 `cache` 文件夹
    + 打开 SDK Manager 重新同步 support libs 和 google play services
    + re-sync  project
    + 搞定

  + **给你的 adb 设置别名** [[Ref Link]](https://medium.com/@jonfhancock/bash-your-way-to-better-android-development-1169bc3e0424#.8zcc4m5ch)

    以下的 **Aliases** 可以被添加到 `~/.bashrc` 或者 `~/.zshrc` ，看起来不错

|Alias|Usage
|---|---|
|`alias screenshot="adb exec-out screencap -p > screen-$(date -j "+%s").png"`|`screenshot`|
|`alias startintent="adb devices | tail -n +2 | cut -sf 1 | xargs -I X adb -s X shell am start $1"`|`startintent https://twitter.com/nisrulz`|
|`alias apkinstall="adb devices | tail -n +2 | cut -sf 1 | xargs -I X adb -s X install -r $1"`|`apkinstall ~/Desktop/DemoApp.apk`|
|`alias rmapp="adb devices | tail -n +2 | cut -sf 1 | xargs -I X adb -s X uninstall $1"`|`rmapp com.example.demoapp`|
|`alias clearapp="adb devices | tail -n +2 | cut -sf 1 | xargs -I X adb -s X shell pm clear $1"`|`clearapp com.example.demoapp`|

  + **设置含有 `//STOPSHIP` 时候编译失败** [[Ref Link]](https://www.reddit.com/r/androiddev/comments/5c8b0a/i_know_android_studio_allows_you_to_make_custom/d9uhdzt/)

      启用这个功能 `//STOPSHIP` 失败功能，  `build.gradle` 如下设置

      ```gradle
      android {
      ...
          lintOptions {
              abortOnError true
              fatal 'StopShip'
          }
      }
      ```
  `//STOPSHIP` 注释也会导致编译失败。
  
  >  在 Android Studio `Preferences` > `Editor` > `Code Style` > `Inspections`, 可以控制这个功能
  

  + **使用 `adb install -g` 安装并授予manifest中的全部权限** [[More Info]](https://developer.android.com/studio/command-line/adb.html)

  + **使用 [`alfi`](https://github.com/cesarferreira/alfi) 查找一个库的依赖**

  >[Gradle, Please](gradleplease.appspot.com) 的命令行版本.

    
    + 执行

        ```bash
        alfi name_of_library
        ```
    
    + 复制结果
    + 粘贴到 build.gradle

  + **使用 [`dryrun`](https://github.com/cesarferreira/dryrun) 直接测试一个库**

    + 运行

    ```bash
        dryrun REMOTE_GIT_URL
    ```
    
    表示还得下各种gradle版本，也就那么回事，不见得多快。
  
  + **控制台直接输入单元测试结果** [[Ref Link]](https://medium.com/@cesarmcferreira/mastering-the-terminal-side-of-android-development-e7520466c521#.1cw4bto7f)

      > 控制台输出单元测试结果小技巧.

      ```gradle
      android {
          ...
          testOptions.unitTests.all {
            testLogging {
              events 'passed', 'skipped', 'failed', 'standardOut', 'standardError'
              outputs.upToDateWhen { false }
              showStandardStreams = true
            }
          }
        }
      ```
  
  + **离线模式编译更快** [[Ref Link]](https://medium.com/@cesarmcferreira/mastering-the-terminal-side-of-android-development-e7520466c521#.1cw4bto7f)

    > `--offline` 总是从cache运行, 离线模式不会访问网络.没有缓存会编译失败.

    + 给你的Debug加速:

        ```gradle
        ./gradlew assembleDevelopDebug --offline
        ```
    
    + 给你的单元测试加速:

        ```gradle
        ./gradlew test --offline
        ```
  
  + **使用一个抽象 [Logger](https://github.com/nisrulz/android-tips-tricks/blob/develop/Logger.java) 类**

  + **如果你想自动初始化你的库 Content Provider** [[Read how Firebase does it - Ref Link]](https://firebase.googleblog.com/2016/12/how-does-firebase-initialize-on-android.html)
  
  译文[自动初始化你的库](http://tanfujun.com/2017/03/13/%E8%87%AA%E5%8A%A8%E5%88%9D%E5%A7%8B%E5%8C%96%E4%BD%A0%E7%9A%84%E5%BA%93-%E8%AF%91/)

  + **使用 `"android:extractNativeLibs:false"` 在 `<application>` 减小包体积** [[Ref Link]](https://medium.com/@wkalicinski/smallerapk-part-8-native-libraries-open-from-apk-fc22713861ff#.bajqmlshi)
  
  这个属性是6.0开始的属性，告诉系统你不用把apk解压缩出来了，但是so不能被压缩，so 需要zipalign对齐，这个步骤不是自动的，我觉得慎用。

  + **选择执行一个特定方法** [[Ref Link]](https://twitter.com/tasomaniac/status/820019068140945408)

    ![Image](https://raw.githubusercontent.com/nisrulz/android-tips-tricks/develop/img/selectiverun.gif)

  + **你收到过Google Play 违反政策的邮件吗? 别担心给你的app生成隐私策略** [[Ref ink]](https://medium.com/@ali.muzaffar/did-you-get-one-of-these-google-play-developer-policy-violation-emails-6c529ceb082d#.f10upj3fy)


###*** UI/UX 相关***

+ **移动**
  + Material Design 使用的是现实风格的设计.现实世界中物体根据运动的性质在曲线上进行加速或者减速，而不是做直线运动.
  + 所以移动也应该使用这样的属性或者动画来保持自然。
  + 例如一辆车离开屏幕应该是先慢后快直到离开。同样的, 视图也应该使用插值器类例如 AccelerateInterpolator, FastOutSlowInInterpolator 
  + 等等 [[更多参考]](https://developer.android.com/reference/android/animation/TimeInterpolator.html)

+ **排版**
  +  While custom typefaces can be used for branding, it is essential to stick to Roboto and Noto if possible, especially for body text, due to their clarity and optimistic nature.
  +  Roboto covers Latin, Greek and Cyrillic extended scripts, with Noto filling in for other language scripts [[More Info]](https://material.google.com/style/typography.html#)
  +  Weight balancing is an important aspect of typography, the fundamental concept of which is that the larger a typeface is, the less its weight should be so that it doesn't appear too thick and balances its weight with smaller typefaces of higher weights
  +  Typography should align to a 4dp baseline grid, and maintain a minimum contrast ratio of 4.5:1 based on luminance values, with a recomemended ratio being 7:1.
  +  The ideal reading length for large blocks of text is 40 to 60 characters per line. Anything less is too narrow and anything more is too wide.

+ **图标**
  + Icons should be designed at 48dp, with 1dp edges, which equates to
      +  48px by 48px at mdpi
      +  72px by 72px at hdpi
      +  96px by 96px at xhdpi
      +  144px by 144px at xxhdpi
      +  192px by 192px at xxxhdpi
  + An additional icon of 512px by 512px should be designed for use on Google Play
      + Material icons, in addition to the base icon, should contain the following important elements
      + 1dp tinted edge at the top
      + 1dp shaded edge at the bottom
      + Contact shadow - a soft shadow around all edges of raised elements
      + Finish - a soft tint to provide surface lighting, fading from upper life to lower right [[More Info]](https://material.google.com/style/icons.html#icons-product-icons)

+ **水波纹**
  + 使用 `?attr/selectableItemBackground` 替代 `?android:attr` ([Ref](https://twitter.com/pareshmayani/status/772061422729637893))
  + 在例如 Button 这种控件内部实现水波纹 ([Ref](https://twitter.com/pareshmayani/status/772268888931176448))

        ```xml
        android:background="?attr/selectableItemBackground"
        ```
  + 实现可溢出的水波纹: ([Ref](https://twitter.com/pareshmayani/status/772269413290520576))

        ```xml
        ?attr/selectableItemBackgroundBorderless
        ```

+ **其他**
  + Views should be aligned to Material Design's 8dp baseline grid and the keylines when possible. This gives the UI a sense of structure and hierarchy. [[More Info]](https://material.google.com/layout/metrics-keylines.html)（这个说的是设计方面的，8dp基线我不知道是啥）
  + 如果你要保留一个 ViewGroup 的引用（像 LinearLayout 、FrameLayout等等）又没有用到他们的特殊方法，就生命一个ViewGroup[[More Info]](https://android.jlelse.eu/android-pro-tip-1-443f423b4de6#.pklc9djmc)
  + accent color 和 primary color 颜色要互补，形成比较好的对比度。


###***Tips 关于 [Kotlin](https://kotlinlang.org/)***

+ **关注 [From Java to Kotlin](https://fabiomsr.github.io/from-java-to-kotlin/)**

      Java 转 Kotlin 的 Cheatsheet.

    -

###***其他资源***

+ **关注 podcasts**
      
  1. [Fragmented](http://fragmentedpodcast.com/)
  2. [Android Developers Backstage](https://androidbackstage.blogspot.in/)

    这两个最为著名。

+ **关注 [Android Dialogs](https://www.youtube.com/channel/UCMEmNnHT69aZuaOrE-dF6ug/feed)**
      
    Android 专家的采访短视频。

+ **关注 [CodePath Android Cliffnotes](https://guides.codepath.com/android)**

    有关于各种主题的完整的 Android 资源，并且实时更新。

+ **[注意 copyright](http://jeroenmols.com/blog/2016/08/03/copyright/)**

+ **关注新的 Android 开发库**

      [Android Arsenal](https://android-arsenal.com/) - 和 Android 开发者相关的工具、库、app

+ **关注 android example apps**
      + [Android Examples](https://github.com/nisrulz/android-examples) - 简单的 Android 例子。
      + [Google Samples](https://github.com/googlesamples) - google 提供的多种 Android 例子
      + [Google Android Codelabs](https://codelabs.developers.google.com/?cat=Android)

+ **Twitter上进行关注**
      
    + [#AndroidDev](https://twitter.com/search?q=%23AndroidDev)

+ **Twitter 创建列表**
      
    + [Android List](https://twitter.com/nisrulz/lists/android)

+ **[阅读Effective Java](https://www.amazon.ca/Effective-Java-2nd-Joshua-Bloch/dp/0321356683)**
    
    + [Cheatsheet/Summary](https://github.com/HugoMatilla/Effective-JAVA-Summary)

+ **[Subscribe to Caster.io](https://caster.io/)**

    Android开发视频
    
+ **书签中加入这些网站**
      
  + [Android Developers - Youtube Channel](https://www.youtube.com/user/androiddevelopers/videos)
  + [Android Niceties - UI Showcase](http://androidniceties.tumblr.com/)
  + [Material Design Specs](https://material.google.com/)
  + [Everything About Material Design](https://material.io/)
  + [Platform Version Distribution](https://developer.android.com/about/dashboards/index.html#Platform)
  + [Android Studio Release Notes](https://sites.google.com/a/android.com/tools/recent)
  + [Android Developers Blog](https://android-developers.blogspot.in/)
  + [AndroidDev-Reddit](https://www.reddit.com/r/androiddev)
  + [Github Trending Java Projects](https://github.com/trending?l=java&since=weekly)
  + [Stackoverflow-Android tag](https://stackoverflow.com/questions/tagged/android)
  + [Support Library History](https://developer.android.com/topic/libraries/support-library/revisions.html)
  + [Android Conferences](https://androidstudygroup.github.io/conferences/)
  + [Android Dev Docs](https://developer.android.com/reference/packages.html)
  + [Material Up - DesignShowcase](http://www.material.uplabs.com/)
  + [Dribbble - MaterialDeisgnShowcase](https://dribbble.com/tags/material_design)

+ **使用免费的 mockable api**
  + [Mockey](https://github.com/clafonta/Mockey) - A tool for testing application interactions over http, with a focus on testing web services, specifically web applications that consume XML, JSON, and HTML.
  + [JSON Placeholder](http://jsonplaceholder.typicode.com/) - Fake Online REST API for Testing and Prototyping
  + [API Studio](http://apistudio.io/) - a playground for API developers
  + [Mocky](http://www.mocky.io/) - Mock your HTTP responses to test your REST API
  + [Mockbin](http://mockbin.com) - Mockbin allows you to generate custom endpoints to test, mock, and track HTTP requests & responses between libraries, sockets and APIs.

+ **订阅这些内容**
  + [Android Weekly](http://androidweekly.net/) - Free newsletter that helps you to stay cutting-edge with your Android Development
  + [AndroidDevDigest](https://www.androiddevdigest.com/) - A Handcrafted Weekly #AndroidDev Newsletter
  + [Infinium #AndroidSweets](https://androidsweets.ongoodbits.com/) - Fresh news from Droid zone
  + [Kotlin Weekly](http://us12.campaign-archive2.com/home/?u=f39692e245b94f7fb693b6d82&id=93b2272cb6) - Free newsletter to stay uptodate with Kotlin Development

+ **[ADB/Fastboot Tools made avaialble as a separate package by google](https://plus.google.com/+ElliottHughes/posts/U3B6H3Sejvv), download latest version for**
  + [MacOSX](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip)
  + [Linux](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)
  + [Windows](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

+ **其他的一些优秀的开发工具**
  + [Android SVG to VectorDrawable](https://inloop.github.io/svg2android/) - 一个 VectorDrawable 适配所有屏幕分辨率
  + [SQLite Viewer](https://inloop.github.io/sqlite-viewer/) - 在线查看Sqlite
  + [Android 9-patch shadow generator](https://inloop.github.io/shadow4android/) - 帮助实现可完全定制的阴影
  + [APK method count](https://inloop.github.io/apk-method-count/) - apk 方法数目统计
  + [Material Palette](https://www.materialpalette.com/) - 快速生成 material 风格调色板
  + [Javadoc Themer](http://javadocthemer.crushingcode.co/) - 丰富你的JavaDoc
  + [Method Count](http://www.methodscount.com/) 
  + [Gradle, please](https://gradleplease.appspot.com/) - 通过名称查出 Android 依赖
  + [jsonschema2pojo](http://www.jsonschema2pojo.org/) - Json转Obj（我一般用GsonFormat）
  + [Android Asset Studio](http://romannurik.github.io/AndroidAssetStudio/) - A web-based set of tools for generating graphics and other assets that would eventually be in an Android application's res/ directory.
  + [Device Art Generator](https://developer.android.com/distribute/tools/promote/device-art.html) - Quickly wrap app screenshots in device artwork
  + [Google Translator Toolkit](https://translate.google.com/toolkit/list?hl=en#translations/) - string.xml 快速翻译
  + [JSONViewer](http://jsonviewer.stack.hu/) - json格式化
  + [ShapeShifter](https://alexjlockwood.github.io/ShapeShifter/) - SVG动画编辑器
  + [App Privacy Policy Generator](https://app-privacy-policy-generator.firebaseapp.com/) - 生成你google play 的隐私策略

+ **优秀的 android libraries**
  + [StorIO](https://github.com/pushtorefresh/storio) - SQLiteDatabase 和 ContentResolver 的优雅封装
  + [Retrofit](https://github.com/square/retrofit) -  Square 出品 NB 网络库 
  + [Picasso](https://github.com/square/picasso) - 优秀的图片加载库
  + [LeakCanary](https://github.com/square/leakcanary) - 内存泄露检查工具
  + [AndroidViewAnimations](https://github.com/daimajia/AndroidViewAnimations) - 可爱的动画合集
  + [Calligraphy](https://github.com/chrisjenx/Calligraphy) - 最简单的自定义字体使用方法

    -

#### **作者的开源库(不是晓晨哦,这篇文档原作者)**
  + [EasyDeviceInfo](https://github.com/nisrulz/easydeviceinfo) - Enabling device information to be at android developers hand like a piece of cake!
  + [Sensey](https://github.com/nisrulz/Sensey) - Android library to make detecting gestures easy
  + [PackageHunter](https://github.com/nisrulz/PackageHunter) - Android library to hunt down package information
  + [Zentone](https://github.com/nisrulz/zentone) - Easily generate audio tone in android
  + [RecyclerViewHelper](https://github.com/nisrulz/recyclerviewhelper) - RecyclerViewHelper provides the most common functions around recycler view like Swipe to dismiss, Drag and Drop, Divider in the ui, events for when item selected and when not selected, on-click listener for items.
  + [StackedHorizontalProgressbar](https://github.com/nisrulz/stackedhorizontalprogressbar) - Android Library to implement stacked horizontal progressbar
  + [QREader](https://github.com/nisrulz/qreader) - A library that uses google's mobile vision api and simplify the QR code reading process
  + [ScreenShott](https://github.com/nisrulz/screenshott) - Simple library to take a screenshot of the device screen , programmatically!
  + [EvTrack](https://github.com/nisrulz/EvTrack) - Android library to make event and exception tracking easy
  + [OptimusHTTP](https://github.com/nisrulz/OptimusHTTP) - Android library that simplifys networking in android via an async http client
  + [ShoutOut](https://github.com/nisrulz/ShoutOut) - Android library for logging information in android
