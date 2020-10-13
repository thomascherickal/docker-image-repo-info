## `amazoncorretto:15-alpine-full`

```console
$ docker pull amazoncorretto@sha256:bc52c0002cf2982ff8a3635e4abcd1d7075ac4fbe1348446e812a7b49bc6ae02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2610ccc798acfabc6fe0eaabc826791dc5c247838248ba6bb68d96d26427ec55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207694943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ea94061bc9b4edc8bb17a4ce9960b1c9ffdfc9e996f4c35eb444d61688c057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 12 Oct 2020 23:20:14 GMT
ARG version=15.0.0.36.1
# Mon, 12 Oct 2020 23:20:24 GMT
# ARGS: version=15.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Mon, 12 Oct 2020 23:20:24 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 12 Oct 2020 23:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a7ca4ddf82070ebcb8ebb450bf522384130967f4d6dbe499f850cd869adaa2`  
		Last Modified: Mon, 12 Oct 2020 23:21:50 GMT  
		Size: 204.9 MB (204897402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
