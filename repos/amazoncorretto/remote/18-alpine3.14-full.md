## `amazoncorretto:18-alpine3.14-full`

```console
$ docker pull amazoncorretto@sha256:7364ff842a6bafaecd1cf44ff2da5a8acfd7ca28bb936093752acc830cd97abb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine3.14-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0e2f673ee014d7dffe6e5cd4b4a544c1448db34b55583fc80a641bceda909399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195688483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d156c6dd20b398b5c5f1e1fcce5e548c51ae60ff8e01acc9e8f0784ec11b20b4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:50 GMT
ARG version=18.0.2.9.1
# Tue, 09 Aug 2022 17:38:56 GMT
# ARGS: version=18.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Tue, 09 Aug 2022 17:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:38:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:38:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35a39b6825c96f12cc216f7426ff04f445f05358acab0289d1bbb9614ddcd14`  
		Last Modified: Tue, 09 Aug 2022 17:46:42 GMT  
		Size: 192.9 MB (192860994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
