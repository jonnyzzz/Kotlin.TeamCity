Kotlin.TeamCity
===============

An Ant script and TeamCity meta-runner to automatically setup all 
required settings for IntelliJ IDEA build runner to build kotlin 
projects

It declares all parameters as specified in 
http://confluence.jetbrains.com/display/JET/Setting+up+a+TeamCity+build+that+uses+Kotlin

Installation
============
- Download and apply meta-runner ```kotlinc.xml``` to your TeamCity installation.
- Add ```Setup Kotlinc``` build runner to the build(s) before the ```IntelliJ IDEA``` build runner
- Enjoy


Internals
==========
The script uses TeamCity service message to set all necessary build parameters. 

It also sets/overrides the ```system.path.macro.KOTLIN.BUNDLED``` parameter with 
full path to Kotlin on build agent. It simplifies use of ```KOTLIN_BUNDLED``` path 
variable in IntelliJ IDEA. You may have any value of the variable in TeamCity build
parameters tab


License
=======
MIT

You may do what ever you like with the script


