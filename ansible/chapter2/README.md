# Password generation

I used this command to generate the SHA512 hash used in the "Create user" task.

```bash
pass=`pwgen --secure --capitalize --numerals --symbols 12 1`

echo $pass | mkpasswd --stdin --method=sha-512; echo $pass
```

example output:
```bash
$6$neHkUxKvA$dBx3.N.UDekgAVfgxtTBpQbTuhvSluXEbxzcM8VvifSVJ.neapI843jkk7COovi5M6YA5DEcXmS53WUEpgtLf1
S^0drP^hHf[V
```
initial hash -
```bash
$6$OStSJfA6FA$ffSDaJBWfSpmnwlC6QWJwLG3PgZWQhPYUSezmRvSiUFpwSWy/57KuUuLg/4yGBpKx2TWYsPDz9Yq7nL2I2XT3/
```
