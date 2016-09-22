This utility will fetch all the file names and sizes from a s3 bucket in a specified region.

USAGE:
```
s3ls bucketname [region]
```
EXAMPLE:
```
./s3ls ourbucket us-west-2
1692           testa.pem
1696           testb.pem
1696           testc.pem
1696           testd.pem
3976           dira/a.json
4346           dirb/b.json
4629           dirc/c.json
4781           dirc/b.json
5461           dird/d.json
5622           dire/e.json
16664          dirf/version1.json
32934          dirf/version2.json
Bucket has 12 items.
0.09 Megabytes total space used.

```

The region defaults to us-east-1 if unset.

You can set your AWS credentials through all the standard methods, i.e. environment variables or a credential file.

Glide installation:  If you don't have all the dependencies installed, you can use [glide](https://github.com/Masterminds/glide) to install them in a vendored location.
```
glide up
go build s3ls.go
```
