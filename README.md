1/31 JAN

Workshop 01

Setting up a project:
Single View Application.
Organisation Identifier.
Uncheck Core Data and including Tests.

Create Git respository on my mac.



*How do you print things out the debug area?

Print "Hello world"

*What is the shortcut to run your app?

CMD R

*What does "IB" mean?

interface builder

*How do you connect things from your storyboard to your code?

CTRL DRAG

*What's the difference between an IBOutlet and an IBAction?

IBOutlet - Label
IBAction - Butten


*What is the name of the function that gets called automaticaly in your view controller classes?


```override func viewDidload() {
    super.viewDidload()

*What is the assistant editor and what does it do?


Workshop 02
Creating a simple project:
Create a class
Set up two variables of different types
Create a function



How do you create a class - key word/casing/brackets?



What is the difference between a variable and a constant?



What must you do after creating a variable?



What does the word 'string' mean?



What key work (abreviation) is used to create a function?



What symbol means 'is of type'?



What does 'Int' mean?



How do you print out a variable or function in the debug area?



*Where is the icon for the Attribute Inspector, where is it located and what does it do?



*Where is the icon for the project navigator and where is it located?






31 Jan Xcode

import Foundation

class Person {
    
    var name: String!
      var age: Int!
      
      
      init(name: String, age: Int) {
            self.name = name
            self.age = age
      }
            func haveBirthday() {
                  age += 1
                  
            }
      
      func bio() {
                  print("My name is \(self.name) I am \(self.age) from bournemouth")
      
      }
}


import UIKit

class ViewController: UIViewController {
      
      let me = Person(name: "Ki", age: 23)
      
      @IBOutlet var Label: UIView!
      
      override func viewDidLoad() {
            super.viewDidLoad()
            Label.text = me.name
            
      }
      
      
      @IBAction func butten(_ sender: Any) {
            me.haveBirthday()
            print("My name is \(self.nibName) I am \(self.age) from bournemouth")
            
      }
      
      
}

