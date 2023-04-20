## `amazoncorretto:8u372-alpine3.16`

```console
$ docker pull amazoncorretto@sha256:51f70ae4722241f22091f0db00ab475d174fe3b2ac8b2e04a131af6e2b032e04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8643732fb9fd1d34bb9ce605aa0f8eb30fa3dffdae7ecc4c477e0181d544c29a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102478943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4025f60c8f401f38b44fe23981a13d3df3dc369c378cab28ff4f62c0916c7292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:24 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:27 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 20 Apr 2023 17:40:28 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:40:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39a3aae33354103b5febf85596933415f29c62f6e6793d07b74704c2db9bf86`  
		Last Modified: Thu, 20 Apr 2023 17:48:48 GMT  
		Size: 99.8 MB (99769599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
