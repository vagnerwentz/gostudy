 # ⚠️Under Construction⚠️ 
# Go (golang)

* **Strong and statically typed.**
* **Excellent community.**
* **Key features**
  * Simplicity
  * Fast compile times
  * Garbage collected
  * Built-in concurrency
  * Compile to standalone binaries

# Variables
* **Variable declaration**
  * The `var` statement declares a list of variables; as in function argument lists, the type is last.
  A `var` statement can be at package or function level.

    ```go
    package main

    import "fmt"

    var c, python, java bool

    func main() {
      var i int
      fmt.Println(i, c, python, java)
    }
    ```
* **Variables with initializers**
  * A `var` declaration can include initializers, one per variable. If an initializer is present, the type can be omitted; the variable will take the type of the initializer.
    ```go
    package main

    import "fmt"

    var i, j int = 1, 2

    func main() {
      var c, python, java = true, false, "no!"
      fmt.Println(i, j, c, python, java)
    }
    ```
* **Short variable declarations**
  * Inside a function, the := short assignment statement can be used in place of a `var` declaration with implicit type. Outside a function, every statement begins with a keyword (`var`, `func`, and so on) and so the `:=` construct is not available.
    ```go
    package main

    import "fmt"

    func main() {
      var i, j int = 1, 2
      k := 3
      c, python, java := true, false, "no!"

      fmt.Println(i, j, k, c, python, java)
    }
    ```
* **Redeclaration and shadowing**
  * Can not redeclare variables, but can shadow them
  * All variables must be used
* **Visibility**
  * lower case first letter for package scope
  * upper case first letter to export
  * no private scope
* **Naming conventions**
  * Pascal or camelCase
    * Capitalize acronyms (HTTP, URL)
  * As short as reasonable
    * longer names for longer lives
* **Type conversions**
  * destinationType (variable)
  * use strconv package for strings
  
  