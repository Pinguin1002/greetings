Saludos en Go 
Este paquete proprociona saludos 

##Instalación
Ejecuta el siguiente comando para instalar el paquete:

```bash

go get -u github.com/Pinguin1002/greetings

```

##Uso
Aqui tienes un ejemplo de como utilizar el paquete:

```
package main

import (
	"fmt"
	"log"

	"github.com/Pinguin1002/greetings"
)

func main() {
	log.SetPrefix("greetings:  ")
	log.SetFlags(0)

	names := []string{"Memo", "Liss", "Ana"}
	messages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}
	fmt.Println(messages)
}

```