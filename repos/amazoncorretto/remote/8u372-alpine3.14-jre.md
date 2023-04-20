## `amazoncorretto:8u372-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:9fb9cac5ca770551cf67353658563102b915e420e5f281a45129dfeab14ae8ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.14-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa4c39cbd784bb24c84035f31d1849a7f2a78f7016d686295b93a450f838c013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43990381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93caffa19d12b47d07e8e30c8a0519335573bde6b80f92f9c217c31aec90bf01`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:02 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:12 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 20 Apr 2023 17:40:12 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94402b2bad8093a058dd0c00c24237fc33fc7f4bcf69c757feb3ee9648c415b1`  
		Last Modified: Thu, 20 Apr 2023 17:48:01 GMT  
		Size: 41.3 MB (41265233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
