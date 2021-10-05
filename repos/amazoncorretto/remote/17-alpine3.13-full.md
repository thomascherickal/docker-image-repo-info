## `amazoncorretto:17-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:ab822969957d5f6acaa68e566525b0f572d7589b0240501a77cd68646e8d1875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a2c5618e903e87c80f5c3540980def71a9bb81a30fdead5943696106d132f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198920038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386146034be35cc90fd05ee718cd1999da1d1fca109cbef95aece44ffc7e187b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 05 Oct 2021 17:20:22 GMT
ARG version=17.0.0.35.1
# Tue, 05 Oct 2021 17:20:29 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 05 Oct 2021 17:20:30 GMT
ENV LANG=C.UTF-8
# Tue, 05 Oct 2021 17:20:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 05 Oct 2021 17:20:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a81fc33cae0d3c1fa5b4ff6e468c8579c2f70487cd25ce0117b699f00cf450`  
		Last Modified: Tue, 05 Oct 2021 17:26:41 GMT  
		Size: 196.1 MB (196105959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
