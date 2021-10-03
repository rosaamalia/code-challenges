## Specs

A Squid Game consists of two players floating using 100 marbles. The players shoot at each other’s marbles and after 10 minutes the player with the most marbles left wins.

```js
class Player {
  constructor(name, hitsPerMinute) {
    this.name = name;
    this.hitsPerMinute = hitsPerMinute;
    this.marbleCount = 100;
  }
 
  status() {
    console.log(`Player: ${this.name} -- Marbles Left: ${this.marbleCount}`)
  }
}
```

Write a game function `marbleAttack` that takes two `Player` instances, calculates the marble left for each player after 10 minutes (using the `hitsPerMinute` property) and returns the name of the winner. If the result is a tie, return the string `'Tie'`.

You can test your `marbleAttack` function by creating two instances of the `Player` class to use as arguments for your function like below:
```js
const p1 = new Player('p1', 5);
const p2 = new Player('p2', 2);
 
marbleAttack(p1, p2);
```

Feel free to use the `status()` method to output each player’s balloon count at any given time.

## Expected Result

```js
const p1 = new Player('p1', 5);
const p2 = new Player('p2', 2);
 
marbleAttack(p1, p2); // return p1

const p3 = new Player('p1', 5);
const p4 = new Player('p2', 5);
 
marbleAttack(p3, p4); // return Tie
```