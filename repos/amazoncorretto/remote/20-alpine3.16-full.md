## `amazoncorretto:20-alpine3.16-full`

```console
$ docker pull amazoncorretto@sha256:519a7d7fd4a3bd0c2619ede92948a9e293153abca55fc86ca1b99352abe57272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.16-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:feb7cab16d5ae82ec963f936873ba74af8a75bf522b03ad1f6b19fe13f0fc028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.4 MB (206432430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb22609621b070deba7ef93f8ba905b644f1a5571de797e16d0fbef8ec632e74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:36:43 GMT
ARG version=20.0.1.9.1
# Thu, 15 Jun 2023 05:36:48 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Thu, 15 Jun 2023 05:36:49 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:36:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 15 Jun 2023 05:36:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76697dccf99ffbb27165787f646616bed7ba20669fd93e86ab773148ad84b4c3`  
		Last Modified: Thu, 15 Jun 2023 05:43:29 GMT  
		Size: 203.6 MB (203624761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.16-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:717288c7c05b92c6e55da9b6a795f74f23df1f77f8a7e9d2b9e840d69cdf67de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.4 MB (204439842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006630b4349717080b612ac8e96e55f9f32b9d8fe322943bb59081010e0c9e49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:09:48 GMT
ARG version=20.0.1.9.1
# Wed, 14 Jun 2023 22:09:54 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Wed, 14 Jun 2023 22:09:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:09:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Jun 2023 22:09:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4223ebd2f7efd0ab65dbe19f6cae73f5afcd74b119313e7845909a993fc14f88`  
		Last Modified: Wed, 14 Jun 2023 22:16:21 GMT  
		Size: 201.7 MB (201731936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
