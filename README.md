# 🪓 CHOP: Comment Header Organization System for Python

> *Slice your code into clean, readable chunks—like a pro.*

CHOP is a custom VS Code snippet pack designed to help you keep your code beautifully structured and **visually readable**. It brings class, function, and group headers into your workflow with minimal effort and maximum style.

---

## 🌱 Origin Story

CHOP started as a personal system I made for myself because I found Python’s indentation-based scoping to be hard to follow. I wanted something that made scopes more *visually* obvious and made large files easier to navigate.

So I started manually adding these headers... and it turned out to be an awesome way to organize everything. Eventually, I turned the system into a VS Code snippet pack so I wouldn’t have to keep copy/pasting. Now it’s quick and clean.

---

## 📦 Features

- 🧱 **Class Headers**  
  Mark the start and end of class sections with bold, distinct headers.

- 🔹 **Sub-Group Headers**  
  Break your classes into organized sections with sub-group labels.

- 🔧 **Function Groups**  
  Organize functions into categories.

- 📜 **Quick Description Comments**  
  Easily add description lines for clarity and documentation.

---

## 💻 Why Use CHOP?

Because messy code is a crime 😤  
CHOP helps you:
- Stay visually organized
- Navigate huge files quickly
- Communicate structure to teammates
- Look cool while coding 😎

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



#  +--- Animal Meathods ---+


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
2. press Ctrl+Shift+P then search "Snippets: Configure Snippets.
3. click `New Global snippets file` or `New snippets file for "Scriptname"` if you dont want it for all scripts
4. Paste in the [CHOP.code-snippets](https://github.com/Futuregus/CHOP/blob/main/CHOP.code-snippets) contents.
5. Save and start choppin’.

> ⚠️ **Note:** CHOP is designed specifically for Python and **VS Code**.

---

## 🚀 Usage

| Prefix     | Purpose                         | Output                      |
|------------|----------------------------------|------------------------------------|
| `C-hdr`    | Class Header                    | `# %--- Class Name ---%`           |
| `C-end`    | Class End Marker                | `# %----------------------%`       |
| `CG-hdr`   | Class Sub-Group Header          | `#  +--- Sub Group ---+`           |
| `CG-end`   | Class Sub-Group End Marker      | `#  +----------------------+`      |
| `FSG-hdr`  | Function Sub-Group Header       | `# === Group Title ===`            |
| `FSG-end`  | Function Sub-Group End Marker   | `# =====================`          |
| `desc`     | Description Comment             | `# Description: ...`               |

---

If you want to use the system manually without the snippets, Just click below and follow these header formats for different sections of your code:
<details>
  <summary>Click to view CHOP </summary>


- **Class Header**  
  Use `%--- Title ---%` to mark the start of a class.

- **Class Sub-Group Header**  
  Use `+--- Title ---+` to orgonize similar functions within a class.

- **Function Sub-Group Header**  
  Use `=== Title ===` to organize parts whithin a function.

- **End of Function Sub-Group**  
  Use `=====================` to mark the end of a function group.

- **End of Class Sub-Group**  
  Use `+----------------------+` to mark the end of a class sub-group.

- **End of Class Header**  
  Use `%----------------------%` to mark the end of a class.

</details>

---

### Feedback? Feature ideas? Just reach out by making an [issue](https://github.com/Futuregus/CHOP/issues).
