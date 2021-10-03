## Specs

You are a college student and you want to stream a movie over one of the campuses Wi-Fi networks. Based on the number of users, some networks won’t have the data to stream a movie.

Use the following `Network` class to track how much total data and how many users each network has:

```js
class Network {
  constructor(data, users) {
    this.data = data;
    this.users = users;
  }
}
```

The properties of the `Network` class are:

`data`: Total units of data supplied by the network
`users`: Total numbers of users currently on the network

Each user on average deducts 5 units from the network’s total data. 

To watch a movie you must connect to a network that has at least 50 remaining units of data.

To using video call and conference you must connect to a network that has at least 10 remaining units of data

For the connection, system will disconnect every 60 minutes and pop up `alert` to the user

- Add a method `movieTime()` to the `Network` class that returns `true` if there is enough data available to watch a movie, `false` if there isn’t.

- Add a method `videoCall()` to the `Network` class that returns `true` if there is enough data available to using video call and conference, `false` if there isn’t.

-  Add method `disconnect()` to the `Network` class that will show string `"You must reconnect the Internet Connection"` using `alert` every 2 minutes of the connection for the simulation (in the real case usually 60 - 120 minutes)

## Expected Result
```js
const library = new Network(50, 8) 

library.movieTime() // returns false
library.videoCall() // returns true and show alert from `disconnect()` method after 2 minutes
```

