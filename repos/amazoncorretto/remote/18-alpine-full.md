## `amazoncorretto:18-alpine-full`

```console
$ docker pull amazoncorretto@sha256:a7a3987a45a4f6666971953b3839d00cda354eb703711f25f8217c3a2d895704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:52679264dee28c1cbe2ff8455efc86cc44cbceb6f94d9971abd7cd7e4c8bdc50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.8 MB (195780859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6cb1ff0ea94c1f4b7a7ea5a579e65f706c40c3bdd1cc98895b6c7457cc3770`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:27:14 GMT
ARG version=18.0.1.10.1
# Tue, 19 Apr 2022 22:27:20 GMT
# ARGS: version=18.0.1.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Tue, 19 Apr 2022 22:27:21 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:27:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:27:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a57c8e96cbc4fcccd45380975228c790db70513e0b8e6a6bdcbe6aea43f527f`  
		Last Modified: Tue, 19 Apr 2022 22:39:31 GMT  
		Size: 193.0 MB (192966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
