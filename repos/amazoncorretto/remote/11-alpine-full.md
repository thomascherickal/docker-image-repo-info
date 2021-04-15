## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:0ab02867f1b7a0bef119f284a2922f20f7aa50dd501e023b063a9ca2ac1c959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:bbb7581d68254b05ec7d6fafa68af22701b6cbb3fdce53e45d5fab85471d1fb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195087944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0727713de19bed425d50af8f1ff96eb336fbe16990074ac14fe340c1a1e94b23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:38:54 GMT
ARG version=11.0.10.9.1
# Wed, 14 Apr 2021 19:39:00 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 14 Apr 2021 19:39:01 GMT
ENV LANG=C.UTF-8
# Wed, 14 Apr 2021 19:39:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Apr 2021 19:39:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c496f1543a6cf36a79305de7c709ea55c16b63ea86219c4b98c334b70488d`  
		Last Modified: Wed, 14 Apr 2021 19:42:02 GMT  
		Size: 192.3 MB (192287377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
