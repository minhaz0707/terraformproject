 provider "aws" {
  region     = "ap-south-1"
  access_key = "AKIA6OVGHU2VVYH4H7H7"
  secret_key = "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"
}

resource "aws_instance" "SERVER11" {
  ami           = "ami-079b5e5b3971bd10d"
  instance_type = "t2.micro"

} 

data "aws_ami" "ec2_ami" {
    most_recent = true

    owners = ["amazon"]

    filter {
        name = "name"

        values = ["amzn2-ami-kernel-5.10-hvm-2.0.20220426.0-x86_64-gp2"]
    }
}

