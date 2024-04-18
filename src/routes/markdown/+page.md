# This was wrtiten in markdown!
**I think Andrew will really like it:**
- cause it's cool
- cause he likes frontend stuff (kinda)
- cause I'm a boss and used an emoji! 😎

**This is a code block in markdown**

***https://go.dev/play/***
```go
package main

import (
    "bufio"
    "fmt"
    "os"
    "strings"
)

func main() {
    // Prompt the user for input
    fmt.Println("Enter text:")
    
    // Read user input
    scanner := bufio.NewScanner(os.Stdin)
    scanner.Scan()
    input := scanner.Text()

    // Convert input to Spongebob meme text
    var sbText string
    upper := true
    for _, char := range input {
        if char != ' ' {
            if upper {
                sbText += strings.ToUpper(string(char))
            } else {
                sbText += strings.ToLower(string(char))
            }
            upper = !upper
        } else {
            sbText += " "
        }
    }

    // Print Spongebob meme text
    fmt.Println(sbText)
}
// shoutout to chadGPT for writing this... I take no responsibility for whatever it spewed, right or wrong.
```