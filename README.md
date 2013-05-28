### setup s3cmd

```
git clone git://github.com/s3tools/s3cmd.git
cd s3cmd
python setup.py install
// check
s3cmd --help
s3cmd --version
```

### sync to s3 and cloudfront

```
s3cmd sync --cf-invalidate --cf-invalidate-default-index --acl-public --recursive <directory> s3://<bucket name>
// check output for invalidate state check command
```