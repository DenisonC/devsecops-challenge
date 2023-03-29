Com a Amazon Web Services (AWS), vamos utilizar o terraform como IAC para o provisionamento da instância EC2
-----------------------------------------

Para provisionar uma instância EC2 na AWS usaremos o seguinte arquivo que está localizado neste diretório "main.tf"

```ruby
provider "aws" {
  region = "us-east-1"
}

resource "aws_instance" "example" {
  ami           = "ami-0c94855ba95c71c99"
  instance_type = "t2.micro"
}
```
