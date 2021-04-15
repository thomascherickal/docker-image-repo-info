## `amazoncorretto:8u282-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:b1cc14a69a3e00909ba63458b63b4ca6f613480c4fdcf3b0572ecd3455949427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:72401e3e80c4bf9379ba28872437fc4b1cd5063215d557cbcf058b5116213697
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43116550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4651e9a1a21544bcf9ad95549befa33b9b4188bf63f043a614ce95d9586353`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:38:39 GMT
ARG version=8.282.08.1
# Wed, 14 Apr 2021 19:38:50 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 14 Apr 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Wed, 14 Apr 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a890d0b48812a686656338dab896e2d1fa60066211b474ca5deb03ff5e2eedd6`  
		Last Modified: Wed, 14 Apr 2021 19:41:34 GMT  
		Size: 40.3 MB (40315983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
