This utility will fetch all the file names and sizes from a s3 bucket in a specified region.

USAGE:
`s3ls bucketname [region]`

The region defaults to us-east-1 if unset.

You can set your AWS credentials through all the standard methods, i.e. environment variables or a credential file.

Glide installation:  If you don't have all the dependencies installed, you can use glide to install them in a vendored location.
```
glide up
go build s3ls.go
```
