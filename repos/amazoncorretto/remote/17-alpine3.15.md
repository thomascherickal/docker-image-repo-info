## `amazoncorretto:17-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:dd3a117328e6f8e5194eac0d1e5ff92b968e2ee09aed909582616d43d700d190
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:590c94a776892a514a28b7232b6646a80bb67166cd4e233ee0c495b053093448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196396024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90268ccf1e2417b388e6418cc2ba64797d4893115b8e87aab0d348327ed77043`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:18:46 GMT
ARG version=17.0.6.10.1
# Wed, 29 Mar 2023 19:18:51 GMT
# ARGS: version=17.0.6.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Wed, 29 Mar 2023 19:18:52 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:18:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:18:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c73a1cccb8b02449f83f7fb04eace4dc3fa8794ad95f6f3b23afb613542e43b`  
		Last Modified: Wed, 29 Mar 2023 19:26:25 GMT  
		Size: 193.6 MB (193569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c49263a8e50a4fc8ce159021a3f88859c2a4a5d15b08f1cb9d129101b97ba473
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194711557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccdc9d86cecbea9d2b13898e47404e10e97d256541bec4f409d57f61c0a5da97`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:44:14 GMT
ARG version=17.0.7.7.1
# Thu, 20 Apr 2023 17:44:19 GMT
# ARGS: version=17.0.7.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Thu, 20 Apr 2023 17:44:21 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:44:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:44:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787d7ee7fd5ab1bdce644ab08f79f4f1910b8e32d165a728721fb0a4c1a02e5`  
		Last Modified: Thu, 20 Apr 2023 17:54:56 GMT  
		Size: 192.0 MB (191989555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
