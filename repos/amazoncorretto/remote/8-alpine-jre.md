## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:7934f54c28f94710fb96f5ac9b862244159fe65cf464f91b07c983cf1e9bcc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c25db82e7c7066dc0a36088a42943abd328fde25d0f4e46e689d088dd8b68696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44940628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798848703d887c04d3d6abdf841bf67defe90721fed68187116db11622d92c85`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:17:55 GMT
ARG version=8.392.08.1
# Thu, 19 Oct 2023 03:18:07 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:18:07 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:18:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abe48b800380b92380000558d3c8bf38e16b49edebeae228decd9c7ad1a7db4`  
		Last Modified: Thu, 19 Oct 2023 03:35:17 GMT  
		Size: 41.5 MB (41538661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:aea41bb62f426b0b419e861ebfac767d214ea3814585d5336471c5e01fff3e4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44622018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab7b9050d951729ff487203fc04778ddae83745c2efba488fc0a353a221dc75f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:45:05 GMT
ARG version=8.392.08.1
# Fri, 01 Dec 2023 02:45:18 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:45:18 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:45:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327f1ca92b465b77135e5763d1c0cf1a05367872f2fc81686aab663e7e482f13`  
		Last Modified: Fri, 01 Dec 2023 02:49:56 GMT  
		Size: 41.3 MB (41288985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
