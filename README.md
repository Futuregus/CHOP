# 🪓 CHOP: Comment Header Organization System for Python

> *Slice your code into clean, readable chunks—like a pro.*

CHOP is a custom VS Code snippet pack designed to help you keep your code beautifully structured and **visually readable**. It brings class, method, and group headers into your workflow with minimal effort and maximum style.

---

## 🌱 Origin Story

CHOP started as a personal system I made for myself because I found Python’s indentation-based scoping to be hard to follow. I wanted something that made scopes more *visually* obvious and made large files easier to navigate.

So I started manually adding these headers... and it turned out to be an awesome way to organize everything. Eventually, I turned the system into a VS Code snippet pack so I wouldn’t have to keep copy/pasting. Now it’s quick and clean.

---

## 📦 Features

* 🧱 **Class Headers**
  Mark the start and end of classes.

* 🔹 **Class Sub-Group Header**
  Break your classes into groups of related methods.

* 🔧 **Method Sub-Group Header**
  Organize the inside of your methods.

* 📜 **Quick Description Comments**
  Easily add description lines for clarity and documentation.

---

## 💻 Why Use CHOP?

Because messy code is a crime 😤
CHOP helps you:

* Stay visually organized
* Navigate huge files quickly
* Communicate structure to teammates
* Look cool while coding 😎

<details>
  <summary>Click to view example code using CHOP </summary>

```python
# %--- Animal Class ---%

class Animal:

#  +--- Animal Initialization  ---+

    def __init__(self, name, age):
        self.name = name
        self.age = age

#  +----------------------+



#  +--- Animal Methods ---+


    def speak(self):
        pass

    def eat(self):
        pass

#  +----------------------+


# %----------------------%



# %--- Dog Class ---%

class Dog(Animal):

#  +--- Dog Initialization ---+

    def __init__(self, name, age, breed):
        super().__init__(name, age)
        self.breed = breed

 
    def speak(self):
        return f"{self.name} says woof!"

    def fetch(self):
        return f"{self.name} is fetching a ball."

#  +----------------------+

#  +--- Dog Methods ---+

def main():

    my_dog = Dog("Buddy", 3, "Golden Retriever")
    

    print(my_dog.speak())   
    print(my_dog.fetch())   

#  +----------------------+

# %----------------------%


if __name__ == "__main__":
    main()
    
```

</details>

---

## 🛠️ Installation

1. Open VS Code
2. Press Ctrl+Shift+P then search "Snippets: Configure Snippets".
3. Click `New Global snippets file` or `New snippets file for "Scriptname"` if you don’t want it for all scripts.
4. Paste in the [CHOP.code-snippets](https://github.com/Futuregus/CHOP/blob/main/CHOP.code-snippets) contents.
5. Save and start choppin’.

> ⚠️ **Note:** CHOP is designed specifically for Python and **VS Code**.

---

## 🚀 Usage

| Prefix    | Purpose                     | Output                        |
| --------- | --------------------------- | ----------------------------- |
| `C-hdr`   | Class Header                | `# %--- Class Name ---%`      |
| `C-end`   | Class End Marker            | `# %----------------------%`  |
| `CG-hdr`  | Class Sub-Group Header      | `#  +--- Sub Group ---+`      |
| `CG-end`  | Class Sub-Group End Marker  | `#  +----------------------+` |
| `MSG-hdr` | Method Sub-Group Header     | `# === Group Title ===`       |
| `MSG-end` | Method Sub-Group End Marker | `# =====================`     |
| `desc`    | Description Comment         | `# Description: ...`          |

---

If you want to use the system manually without the snippets, just click below and follow these header formats for different sections of your code:

* **Class Header**
  Use `%--- Title ---%` to mark the start of a class.

* **Class Sub-Group Header**
  Use `+--- Title ---+` to organize similar methods within a class.

* **Method Sub-Group Header**
  Use `=== Title ===` to organize parts within a method.

* **End of Method Sub-Group**
  Use `=====================` to mark the end of a method sub-group.

* **End of Class Sub-Group**
  Use `+----------------------+` to mark the end of a class sub-group.

* **End of Class Header**
  Use `%----------------------%` to mark the end of a class.

---

### Feedback? Feature ideas? Just reach out by making an [issue](https://github.com/Futuregus/CHOP/issues).
