FROM golang:1.21 as builder
WORKDIR /src
COPY <<EOF ./main.go
package main
 
import "fmt"
 
func main() {
  fmt.Println("hello, world")
}
EOF
RUN go build -o /bin/hello ./main.go
 
CMD ["/bin/hello"]