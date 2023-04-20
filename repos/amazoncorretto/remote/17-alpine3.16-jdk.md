## `amazoncorretto:17-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:1ddbbc625e62b47f1a99250e03426805ca9019eeb71365fb22708386695ba74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:adcf91786564164f86815fb5c2797492ec9e50f5ca010be53b23994b19c3e9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196377344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c6c416a7107f7e404270d040dc77a7d85a8114e5ca0c27a300b48682278b8fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:18:54 GMT
ARG version=17.0.6.10.1
# Wed, 29 Mar 2023 19:19:00 GMT
# ARGS: version=17.0.6.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Wed, 29 Mar 2023 19:19:00 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:19:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:19:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7d860632aadc8049001eec630273d80a42ad006263ff3a5e1e3c2c4126a934`  
		Last Modified: Wed, 29 Mar 2023 19:26:51 GMT  
		Size: 193.6 MB (193569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:271e220f299f7d50906493198172f9d8993bbd4271d5c3b1d257da82813c98d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194698528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6fb56de89b052dd8363b542a8d1f37430ef5e2d89a6900483d64fbf2e4f0da`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:44:23 GMT
ARG version=17.0.7.7.1
# Thu, 20 Apr 2023 17:44:28 GMT
# ARGS: version=17.0.7.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Thu, 20 Apr 2023 17:44:30 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:44:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:44:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548e58e9cc37dc7a96302135063710d5a49df873057ef4087326bc4d9224fcba`  
		Last Modified: Thu, 20 Apr 2023 17:55:20 GMT  
		Size: 192.0 MB (191989184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
