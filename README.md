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