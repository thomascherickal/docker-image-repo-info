## `amazoncorretto:8-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:57b1bf560d8f8e1f817eb1be91270de545a0016fcfb2f0d7d3c3de2b04580bd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:64a4f9f24ac35903ce16a4ad17f4a6f94b4e44b268b8a971ef4ddf5f63057115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101614570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d23b1cc9146a069f5d580aa0e47bde72c44644247553d34f310f872c120102d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:37:23 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:27 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Jul 2022 22:37:27 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:37:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d9180e88f4cc3ef7b950eae90122524c97f9f36f36d5d938914b174b95124e`  
		Last Modified: Tue, 19 Jul 2022 22:43:39 GMT  
		Size: 98.8 MB (98799925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
