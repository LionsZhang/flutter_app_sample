# flutter_app

A new Flutter application.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


Step1: https://www.myfreax.com/detailed-flutter-command/按文档搭建flutter开发环境
Step2: 新建flutter项目,配置下载镜像
      maven { url 'https://maven.aliyun.com/repository/google' }
          maven { url 'https://maven.aliyun.com/repository/jcenter' }
          maven { url 'http://maven.aliyun.com/nexus/content/groups/public' }
  替换//        google()
    //        jcenter()
   指定kotlin 版本如果使用kotlin开发,在File——>set——>language&frame中查看本地下载的kotlin版本，然后在anroid的build.gradle中指定
   指定gradle版本，（如果本地已经存在可以直接修改指定对应gradle和gradle plugin）如果没有执行step3.
   将flutter SDK中 /packages/flutter_tools/gradle/flutter.gradle添加上述镜像并且修改gradle plugin依赖版本与项目一致
step3  运行项目，先用Android环境打开试运行看是否顺利运行，根据提示操作(没有gradle会下载执行)
     如果能顺利运行则表明环境没问题
step4  去除flutter项目报红问题
      a. File——>Project Structure选择project 指定Androidsdk api等级
      b. File——>set——>language&frame 指定flutter和dart sdk路径
      c. 关闭项目删除项目中.idea和.gradle目录清除缓存
      d. 将app目录下的build文件中GradleException 改为Exception