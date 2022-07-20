## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:e2b6137d42add09301499f0747ab073916127942ffa140896870e8c0c868be15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4c816a5490d1e68862b9c1f304f652333fd54620be4525d223809289f8a6c908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43252527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d722add027e112a09491347d634993fe8e1e0a4e90a7c29a7be2c5f8b04189`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:37:23 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:33 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 19 Jul 2022 22:37:34 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2365bab9942a6fdfb86acfa1955c2b153a873deaf9ecc2ceb6d12df32501439`  
		Last Modified: Tue, 19 Jul 2022 22:44:06 GMT  
		Size: 40.4 MB (40437882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
