# phing-tutorial
Trying out phing

1. Download Phing by using composer and the composer.json file.
2. "/usr/bin/php" "{FilePathTo}/composer.phar" "--ansi" "--no-interaction" "install"
3. Phing will now be available in ./vendor/bin/phing
4. Create your build.xml file 
5. Run phing
```
Computer:CurDir User$ ./vendor/bin/phing
Buildfile: ./phing-tutorial/build.xml

HelloWorld > welcome:

     [echo] Hello World!

BUILD FINISHED

Total time: 0.2455 seconds
```