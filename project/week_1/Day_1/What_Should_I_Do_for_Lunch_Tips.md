### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
let whatToDoForLunch = (hungry, availableTime) => {
  let a = '';
  if (hungry === false) {
    a += 'not hungry';
    console.log('wait till you are hungry');
  } else if (hungry === true && availableTime < 20) {
    a += 'hungry';
    console.log('pick up a snack or grab something you have ready at home');
  } else if (hungry === true && 20 <= availableTime && availableTime <= 30) {
    a += 'hungry';
    console.log('you deserve a break and should take time to cook a tasty meal');
  } else if (hungry === true && availableTime > 30) {
    a += 'hungry';
    console.log('this is an intense program after all and you should probably reconsider.');
  }
  return 'Im ' + a + ' and I have ' + availableTime + ' minutes for lunch.';
};
```