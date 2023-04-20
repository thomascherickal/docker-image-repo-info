## `amazoncorretto:8u372-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:3953e40efc699ca07ce25ef75572eee1058e5accd12a89876f20939fbb765ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d0f8018b7765da7cbf49b99f6977f7fe23f8a33546099a61de8ace34223ec68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102492038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ca821fa3d9240e545e9e4c52096f9e857862a005e69b76c0ae81966b1156ef`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:13 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:17 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 20 Apr 2023 17:40:18 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:40:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e3a79bb57074fce6db10791aa95c1ef09f6ae4824ea19397974f5ae057b06a`  
		Last Modified: Thu, 20 Apr 2023 17:48:16 GMT  
		Size: 99.8 MB (99770036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
