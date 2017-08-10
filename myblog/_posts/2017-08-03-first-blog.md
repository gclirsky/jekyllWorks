---
layout: post
title: Git Tips
date: 2017-08-02 09:38:00 +0800 # permalink: var.date>filename
slug: git tips # permalink: var.slug>filename>var.title
tags: [git, beginner, tutorial] # similar to category but unlike category will put on spec paths/folders (tag doesn't)
categories: guide git # delimiter is space
---

### How can I associate local unversioned code to git remote repository?

- First of all, remove all .svn directories in working copy directory;

- Initialize new git repository in the working copy directory
 
```bash
cd /path/to/my/project
git init
```

- Add git remote repository and fetch it

```bash 
git remote add origin url-to-your-remote
git fetch origin
```

- Reset working copy to remote repository
 
```bash
git reset --hard origin/master
```

At the end local repository will be synchronized with remote repository.


- Code Highlighter Test - C# codes

```c#
public test {
    public void print(string name){
        Console.WriteLine("Hello " + name);
    }
}
```

with hightlight command

{% highlight c# %}
public test {
    public void print(string name){
        Console.WriteLine("Hello " + name);
    }
}
{% endhighlight %}