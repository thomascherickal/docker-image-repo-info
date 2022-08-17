## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:77675e4ccda47f136090966b00f271d4c194bde8fb2d901929d99ac18e553ce4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:aa9ed5ca43fe371320f50bf47b27c5f6d8b3b83c2302c5c54778dcaa7643ccbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196032833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:283ddb4a3d7a6aaefe443829f2fe0ec3a90e874167be5700853e8216516b6d54`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:20:32 GMT
ARG version=11.0.16.9.1
# Tue, 16 Aug 2022 23:20:38 GMT
# ARGS: version=11.0.16.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 16 Aug 2022 23:20:39 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:20:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:20:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965691d554a32a0bd7fe0064d0d0feff899c69ff4979fcb383fc00f5fb5b628`  
		Last Modified: Tue, 16 Aug 2022 23:25:09 GMT  
		Size: 193.2 MB (193209321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
