## `amazoncorretto:8u382-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:8bdd1666a485b37cb6ff20a6d8f2c86e59c391fe5453dffd79db589eb225521a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u382-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e04f300c754fa70e61d0cd09357de53117b33440f272394c5ad3a569bcaa2490
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44357876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0483453783d06af806db96f09f4b11812168574d26ae7533d83d6a47426d6ead`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:00 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:10 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:10 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af6727a6d510fec00e04679aa8a152ec404e6ce359275900d9d9d44e2165927`  
		Last Modified: Mon, 07 Aug 2023 19:50:25 GMT  
		Size: 41.5 MB (41531870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u382-alpine3.15-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d7eea8c3bdb44c02f6e68eb3869d5e7fecf43ff871e168808c14ce6a1cbf958f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44009135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b18ccca5ddf1aaa9ed7fd6b52f6cdaebc19678ea745d97f9d07abf805e51e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:22:56 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:05 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:05 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acd72a78453db05596b55a8bbace5e034cab6d2075b560d118f5298efaf39d`  
		Last Modified: Mon, 07 Aug 2023 20:34:55 GMT  
		Size: 41.3 MB (41288267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
