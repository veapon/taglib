# Install
See: [https://github.com/veapon/taglib/blob/master/INSTALL](https://github.com/veapon/taglib/blob/master/INSTALL)

By default, taglib head files were installed in /usr/local/include/taglib and library files in /usr/local/lib.
You may need to make some changes to let the complier know where the taglib library is, for example, change the ld.so.conf file with follow command:

	echo "/usr/local/lib" >> /etc/ld.so.conf
	ldconfig

# Code examples
See: [https://github.com/veapon/taglib/tree/master/examples](https://github.com/veapon/taglib/tree/master/examples)

# Complie 
	gcc -c -I /usr/local/include/taglib -o a.o
	gcc -ltag_c a.o -o a
	./a