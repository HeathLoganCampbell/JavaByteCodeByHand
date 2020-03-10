# Java Byte Code By Hand
So I thought I would look into the nitty gritty of how java real works

## Notes
### Magic number
```
cafe babe
```

### Java version 8
Java 8 is version 52 which then decodes to 
```
00 00 00 34
```

### Constant Pool
this is basically the most  important part to java's bytecode which allows us to reference other classes, 
use strings and store other variables

### Access Modifiers
```
ACC_PUBLIC     0x0001
ACC_PRIVATE    0x0002
ACC_PROTECTED  0x0004


ACC_STATIC     0x0008
ACC_FINAL      0x0010
ACC_SUPER      0x0020
ACC_INTERFACE  0x0200
ACC_ABSTRACT   0x0400
```

### Quick structure
```
Java File: CAFE BABE
Version 8: 0000 0034
Constant Pool Size of ZERO: 0000
Super Public: 0021
Unknown index of class in constant pool: 0000
Unknown index of super class in constant pool: 0000
zero interfaces: 0000
zero fields: 0000
zero methods: 0000
zero attributes: 0000
``` 
Class name must be at reference constant pool at #1

#### Example
```
07 00 02
01 00 0a            48 65 6c 6c 6f 57 6f 72 6c 64
```

this points #1 to #2

```
Constant pool:
   #1 = Class              #2             // JavaByHand
   #2 = Utf8               JavaByHand
   #3 = Class              #4             // java/lang/Object
   #4 = Utf8               java/lang/Object
   #5 = Class              #6             // java/lang/System
   #6 = Utf8               java/lang/System
   #7 = Class              #8             // java/io/PrintStream
   #8 = Utf8               java/io/PrintStream
   #9 = String             #10            // Hello World
  #10 = Utf8               Hello World
```


## Take aways 
 - useage of javap
 - The structure of a java class
 - How variables and strings are saved and loaded in java


## References 
https://medium.com/@davethomas_9528/writing-hello-world-in-java-byte-code-34f75428e0ad
https://www.javaworld.com/article/2077233/bytecode-basics.html
https://www.programcreek.com/2013/04/what-can-you-learn-from-a-java-helloworld-program/
https://gitlab.ow2.org/ 