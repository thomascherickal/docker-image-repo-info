## `amazoncorretto:8u382-alpine3.16-jre`

```console
$ docker pull amazoncorretto@sha256:b1ba5af32a81f4b6a66bb24c200665073c255d9bb3664e1f75416e4169f63073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u382-alpine3.16-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a8e55104ae7effc0adc8dcf559460b57d8d223e8038bfd992257e643714db6de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44339437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15da7f10128cd1080b2cafacf9226d0b27e0a6a0a47c2e3171e3bf247951d4f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:13 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:24 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:24 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5579a471323945ba5e7b700230d672f1e658f9baadcf505ee0867e423953ad`  
		Last Modified: Mon, 07 Aug 2023 19:51:01 GMT  
		Size: 41.5 MB (41531754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u382-alpine3.16-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1b59d78394fbcceda7921a2abe59154c4af2e42ea5a382bd475c9edc3e5bd554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43996069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:140c8d9d683a866875f28b80b61e79d66b84587d47e07dbc3120f66f33b7e080`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:23:07 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:17 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:17 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35379383a9855077b02139baf896ab1c5dd435a34404e51cf5af54f577ad0235`  
		Last Modified: Mon, 07 Aug 2023 20:35:32 GMT  
		Size: 41.3 MB (41288046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
