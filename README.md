# Learning
 In spring config bean attribute scope importance 

**Singleton(default):-**
After the context.getBean("class name") again 
we write the context.getBean("class")
It will refer the first(old) object that is called the Singletone .

If we are creating the new object, it still refer the old object which is earlier created.

**Prototype:-**
When we invoking/creating the obj/instance through the context.getbean and in xml file we mention the scope of the class is prototype then after creating the multiple obj that obj refering to unique reference which is created by that obj.

Request:-
Session":-
Global Session:-


**Lazy and Eagar Bean=>**

# Eagar(Default)=>
```
    Bean is instantiated when classpathApplication (IOC ) container is created.

 # Lazy=>**
    Bean is instantiated when context.getbean("Class") .

    note:- when there is lot off heavy resources then it's better to used the Lazy.

    lazy-init="true" mention inside the XML file for specific class.

    Lazy-Init=>
      a)it will instansited the applicationxmlcontext 
      b)all the class will be instansited expect the lazy-init
      c)after invoking the getbean it will get instansited 
      
