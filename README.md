# #2 Simple Web Server

Simple Web Server is a Golang project to display simple hello webpage, form webpage, and server page. 

This project uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the World Wide Web.

## Tools

[golang](https://go.dev/dl/go1.19.darwin-amd64.pkg) to install golang and check for go version.

[html](https://html.com/) for html documentation

```bash
go version
```

## Code 

```golang
import (
	"fmt"
	"log"
	"net/http"
)

# form webpage
func formHandler(w http.ResponseWriter, r *http.Request) 

# hello webpage
func helloHandler(w http.ResponseWriter, r *http.Request)

# main server
func main() {
	fileServer := http.FileServer(http.Dir("./static"))
	http.Handle("/", fileServer)
	http.HandleFunc("/form", formHandler)
	http.HandleFunc("/hello", helloHandler)
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[LYFEYTECH](https://github.com/lyfeytech)
