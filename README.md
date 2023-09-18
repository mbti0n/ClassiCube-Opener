# ClassiCube-Opener
Shortcut to open [ClassiCube](https://www.classicube.net/) (normally)

## Why?
On Windows, you only need to open the ClassiCube.exe file, and you are done. But on macOS, you have a Unix executable file name `ClassicCube`. Just `ClassiCube`, neither `ClassiCube.exe` nor `ClassiCube.dmg`. You cannot open it just by double clicking on that file, it will look like this:

<img width="569" alt="image" src="https://github.com/mbti0n/ClassiCube-Opener/assets/105599214/2f5eb76b-52ba-4017-8cd2-e72a428d07b9">

You have to run this script:
```
chmod +x /path/to/ClassiCube
/path/to/ClassiCube
```

The problem is, you have to do it in Terminal EVERY TIME you want to open the app. This does not feel like a proper app, this feels more like a Python script that takes you 10 years to finish. Too long, too complicated, too mid, because you cannot just double click to open it like on Windows. And here's the beginning of my work.

## How it works
Well, it is simple. Open `Shortcuts` app and create a new shortcut. Then, add a ``Run Shell Script`` action. Replace the `echo "Hello World"` with:
```
chmod +x /path/to/ClassiCube
/path/to/ClassiCube
```

Add the shortcut to your Dock (or you can move it into your Application folder), and now you can run ClassiCube on macOS without running the script in Terminal.
