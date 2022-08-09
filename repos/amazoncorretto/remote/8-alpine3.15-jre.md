## `amazoncorretto:8-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:6be84126fac97770531652833a6cb7696667237a41e7f1ed8d87a49b5b175f2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:89dcbe5103ad0fd420881ad1f2dd4d0627d5b930153c3869162ebea7b2e5c013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43263037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2951bb00c413a9938ce24c3ad71ff91ce8f7a1736cf294aee0c8de8df2acfb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:37:16 GMT
ARG version=8.342.07.4
# Tue, 09 Aug 2022 17:37:27 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 09 Aug 2022 17:37:28 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:37:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ded0c8d65125226422f93f2696d1e8f4309bc7decd1aef61edba1c88f234dc`  
		Last Modified: Tue, 09 Aug 2022 17:42:28 GMT  
		Size: 40.4 MB (40439525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
