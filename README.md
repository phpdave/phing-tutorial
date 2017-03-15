# phing-tutorial
Trying out phing

1. Download Phing by using composer and the composer.json file.
2. "/usr/bin/php" "{FilePathTo}/composer.phar" "--ansi" "--no-interaction" "install"
3. Phing will now be available in ./vendor/bin/phing
4. Create your build.xml file 
5. Run phing against default
```
Computer:CurDir User$ ./vendor/bin/phing
Buildfile: ./phing-tutorial/build.xml

HelloWorld > welcome:

     [echo] Hello World!

BUILD FINISHED

Total time: 0.2455 seconds
```
6. Run phing against a target environment
./vendor/bin/phing dev
./vendor/bin/phing qa
./vendor/bin/phing prod

7. Getting fancy install php's ssh2 extension on mac:
```
brew install php56-ssh2
brew link autoconf
brew install homebrew/php/php56-ssh2
```
8.a. handle annoying ssh2 bug
cd ~/.ssh
openssl rsa -in id_rsa -out id_rsa.pem
8.b. still cant figure out how to do ssh or scp task in phing... just going to use exectask
9. Moved on from example build.xml to current build
Computer:CurDir User$ ./vendor/bin/phing
Buildfile: ./phing-tutorial/build.xml

LitmisSpaceDeploy > dev:

     [echo] Phing has started
     [echo] Current Directory
       ./phing-tutorial
     [echo] Copying files to spaces.litmis.com

BUILD FINISHED

Total time: 2.1710 seconds