# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

The function below takes the input of actualAge and first checks if it is equal to 1. If it does equal 1, it returns catYears and dogYears as 15 and humanYears as 1. If not, it continues to the next portion and checks if it is equal to 2. If it is, you'll return humanYears: 2, catYears: 24, and dogYears: 24. If neither of those functions are true, your value will be entered in the final bit of the function where your value is put through an equation to return a number. 

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input |                   Output                          |
| ----- | ------------------------------------------------- |
|  10   | humanYears: 10, catYears: 56, dogYears: 64        | 
|   3   | humanYears: 3, catYears: 28, dogYears: 29         | 
|   2   | humanYears: 2, catYears: 24, dogYears: 24         | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program takes an input of actualAge and gives you an output of actual age in human years and converts it to dog years and cat years.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
