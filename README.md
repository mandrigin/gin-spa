# gin-spa
A simple SPA (single-page application) serving for gin-gonic.


## Usage

```go
package main

import (
	"github.com/gin-gonic/gin"
	"github.com/mandrigin/gin-spa/spa"
)

func main() {
	r := gin.Default()
	r.Use(spa.Middleware("/", "./static/spa")) // your build of React or other SPA
	r.Run()
}
```
