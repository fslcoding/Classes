# Classes

Everything in C# is made up of classes and objects. This repo is a brief introduction into the concepts of classes.

**_What is a class?_**

A class is like a blueprint. Like a car needs a blueprint to be built, an object needs a class to be built.

### Creating a class

To create a class, we need the ```class``` keyword.

```
class ClassName { }
```

Classes are made up of **_Members_**. Members can be:
+ [Variables](https://github.com/fslcoding/Variables_CS "Variables Repo")
+ [Properties](https://github.com/fslcoding/Properties_CS "Properties Repo")
+ [Methods](https://github.com/fslcoding/Methods_CS "Methods Repo")

Look at [Car.cs](https://github.com/fslcoding/Classes_CS/blob/main/Car.cs "Car Class"), we can see it has two variables.
```
string Colour;
string CarName;
```

This means that every car will have a ```Colour``` and a ```CarName```.


### Instantiating an object

When you instantiate an object, you create a version of the specified class.

This is what that would look like.

```
ClassName VariableName = new ClassName();
```

In [Program.cs](https://github.com/fslcoding/Classes_CS/blob/main/Program.cs "Program Class"), we create an object of the ```Car``` class.

```
Car Ferrari = new Car();
```

To access a **_member_** of an object, you use the ``` . ``` syntax.

```
// Car.cs
string CarName;

// Program.cs
Ferrari.CarName
```


<details>
    <summary>
        What would happen if you tried to access the Car's name? 
    </summary>

    Car.CarName is unaccessable due to it's protection level.

</details>

### Accessibility Modifiers
There are 2 main types of accessibility:
+ ```public```
+ ```private```

**_Public_** means that the member _can_ be seen outside of the class. <br>
**_Private_** means that the member _cannot_ be seen outside of the class.

The above error occured because **_members, by default, are private_**

<details>
    <summary>
        How would you fix the error?
    </summary>

    public string CarName;

</details>

### Changing / running a classes' members

Changing a classes' variable or _property_
```
Ferrari.CarName = "Ferrari F8";
Ferrari.Colour = "Red";
```

## Useful Links

[W3 Schools OOP](https://www.w3schools.com/cs/cs_oop.php)<br>
[W3 Schools Classes](https://www.w3schools.com/cs/cs_classes.php)

## More Learning

+ [Properties](https://github.com/fslcoding/Properties_CS)
+ [Inheritance](https://github.com/fslcoding/Inheritance_CS)
