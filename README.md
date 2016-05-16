# mupdf-source
这里提供mupdf开源库的源代码，并已为android平台编译好；

#MuPdf官方地址：http://mupdf.com/

#文件说明
mupdf-1.8-source.tar.gz为官方1.8版本原版源代码；
mupdf-1.9a-source.tar.gz为官方1.9a版本原版源代码；
mupdf-1.8-source-compiled.7z为官方1.8版本且已为android平台编译过的源代码，解压可得到mupdf-1.8-source目录；
mupdf-1.9a-source-compiled.7z为官方1.9a版本且已为android平台编译过的源代码，解压可得到mupdf-1.9a-source目录；

目前上传了两个版本的mupdf开源库，mupdf-1.8和mupdf-1.9a;
并已安装官方指导为android平台编译过；
1.9a版本编译后的so库比较大，有17M左右，将近1.8及以前版本的两倍，代码1.9a的流畅度要由于1.8，所以在选择上酌情考虑；

如要使用原版源代码，请参考官方编译指导和我在编译过程中遇到的一些问题记录http://blog.csdn.net/super_spy/article/details/51385869；

如要使用已编译过的源代码，请参照如下说明：
mupdf-1.8-source-compiled.7z解压可得到mupdf-1.8-source目录；
mupdf-1.9a-source-compiled.7z解压可得到mupdf-1.9a-source目录；
1.8版本的android demo目录位置mupdf-1.8-source\platform\android，可以使用eclipse和android studio引入；已编译全cpu平台库；
1.9a版本的android demo目录位置mupdf-1.9a-source\platform\android\viewer可以使用eclipse和android studio引入；目前只编译了armeabi-v7a库，如果需要其他cpu平台的库，可以编辑mupdf-1.9a-source\platform\android\viewer\jni目录下的Application.mk文件，选择需要编译cpu平台，然后在mupdf-1.9a-source\platform\android\viewer\目录下执行ndk-build命令重新编译；

#重新编译
  如果需要重新编译，请务必保证源代码的目录结构完整，并在android demo目录（1.8版本为mupdf-1.8-source\platform\android，1.9a版本为mupdf-1.9a-source\platform\android\viewer）下执行ndk-build命令；
  （注：如果无法重新编译，可以使用官方原版源代码参照官方编译指导进行重新编译）
#运行
  编译完成后，使用eclipse或android studio导入android demo（1.8版本为mupdf-1.8-source\platform\android目录，1.9a版本为mupdf-1.9a-source\platform\android\viewer目录），一般不需要做什么调整即可运行（如果无法直接运行，那就只能根据错误日志进行调整，一般比较简单）；
#开发
  结合demo运行情况及其代码，重新开发自己需要的界面和功能即可；
  
  ![image1](https://github.com/ZhangSir/mupdf-source/blob/master/Screenshot_2016-05-16-14-33-44.jpeg)
  ![image2](https://github.com/ZhangSir/mupdf-source/blob/master/Screenshot_2016-05-16-14-33-58.jpeg)
