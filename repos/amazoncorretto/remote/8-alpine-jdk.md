## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:7090e8c16fd0229c4e716a75845925e83d4d4772532fb16aa9119742c770d313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08c47c1f375704565fc6a35f0863d23d7aefcd7f8609e0d28b3c8fb0ab89cf77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103463071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632d98ba4c9841779045b028ee5abc3c05403c451dfc0e108852718eb4c2b1e8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:17:55 GMT
ARG version=8.392.08.1
# Thu, 19 Oct 2023 03:17:59 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:18:00 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:18:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:18:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b60e325470584ed08ef5508e8812b14738c34884b7de313759e6aaea9eaf8d`  
		Last Modified: Thu, 19 Oct 2023 03:34:50 GMT  
		Size: 100.1 MB (100061104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:524a150c094722db68515712347db89860fd0baa57c865a85ca1b4eca805f771
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103138834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d98b0027d10a41918f561b26fcae49ba58b071c2e2b7e6a2bad4a05c550d08f0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:45:05 GMT
ARG version=8.392.08.1
# Fri, 01 Dec 2023 02:45:10 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:45:11 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:45:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:45:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab2166af38afe22ed3728ab432d84b4df35d574d5675a01338894470ad57fb`  
		Last Modified: Fri, 01 Dec 2023 02:49:34 GMT  
		Size: 99.8 MB (99805801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
