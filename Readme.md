Subject:

Select All elements (#id or .class):
```
  const listOfAllDice = document.querySelectorAll(".die");
```

Select element by Id
```
  const roundElement = document.getElementById("current-round");
```

Arrow Function:
```
  const rollDice = () => {}
```

Event Listener:
```
  rollDiceBtn.addEventListener("click", () => {});
```

For Loop:
```
  for (let i = 0; i < 5; i++) {}
```

For of Loop:
```
  for (const num of arr) {}
```

Time Out Function:
```
  setTimeout(() => {
          alert(`Game Over! Your total score is ${score}`);
        }, 500);
```

Sort Numbers in an Array:
```
const sortedNumbersArr = arr.sort((a, b) => a - b);
```

Remove Duplicate values in an Array:
```
  const uniqueNumbersArr = [...new Set(sortedNumbersArr)]
```

My Logic Version of the Function:
```
  const checkForStraights = (arr) => {
    const sorted = [...new Set(arr)].sort((a, b) => a - b);
    let count = 0;

    for (let i = 0; i < sorted.length - 2; i++) {
      if (sorted[i] === sorted[i + 1] - 1 && sorted[i + 1] === sorted[i + 2] - 1) {
      count++;
      continue;
      }
      if (count === 2){ 
        continue;
      }
      count = 0;
    }

    if (count === 3){
      updateRadioOption(4, 40);
    } 
    if (count >= 2){
      updateRadioOption(3, 30);
    } 
  }
```
