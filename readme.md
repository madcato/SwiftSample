# Swift in ubuntu


http://www.makeuseof.com/tag/start-programming-swift-ubuntu/

Finally, you can also make executables from your Swift code. All you need to do is the following:

1. Create a project folder with any name you like, then inside there create a folder with the name “sources”.
2. Place all of your code files inside the source folder.
3. Create a text file named “Package.swift” in the project folder (but outside the sources folder) and put at least the following in it:

```swift
import PackageDescription

let package = Package(
    name: "package_name_here_and_keep_quote_marks"
)
```

Finally, run

	$ swift build

while the project folder is the working directory. You will find the executable under

	$ .build/debug/package_name