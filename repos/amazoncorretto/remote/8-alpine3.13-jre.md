## `amazoncorretto:8-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:d5216bf119d9145bacf3818a97f9bb47924dba3f4bdf2975992764dcea1fbf9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4dc6944435cc0b4332ae1c7f2bbd4dbcf985f9823adf28d67d8b10fb606600d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43162525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa21fe9930b7d0a9a97ca04a78f793603e956280f8dadbbb700a35f342c86080`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Sat, 02 Oct 2021 01:19:37 GMT
ARG version=8.302.08.1
# Sat, 02 Oct 2021 01:19:49 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Sat, 02 Oct 2021 01:19:49 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 01:19:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb89002459d6d2118787abde6ce4cea8c6ddae8492f18fc5125f118116f5fab`  
		Last Modified: Tue, 05 Oct 2021 17:22:44 GMT  
		Size: 40.3 MB (40348446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
