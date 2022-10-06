## `amazoncorretto:19-alpine-full`

```console
$ docker pull amazoncorretto@sha256:7f44001170267d97203ecf4cab6b4787a3a68b457c7179a1e21abb65f2742357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:19-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f320eb0a38e11cd7aac76cbf9c6cf5c2394647fd64b41db66fc581ad689b7a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.0 MB (203022942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8564224c5b4ca87cc050376a2560ab9cf4808ab8bab6fb4c74faf1f49ecca0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:38:01 GMT
ARG version=19.0.0.36.1
# Thu, 06 Oct 2022 19:38:07 GMT
# ARGS: version=19.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-19=$version-r0
# Thu, 06 Oct 2022 19:38:08 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:38:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:38:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db9389f83463108ce2d6c6a9d068d8c118e9a767fc931817af61c10e38cdf6b`  
		Last Modified: Thu, 06 Oct 2022 19:50:48 GMT  
		Size: 200.2 MB (200216888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
