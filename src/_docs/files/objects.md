---
title: Reading and Writing Objects
permalink: /docs/files/objects/
---

Create a program that saves data beyond the life time of the program.  

Utilize the following struct:
{% highlight c++ %}
struct PetRock {
    string name;
    int age;
};
{% endhighlight %}

When the program runs, it first checks to see if a file contains data (PetRocks). If the file contains data then the data will be read from the file into an array of size 3 and will be printed (assume there will be no more than 3 objects saved in the data file). If no data is contained within the file, 3 {% ihighlight c++ %}PetRock{% endihighlight %} objects will be created and written to the file.

### Sample Output
**First time executing the program**
```
No data in file
Collecting Pet Rocks...
Storing Pet Rocks...
```

**Second time executing the program**
```
Data found in file
Storing Pet Rocks into array...

Pet Rocks:
Name: Pete
Age: 1032

Name: Eugene
Age: 124832

Name: Dwayne the Rock
Age: 2374
```