## `amazoncorretto:8u342-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:43a58266c9d87b48e74c0597d3f63c08a545b1ac6a5773e6715618392a0323f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u342-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8a1ff678d2ee7d2ae5200d175ff3ea15325be6b9c717f5dff4f09a9d172ad8de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43263056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb90055346e42df327648e08bfc154c74734dce44d08141652a6909c7f0f462`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:34:52 GMT
ARG version=8.342.07.4
# Thu, 06 Oct 2022 19:35:02 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 06 Oct 2022 19:35:02 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:35:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabff8883c2e32c215e5ebe5480cf498feb227ff9558ea9d0e672682eabb029b`  
		Last Modified: Thu, 06 Oct 2022 19:41:53 GMT  
		Size: 40.4 MB (40439544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
