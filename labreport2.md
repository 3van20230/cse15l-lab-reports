PART 1
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    private static StringBuilder chatMessages = new StringBuilder();

    @Override
    public String handleRequest(URI url) {
        if (url.getPath().equals("/add-message")) {
            String user = url.getQuery().split("&")[1].split("=")[1];
            String message = url.getQuery().split("&")[0].split("=")[1];
            addMessage(user, message);
            return chatMessages.toString();
        }
        return "404 Not Found!";
    }

    private void addMessage(String user, String message) {
        if (user != null && message != null) {
            chatMessages.append(user).append(": ").append(message).append("\n");
        }
    }
}

class ChatServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}

```

