# ntt (nim typing tutor)
A typing tutor website in nim 

### will update this 🔜 🔜 🔜 


### Predefined Text Challenges
We’ll create a set of predefined texts for the typing challenge.
```
const challenges = [
  "The quick brown fox jumps over the lazy dog.",
  "Nim is a statically typed compiled systems programming language.",
  "Jester is a simple and powerful web framework for Nim."
]
```
### Start the Test
```
proc startTest() =
  startTime = epochTime()
  correctWords = sampleText.split(" ")
  typedWords = @[]
```

```

var startTime: Time
var typedWords: seq[string]
var correctWords: seq[string]
var inputText = ""

# Words to test typing speed on
let sampleText = "The quick brown fox jumps over the lazy dog"

proc startTest() =
  startTime = epochTime()
  correctWords = sampleText.split(" ")
  typedWords = @[]

proc calculateSpeed(): int =
  let endTime = epochTime()
  let timeTaken = (endTime -startTime).float / 60.0 # Minutes
  return int(typedWords.len.float / timeTaken) # Words per minute
```

- expand this application by adding more features such as:

- Adding a typing challenge page with predefined texts.
- Calculating typing speed (words per minute).
- Creating a web-based interface using HTML/CSS for better user interaction.
