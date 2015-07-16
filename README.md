
### Android Studio Project Structure

/*
 * ASProjectStructure
 * +-- .gradle
 * +-- .idea
 * +-- app
 * |   +-- build
 * |   +-- libs
 * |   +-- src
 * |   |   +-- main
 * |   |   |   +-- java
 * |   |   |   +-- res
 * |   |   |   +-- AndroidManifest.xml
 * |   +-- build.gradle (module: app)
 * |   +-- proguard-rules.pro (proguard rules for app)
 * +-- build
 * +-- gradle
 * |   +-- wrapper
 * |   |   +-- gradle-wrapper.properties (gradle version)
 * +-- module1
 * |   +-- build.gradle (module: module1)
 * |   +-- proguard-rules.pro (proguard rules for module1)
 * +-- module2
 * |   +-- build.gradle (module: module2)
 * |   +-- proguard-rules.pro (proguard rules for module2)
 * +-- build.gradle (project: ASProjectStructure)
 * +-- gradle.properties (project properties)
 * +-- local.properties (SDK location)
 * +-- settings.gradle (project settings)
 */

### Common Commands

./gradlew -v
./gradlew clean
./gradlew build
./gradlew assembleDebug
./gradlew assembleRelease

### References

http://tools.android.com/tech-docs/new-build-system/user-guide
https://docs.gradle.org/current/userguide/userguide.html
http://groovy-lang.org/documentation.html
https://developer.android.com/sdk/installing/migrate.html

### .gitignore

# .gitignore规则
# 以斜杠“/”开头表示从根目录出发
# 以星号“*”通配多个字符(至少一个)
# 以问号“?”通配单个字符
# 以方括号“[]”匹配字符集中的单个字符
# 以叹号“!”表示不忽略(跟踪)匹配到的文件或目录
# 按行从上到下进行规则匹配的，如果前面的规则匹配的范围更大，则后面的规则将不会生效

# .gitignore例子
# /.idea/ : 表示忽略.idea整个文件夹，包括自身，只匹配根目录下的.idea文件夹
# .idea/ : 表示忽略.idea整个文件夹，包括自身，匹配任意目录下的.idea文件夹
# .idea/* : 表示忽略.idea文件夹下的所有内容，不包括自身，只匹配根目录下的.idea文件夹
# .idea/*结合!/.idea/vcs.xml : 在.idea/*的基础上，不忽略vcs.xml（注意先后顺序）
# *.[ab] : 等价于 *.a *.b, 不会匹配*.ab, .a, .b