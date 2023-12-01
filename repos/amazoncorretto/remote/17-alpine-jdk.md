## `amazoncorretto:17-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:4caf8c150836393a500eef522bd94499f43cc75b1dca294d036237470b52f8dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:df48bf2e183230040890460ddb4359a10aa6c7aad24bd88899482c52053c7e17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149005324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8efd4627b3a15e27b555c4a74b51f28f0fb710367aa20a1dacfb3978e67f70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:26:18 GMT
ARG version=17.0.9.8.1
# Thu, 19 Oct 2023 03:26:25 GMT
# ARGS: version=17.0.9.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:26:25 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:26:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:26:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3e82fee6c9df6e81df760df601510e1821f6f84f3dc0956a5b3fbe5f5cb5a9`  
		Last Modified: Thu, 19 Oct 2023 03:43:46 GMT  
		Size: 145.6 MB (145603357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:77133e85578e287190f991a7ecb7357fb9df6dd27d03d43a9f2cb05b8688f5ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.3 MB (147347260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439116aa67f8f9e06521b0999e31c04cf566c7fc71b1153087949c5c078c4517`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:46:33 GMT
ARG version=17.0.9.8.1
# Fri, 01 Dec 2023 02:46:38 GMT
# ARGS: version=17.0.9.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:46:40 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:46:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:46:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7959a0748edc5c4e60be561f317589456f47dd903864e189ba8059bff388bdf`  
		Last Modified: Fri, 01 Dec 2023 02:52:20 GMT  
		Size: 144.0 MB (144014227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
