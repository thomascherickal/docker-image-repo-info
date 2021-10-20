## `amazoncorretto:8-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:1a3f37f4cd3102a1b12256191b29171238bf20d6a9e574deb0f656990b913440
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5f7c09dedaf02836c47c9996b266fe3ce34bf9705dd4bd29d203cbfa22101134
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101869012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1648c6aacf5eb6ab7a0717392a620994da5a787f694b23240946e2d5460966`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:20:19 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:20:23 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 20 Oct 2021 18:20:23 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:20:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:20:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cd4a8f8421355f43e10b181ca36b0a22621b94da2d40d5fab7e7b261d6921`  
		Last Modified: Wed, 20 Oct 2021 18:25:17 GMT  
		Size: 99.1 MB (99054566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
