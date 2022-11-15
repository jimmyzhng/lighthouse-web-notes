### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```

### My code

```
const whatToDoForLunch = function(hungry, availableTime) {
  if (!hungry) {
    console.log("Get back to work!!!");
    return;
  }

  if (availableTime < 20) {
    return console.log("Pick up a snack or grab something you have ready at home.");
  }

  if (availableTime <= 30) {
    return console.log(
      "You deserve a break, and should take time to cook a tasty meal."
    );
  }

  console.log(
    "You sure about that? We're in a bootcamp, and you do not have that much free time."
  );


};
```

Through a brief conversation with Gary J, I learned the importance of avoiding the usage of "else" in situations where mutually exclusivity is not present. He was able to quickly clean up my code, and gave me some great advice about how to approach the question.