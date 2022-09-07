<div align='center'>
    <h1>Day 16</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
    <a class="header-badge" target="_blank" href="https://instagram.com/100rabhch">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=instagram&logo=instagram&style=social">
    </a>
    <a class="header-badge" target="_blank" href="https://stackoverflow.com/users/12053852/saurabh-chavan?tab=profile">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=stackoverflow&logo=stackoverflow&style=social">
    </a>
 </div>

<div align='center'>
    <h1>Project 1</h1> 
</div>

## Day 16

**ViewController.swift**

```

import UIKit

class ViewController: UIViewController {
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }
}
```

Four things in it.

**1**. The file starts with import UIKit, which means “this file will reference the iOS user interface toolkit.”

**2**. The class ViewController: UIViewController line means “I want to create a new screen of data called ViewController, based on UIViewController.”
When you see a data type that starts with “UI”, it means it comes from UIKit.
UIViewController is Apple’s default screen type, which is empty and white until we change it.

**3**. The line override func viewDidLoad() starts a method. As you know, the override keyword is needed because it means “we want to change Apple’s default behavior from UIViewController.”
viewDidLoad() is called by UIKit when the screen has loaded, and is ready for you to customize.

**4**. The viewDidLoad() method contains one line of code saying super.viewDidLoad() and one line of comment (that’s the line starting with // ).
This super call means “tell Apple’s UIViewController to run its own code before I run mine,” and you’ll see this used a lot.
