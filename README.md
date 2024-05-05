Run the server with:
```
cargo run --bin server
```

and the client with:
```
cargo run --bin client
```

![Running](https://cdn.discordapp.com/attachments/314315831465213953/1235902534602981396/image.png?ex=66360f6e&is=6634bdee&hm=243f952bbcbf29572fbbc2ea79c95b9bffc52180cea4535a5f1dedff8a21a68a&)

If I type something into each client each message will be sent to the server, printed by the server, and then sent back to the client that sent it.

The WebSocket protocol is defined by the `tokio_websockets` crate that is being used. This crate provides the `ClientBuilder` and `Message` types that are used in the client code.

![Modify](https://cdn.discordapp.com/attachments/314315831465213953/1236579135426658325/image.png?ex=66388590&is=66373410&hm=85f09d779a00e8f9ebbb1df1d9e118caf7c28ae1552924b581a877087fec73cf&)

We add a `username` variable and pass it as a command-line when starting the client. 