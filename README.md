 * Java并发,详见NOTICE:https://blog.csdn.net/zhuhai0613/article/details/133545621
 
 * 如果报错: SourceSet with name ‘main’ not found,则采取下列方式:
 * 1.先选择合适的as版本，建议：3.5.3
 * 2.将项目结构转换成project，然后在.idea文件夹中找到gradle.xml，
 * 打开文件，在 GradleProjectSettings 标签下添加<option name="delegatedBuild" value="false" />
 * 这句话的意思是不让gradle接管构建任务，防止当作gradle的task来执行。
 * 3.clean project或清除缓存后（但依然要有上述标签）重新执行main函数
 * 代码都在test目录下