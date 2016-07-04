### a
* ar -r libtest.a test_a.o
  gcc -c test_a.c
* gcc -o test test.c -static -L. -ltest   --->OK
  gcc -static -o test -L. -ltest test.c   --->NG
  undefined reference to 'TestA'
  因为编译器从左向右读取文件， 当读到-ltest时，因为是静态的，但此时还不知道该把哪个符号抽出来。所以只好往后继续处理，等在test.c中发现
  需要填入的函数时，后面的文件却没有这个符号的实现。所以就抱错了。【静态库链接时放在后面】
  -static 因为在GCC中，会优先使用so. 当a/so都存在时，为了确保使用的是a，则使用此选项。
* nm libtest.a

### so
* gcc test_a.c -fPIC -shared -o libtest.so
  -fPIC 作用于编译阶段，告诉编译器产生与位置无关代码(Position-Independent Code)
* gcc test.c -o test -L. -ltest
* export LD_LIBRARY_PATH=./
  环境变量中添加动态库搜索当前路径
* nm libtest.so
* ldd libtest.so
