<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:2022.1`](#bonita20221)
-	[`bonita:2022.1-u0`](#bonita20221-u0)
-	[`bonita:2022.2`](#bonita20222)
-	[`bonita:2022.2-u0`](#bonita20222-u0)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:7.14`](#bonita714)
-	[`bonita:7.14.0`](#bonita7140)
-	[`bonita:7.15`](#bonita715)
-	[`bonita:7.15.0`](#bonita7150)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:74600c1b8fdd9e9da6ea7d1846ed66fe53eb58b1f8010c18e1ae298ca8b3a7c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:852b5df555a8386f4fd700ce082cc5d7e71114541aef4dd4911ba29f3ede1792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235217428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dab908e3e1e86566a9dc2e1596e0607b8530e5403b271ce80ca9349e9ead4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:06 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 02 Mar 2023 03:18:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:08 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 02 Mar 2023 03:18:08 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:08 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 02 Mar 2023 03:18:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 02 Mar 2023 03:18:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 02 Mar 2023 03:18:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 02 Mar 2023 03:18:20 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:18:20 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:18:20 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:18:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b184c9242594a7a061169b3421fc262998de1c5a8915d9c6498e2a0ccbdec`  
		Last Modified: Thu, 02 Mar 2023 03:19:45 GMT  
		Size: 91.6 MB (91573680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16a7b46a4018d71f769d60de0e03b74b1956aec2bd85f107278a759042918cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9823443109d9c74449d689c0f969bedb664341da0b074eb5b9ca191377afb5`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c56556e15411a3080cb298dc4f120b64e46c2ebbd0345c878a0184f096aba`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 506.4 KB (506351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e594029d02a66ca0ec3a57cf6caca8deff2fd287f00d768510e497c6fda0c3cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228133fa44f5f22935c7e704e20a56d74b6e000411c94e4672441bcdc967c9e3`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29c2cd8efefaa621d032e36351382b6b83a9d1d48d2df20275d713cd0449b`  
		Last Modified: Thu, 02 Mar 2023 03:19:36 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3460cc22df94fcecdfd7a2b57b08d58ff845fd633a093b7c85eca8ffa9a3594`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8902dc37b5c4d6e783edf42d065a619344e60e432ab99982d40925778877fd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226708998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c825d83cc31c6a32cec944449692b27b880cff76bf3381802d28a76a891a5c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:44:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:00 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:00 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:03 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 01:45:04 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 01:45:05 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:05 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 01:45:08 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 01:45:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 01:45:10 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 01:45:10 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:10 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:10 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae5733be1a47f93cf4115c8eb5d708ebba97340bdd829e28046dc600693677`  
		Last Modified: Thu, 16 Mar 2023 01:46:30 GMT  
		Size: 86.1 MB (86072244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f734a0f60abf1e27fac341a223580695dfe5f73b334ff706732361b8184c045`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720974a9ce140f380e608ab07d8c0ef57f711bbdec59ef43f666f2dba7a58e4c`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6af71e6e130e039dbf9930a47790d5022d3c7caeea6e0b4c56011f460705e96`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 475.8 KB (475801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05332412e688d0adb5a302bf1e48e3dbffdb93791382f9db44c640864f87b4`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162842b43ce25faf3fe11d9ebed13d4abce346ca2247d4a82035dd4d0c3bacb`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e702678d0a20a29376f82c8f237e5dac8d61c8adb6c14cb015a030f9e51af59`  
		Last Modified: Thu, 16 Mar 2023 01:46:24 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f6a37ae7d6569119ec6010cb19ce29652e71dcef93be8303070a6304cbc67e`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad6a2eed1730df305984d2d08e2b6d05d664f5486666ff3d6ce2fcd62d7f3e68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234217649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1deb6a96b55e268c39555e677ecd02eaa45a10110c6b72b724d83a023de9b6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:11 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:00:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:00:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:00:22 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:00:25 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 03:00:26 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 03:00:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 03:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:00:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 03:00:35 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:00:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 03:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 03:00:47 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 03:00:49 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 03:00:49 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:00:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:00:50 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:00:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf534da892a5857363836b577335a4b6c17a5b42a1a7ea1ff52630df1c6ec3`  
		Last Modified: Thu, 16 Mar 2023 03:04:30 GMT  
		Size: 86.9 MB (86874102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86733899243167c2217ab5a8c14cc3e45516beb302d293a31b9766445e7515b1`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bd5f53e9da1a5f4b8e9693a01f1628e5ab2d15f651c6ef925739beb14d064b`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bccc4039a31c40a2b9b85bb4cb543a3efb9416fd195edbe23404565d37c381`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c590139130e876e3d5d93370b50f0548036e3de1bee12f237950a476b5ec20`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd9505d0a45154d01bbab1b4091b6e9e462466c514b6b8d4b87f8a11b2f658d`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd74d70744e2ec85d5265ef1c01012ac2cf6baffec913859a505dbbb449b073`  
		Last Modified: Thu, 16 Mar 2023 03:04:16 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5388d68c3974a11bcf5fff3dfa9dabc966f61e6c1bcf1a66374a8a1ca7ab8377`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:d90b60ec75b897585175c6ef9b3bd346247ed412baa81f8dac0248d5072b4c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:571941485e105cf84e94a41c4ba2d70adc7485eca711c139581d538cda2b3695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232950406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c818075063cf50ec77f179e29187fdc568eb8d5b781f6e0c2295c119a6a5b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:56 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 02 Mar 2023 03:18:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:58 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:58 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 02 Mar 2023 03:19:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 02 Mar 2023 03:19:08 GMT
ENV HTTP_API=false
# Thu, 02 Mar 2023 03:19:08 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:19:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:19:09 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:19:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79eb0557cffad3694c73b9238f740363322edda3463516b85107dfd5f03943b`  
		Last Modified: Thu, 02 Mar 2023 03:20:10 GMT  
		Size: 91.6 MB (91573658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65108a5e0ec07ffe53e285cf5bf0ad0ea470da18c1aab99e8e8bcec75274e1`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879bcd0356cfb8fd5e06e48295068b03787757e3cd18e28aaa23097caca64b`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782965c7157ba1f09a12b9582dc4c36bcaf6869972f8ec062d55ac5d03db30ea`  
		Last Modified: Thu, 02 Mar 2023 03:19:57 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa204ac00dc80a7baf43c5cbd57e58dac7750c4461bee824e172e5b371bbc3a1`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed0500e0556e564ee3c061aab8ba437d6972a1601a4613e15745217d3e4e8`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 3.3 KB (3302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87037e492f742fa8c7655975c6bc8645dffa4b65af54b668397600a9df88bf67`  
		Last Modified: Thu, 02 Mar 2023 03:20:03 GMT  
		Size: 113.7 MB (113727920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada8b01266f7e1f58c7edbd36ac5b4be19e0964ad45faec4c0fa5d2fbd059c`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5bdabc3dd8ac152b0d4882b8790913ebe82d1df88ad9665f56a34964d85c6267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224401747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9798e89fb91eb41b6546e22b3e1a8bb4eee896d73859371b7a4556be5bc24f99`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:45:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:42 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:45 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 01:45:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:47 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:47 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 01:45:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 01:45:53 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 01:45:54 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:54 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:55 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554a400a3ae29c7fc55fd01a1e6f89137ca8d9d3b02bf899ed8219abd07e1993`  
		Last Modified: Thu, 16 Mar 2023 01:46:51 GMT  
		Size: 86.1 MB (86072279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b22cc42d586b93ed7f94332b6a66994a34f5c065fe9d2425ce49071b4658f`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11de9a3c7925a5396ee3523f43f15d472699921dd1a7a99f4259ad1060df5e62`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b9499c8ebe932301593bc3865ca3603ccd3e1385bf84b54dbb6af12137799a`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 859.6 KB (859579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37df609363a71f5ab61fa9eb2af4a07123bf3bcdaacaf717edf1d1fb186f6d9`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678d09a98290708b919069aef07aa2d3822b2f72cdc1032cfe9ec0a75a762c5`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63948bdb946efea19b4e746f7a71f6595db1a4887500954f4c34338537e4937`  
		Last Modified: Thu, 16 Mar 2023 01:46:46 GMT  
		Size: 113.7 MB (113727975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db3eecbce81b2ac2a9a5dab52e5473e81f09e6147a808a8f25321fe088866a1`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:d0d34aef89dee901c975420cfd3e18eed5a93fc22e9341faf17223e33f9f6a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231882623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e12e9971e36b9edfe3def161c83794858c7e19cdbfddf75737b4a66891febaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:02:32 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:02:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:02:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:02:42 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:02:43 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:02:44 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:02:45 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:02:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:02:47 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 03:02:48 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 03:02:49 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 03:02:50 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:02:53 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 03:03:06 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 03:03:09 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 03:03:12 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:03:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:03:14 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:03:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72676d8549372f1daaddbf5c057a44f82f8715421418692689296c3e6b6f18`  
		Last Modified: Thu, 16 Mar 2023 03:05:10 GMT  
		Size: 86.9 MB (86873898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133637599f2fe5d1949412e3f784798a9627667094b9afef054ec7aec8fbfc44`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4fae4d96045ab19d99c23311d702b17ad2744313c88c8409b7dc34c6fa2383`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4332c8a51f0dab0c9f4b7f58c974dbc19a5c7ccbdedbec5edb08171026865a9a`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 831.6 KB (831588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f9070dec5a5cb96a66f68859fb875729fef6e460ae727e62e5840b7472cb27`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbca5f6c45985a0e90f2ade072224613e89748d976c3e1bd6e6a3237b2e8fc9`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d108b0a9df94dad05287cf1abeff95905374642c3fac8ebe6491abec28cec`  
		Last Modified: Thu, 16 Mar 2023 03:04:59 GMT  
		Size: 113.7 MB (113727985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4034b6462f66f8eacbb1bf3610b0ac2ca03aa7235cc0b9d369afb2e594459`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:d90b60ec75b897585175c6ef9b3bd346247ed412baa81f8dac0248d5072b4c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:571941485e105cf84e94a41c4ba2d70adc7485eca711c139581d538cda2b3695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232950406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c818075063cf50ec77f179e29187fdc568eb8d5b781f6e0c2295c119a6a5b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:56 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 02 Mar 2023 03:18:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:58 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:58 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 02 Mar 2023 03:19:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 02 Mar 2023 03:19:08 GMT
ENV HTTP_API=false
# Thu, 02 Mar 2023 03:19:08 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:19:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:19:09 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:19:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79eb0557cffad3694c73b9238f740363322edda3463516b85107dfd5f03943b`  
		Last Modified: Thu, 02 Mar 2023 03:20:10 GMT  
		Size: 91.6 MB (91573658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65108a5e0ec07ffe53e285cf5bf0ad0ea470da18c1aab99e8e8bcec75274e1`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879bcd0356cfb8fd5e06e48295068b03787757e3cd18e28aaa23097caca64b`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782965c7157ba1f09a12b9582dc4c36bcaf6869972f8ec062d55ac5d03db30ea`  
		Last Modified: Thu, 02 Mar 2023 03:19:57 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa204ac00dc80a7baf43c5cbd57e58dac7750c4461bee824e172e5b371bbc3a1`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed0500e0556e564ee3c061aab8ba437d6972a1601a4613e15745217d3e4e8`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 3.3 KB (3302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87037e492f742fa8c7655975c6bc8645dffa4b65af54b668397600a9df88bf67`  
		Last Modified: Thu, 02 Mar 2023 03:20:03 GMT  
		Size: 113.7 MB (113727920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada8b01266f7e1f58c7edbd36ac5b4be19e0964ad45faec4c0fa5d2fbd059c`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5bdabc3dd8ac152b0d4882b8790913ebe82d1df88ad9665f56a34964d85c6267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224401747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9798e89fb91eb41b6546e22b3e1a8bb4eee896d73859371b7a4556be5bc24f99`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:45:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:42 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:45 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 01:45:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:47 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:47 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 01:45:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 01:45:53 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 01:45:54 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:54 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:55 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554a400a3ae29c7fc55fd01a1e6f89137ca8d9d3b02bf899ed8219abd07e1993`  
		Last Modified: Thu, 16 Mar 2023 01:46:51 GMT  
		Size: 86.1 MB (86072279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b22cc42d586b93ed7f94332b6a66994a34f5c065fe9d2425ce49071b4658f`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11de9a3c7925a5396ee3523f43f15d472699921dd1a7a99f4259ad1060df5e62`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b9499c8ebe932301593bc3865ca3603ccd3e1385bf84b54dbb6af12137799a`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 859.6 KB (859579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37df609363a71f5ab61fa9eb2af4a07123bf3bcdaacaf717edf1d1fb186f6d9`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678d09a98290708b919069aef07aa2d3822b2f72cdc1032cfe9ec0a75a762c5`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63948bdb946efea19b4e746f7a71f6595db1a4887500954f4c34338537e4937`  
		Last Modified: Thu, 16 Mar 2023 01:46:46 GMT  
		Size: 113.7 MB (113727975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db3eecbce81b2ac2a9a5dab52e5473e81f09e6147a808a8f25321fe088866a1`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:d0d34aef89dee901c975420cfd3e18eed5a93fc22e9341faf17223e33f9f6a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231882623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e12e9971e36b9edfe3def161c83794858c7e19cdbfddf75737b4a66891febaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:02:32 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:02:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:02:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:02:42 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:02:43 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:02:44 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:02:45 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:02:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:02:47 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 03:02:48 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 03:02:49 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 03:02:50 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:02:53 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 03:03:06 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 03:03:09 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 03:03:12 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:03:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:03:14 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:03:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72676d8549372f1daaddbf5c057a44f82f8715421418692689296c3e6b6f18`  
		Last Modified: Thu, 16 Mar 2023 03:05:10 GMT  
		Size: 86.9 MB (86873898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133637599f2fe5d1949412e3f784798a9627667094b9afef054ec7aec8fbfc44`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4fae4d96045ab19d99c23311d702b17ad2744313c88c8409b7dc34c6fa2383`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4332c8a51f0dab0c9f4b7f58c974dbc19a5c7ccbdedbec5edb08171026865a9a`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 831.6 KB (831588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f9070dec5a5cb96a66f68859fb875729fef6e460ae727e62e5840b7472cb27`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbca5f6c45985a0e90f2ade072224613e89748d976c3e1bd6e6a3237b2e8fc9`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d108b0a9df94dad05287cf1abeff95905374642c3fac8ebe6491abec28cec`  
		Last Modified: Thu, 16 Mar 2023 03:04:59 GMT  
		Size: 113.7 MB (113727985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4034b6462f66f8eacbb1bf3610b0ac2ca03aa7235cc0b9d369afb2e594459`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:2f3c5eed0c94710458be82864edbe4ba9178d8135c9df47799216985906b6002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:02b3824ad75e32956ee983c1496672784d05c33a9be1f0128785b8c39353a978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32baedb9bbed9762a558ee13a022cc8010e548f3b59d0f457c42e8b5ceacb36`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Sat, 11 Feb 2023 07:36:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:26 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_VERSION=7.14.0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BRANDING_VERSION=2022.1-u0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Sat, 11 Feb 2023 07:36:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:28 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:28 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Sat, 11 Feb 2023 07:36:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:36:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:36:39 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:36:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:36:39 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:36:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:36:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c230ac87c111c758dc330d34eec96b2fd040464085514c8bc299cc3ae6301bef`  
		Last Modified: Sat, 11 Feb 2023 07:37:49 GMT  
		Size: 57.5 MB (57457146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94688547e8089bcb2955a83b3c000f4626945038edf17b181125190ed03cb2`  
		Last Modified: Sat, 11 Feb 2023 07:37:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d3c8a6716925340bd1cba3509d4ed3ae9e214f42c3034e737f45e8976e10e`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762f5ac5ff165059fc8cb51b0ece4cc382c58bc04983a796e5df877f5800c95`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ea9043ed6c4923c0f23d917a58009babceba34bd649442325f0b361d86aa2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 3.0 KB (3030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c1ac5378dd5377fa6af775a4285f79537da5cc2e31082ddd1bf022e10c76b`  
		Last Modified: Sat, 11 Feb 2023 07:37:46 GMT  
		Size: 116.7 MB (116690797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eef05f4a0072c0d1417d0aeb36743fd44aef8f908913ab18244ff757658b7e2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4369e5cb8a74d976d78b4cdc4c8393f501cc63a2914e61e652ea4d9c8e0b1c25
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176202935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0d03b50d68ea6eba6c765b08a84d909c5a2968c58a0f53ceea419be6d4e26b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:58:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:58:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 21:58:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:58:47 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 21:58:48 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:58:48 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 21:58:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:58:56 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:58:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:58:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:58:57 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:58:57 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:58:57 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:58:57 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:58:57 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2109a84b98be453581984099b1e5905de15709f8462fd01ef9041a975f814`  
		Last Modified: Fri, 10 Feb 2023 21:59:49 GMT  
		Size: 56.8 MB (56780552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d915f6aab23e3a3243f320b98942b39e4269dda6727389cb292505d57d87070e`  
		Last Modified: Fri, 10 Feb 2023 21:59:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13344da817627abfaaa8f998dca6d0a93349f5ddcf1482d4b776cc634482722`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9c725a2f28d4e241d63208dcbef03c7263a01889033998aacae2aeacd8671`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a436099d21c84764dfe4832afa1166dd2ddf43f451d49e56e47eb787a51e3c`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55eb4882b2e4f60cc8a7a133b428594bcda8bf05708361f476857e093eb45b`  
		Last Modified: Fri, 10 Feb 2023 21:59:47 GMT  
		Size: 116.7 MB (116690810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5e9fd1bc9c10621aa7c5211a6b1be870cef856d036184db08a692c8b9aa953`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:0191aeef4a5882edad729e7ba9d3f866e05e9f7767dcbf4faa1c3abe4656a14d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172793970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cf165f9ce9e1a5741cbecbaa9df6eb357cbc2e0dfd8d0ebcb7d42d4023e924`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:52 GMT
ADD file:0db937922cfd604e84e5df7ed3bfe476af7113be3c4c1e216653f249fdacfd44 in / 
# Fri, 10 Feb 2023 21:20:53 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:09:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:09:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 22:09:31 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:09:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 22:09:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 22:09:38 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:40 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:09:40 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 22:09:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:10:00 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:10:01 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:10:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:10:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:10:04 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:10:06 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:10:07 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:10:07 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:10:08 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:10:08 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:10:09 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5b42622f88c38596f558fe14b894eadc782d1b003f25d0374cf41bc92e716959`  
		Last Modified: Fri, 10 Feb 2023 21:22:05 GMT  
		Size: 2.8 MB (2813687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b13d8f05b508a7505125aca30065be998cdcdfca17cae08199630f66f2a5e8`  
		Last Modified: Fri, 10 Feb 2023 22:12:14 GMT  
		Size: 53.3 MB (53279469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9541b2abe2c930f64fff252af8183fa8af7c1399a60f573966c284dc87cd102e`  
		Last Modified: Fri, 10 Feb 2023 22:12:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d999c19e37140fdfc6a79ddef921f4899f76153ac6f98ec4255ca7bbbe3836b6`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dff5215400cc8e206e0b8f5b659548d5dfc3248de04f06067851bc28a6ada54`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3033fffec12c9bdde2e22b8daa43f15df18b4a70c0e2ddaf82e290e98b81d`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d23e1786c784e08495019b2d059220016be2524706f6172eebcd6982a4d34`  
		Last Modified: Fri, 10 Feb 2023 22:12:10 GMT  
		Size: 116.7 MB (116690801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e978febf076cfc30ca2cb9b6e22a75956a313738f3aea8821c2a339a12a20`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:2f3c5eed0c94710458be82864edbe4ba9178d8135c9df47799216985906b6002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:02b3824ad75e32956ee983c1496672784d05c33a9be1f0128785b8c39353a978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32baedb9bbed9762a558ee13a022cc8010e548f3b59d0f457c42e8b5ceacb36`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Sat, 11 Feb 2023 07:36:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:26 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_VERSION=7.14.0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BRANDING_VERSION=2022.1-u0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Sat, 11 Feb 2023 07:36:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:28 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:28 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Sat, 11 Feb 2023 07:36:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:36:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:36:39 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:36:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:36:39 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:36:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:36:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c230ac87c111c758dc330d34eec96b2fd040464085514c8bc299cc3ae6301bef`  
		Last Modified: Sat, 11 Feb 2023 07:37:49 GMT  
		Size: 57.5 MB (57457146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94688547e8089bcb2955a83b3c000f4626945038edf17b181125190ed03cb2`  
		Last Modified: Sat, 11 Feb 2023 07:37:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d3c8a6716925340bd1cba3509d4ed3ae9e214f42c3034e737f45e8976e10e`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762f5ac5ff165059fc8cb51b0ece4cc382c58bc04983a796e5df877f5800c95`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ea9043ed6c4923c0f23d917a58009babceba34bd649442325f0b361d86aa2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 3.0 KB (3030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c1ac5378dd5377fa6af775a4285f79537da5cc2e31082ddd1bf022e10c76b`  
		Last Modified: Sat, 11 Feb 2023 07:37:46 GMT  
		Size: 116.7 MB (116690797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eef05f4a0072c0d1417d0aeb36743fd44aef8f908913ab18244ff757658b7e2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4369e5cb8a74d976d78b4cdc4c8393f501cc63a2914e61e652ea4d9c8e0b1c25
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176202935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0d03b50d68ea6eba6c765b08a84d909c5a2968c58a0f53ceea419be6d4e26b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:58:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:58:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 21:58:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:58:47 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 21:58:48 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:58:48 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 21:58:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:58:56 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:58:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:58:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:58:57 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:58:57 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:58:57 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:58:57 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:58:57 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2109a84b98be453581984099b1e5905de15709f8462fd01ef9041a975f814`  
		Last Modified: Fri, 10 Feb 2023 21:59:49 GMT  
		Size: 56.8 MB (56780552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d915f6aab23e3a3243f320b98942b39e4269dda6727389cb292505d57d87070e`  
		Last Modified: Fri, 10 Feb 2023 21:59:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13344da817627abfaaa8f998dca6d0a93349f5ddcf1482d4b776cc634482722`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9c725a2f28d4e241d63208dcbef03c7263a01889033998aacae2aeacd8671`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a436099d21c84764dfe4832afa1166dd2ddf43f451d49e56e47eb787a51e3c`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55eb4882b2e4f60cc8a7a133b428594bcda8bf05708361f476857e093eb45b`  
		Last Modified: Fri, 10 Feb 2023 21:59:47 GMT  
		Size: 116.7 MB (116690810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5e9fd1bc9c10621aa7c5211a6b1be870cef856d036184db08a692c8b9aa953`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:0191aeef4a5882edad729e7ba9d3f866e05e9f7767dcbf4faa1c3abe4656a14d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172793970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cf165f9ce9e1a5741cbecbaa9df6eb357cbc2e0dfd8d0ebcb7d42d4023e924`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:52 GMT
ADD file:0db937922cfd604e84e5df7ed3bfe476af7113be3c4c1e216653f249fdacfd44 in / 
# Fri, 10 Feb 2023 21:20:53 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:09:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:09:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 22:09:31 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:09:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 22:09:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 22:09:38 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:40 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:09:40 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 22:09:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:10:00 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:10:01 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:10:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:10:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:10:04 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:10:06 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:10:07 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:10:07 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:10:08 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:10:08 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:10:09 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5b42622f88c38596f558fe14b894eadc782d1b003f25d0374cf41bc92e716959`  
		Last Modified: Fri, 10 Feb 2023 21:22:05 GMT  
		Size: 2.8 MB (2813687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b13d8f05b508a7505125aca30065be998cdcdfca17cae08199630f66f2a5e8`  
		Last Modified: Fri, 10 Feb 2023 22:12:14 GMT  
		Size: 53.3 MB (53279469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9541b2abe2c930f64fff252af8183fa8af7c1399a60f573966c284dc87cd102e`  
		Last Modified: Fri, 10 Feb 2023 22:12:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d999c19e37140fdfc6a79ddef921f4899f76153ac6f98ec4255ca7bbbe3836b6`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dff5215400cc8e206e0b8f5b659548d5dfc3248de04f06067851bc28a6ada54`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3033fffec12c9bdde2e22b8daa43f15df18b4a70c0e2ddaf82e290e98b81d`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d23e1786c784e08495019b2d059220016be2524706f6172eebcd6982a4d34`  
		Last Modified: Fri, 10 Feb 2023 22:12:10 GMT  
		Size: 116.7 MB (116690801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e978febf076cfc30ca2cb9b6e22a75956a313738f3aea8821c2a339a12a20`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:5a83ae61e42cdf265917c0901b79134a23e53b492e378282ad6ca527abe3e761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2` - linux; amd64

```console
$ docker pull bonita@sha256:5d3ed4fd9f9d4cdbd623c66c5f2860105b17a18dc81152fd50709a6ac470caab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e19cd7ca4a306326e953fe500c4dd7bcf5e01b828fb0e84fd9cea954021a4ed`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 11 Feb 2023 07:36:50 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:50 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 11 Feb 2023 07:36:51 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:52 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 11 Feb 2023 07:37:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:37:12 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:37:13 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:37:13 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:37:13 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:37:13 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:37:13 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6663e45425c152dfb7992b8c9eeb8d6cec3a4dc529df5805b63922a919b64`  
		Last Modified: Sat, 11 Feb 2023 07:38:13 GMT  
		Size: 61.4 MB (61364554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298fdbc8a6aaea5b1d47cf5e79516539019c8e4c801d07fab88568ea817933d2`  
		Last Modified: Sat, 11 Feb 2023 07:38:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6169c4b44f713d85daee9434e474d8ddb8ef418b07f2d84ed36b0ec3d86edf`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda69351f0fed8d72a5e23d7b509a47ad85c0e095b97d21c648c7a9488aa8116`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74363046ff94dc8eac9b9006983ab60391b31d9d704a149b1c0ef0c45eeb9b`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8497c92ada3f978eb9372afb70a400410a94485630824181b17ab5d0d07ecf`  
		Last Modified: Sat, 11 Feb 2023 07:38:09 GMT  
		Size: 119.2 MB (119192991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401586f5efd8c65188ba61cda06c3a90b327feb812fedb4c5892af335e5f118`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d27829cdf839117630b67e67dda1aa36aee9e38b33ad3c9900103c27fd927561
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d743d25eeb0209db92987de7cf880598ab7cdeb1f10e8dc15a80befa4634599b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:59:02 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:59:05 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 21:59:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:59:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 21:59:07 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:08 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:59:08 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 21:59:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:59:15 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:59:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:59:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:59:16 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:59:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:59:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6859fdd3217ce6cda78174b39b4159a001e759607691e5cd8ffd91a23e38dabf`  
		Last Modified: Fri, 10 Feb 2023 22:00:15 GMT  
		Size: 60.6 MB (60620702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a069538501b951d72a4315d077fb0d6693149fe6ecc98fdcc71c8f1c8b8b966a`  
		Last Modified: Fri, 10 Feb 2023 22:00:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf012f3ecb3cab9ab2cb88227277f4b401712ec5b1761fc017360232e4521d0`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c031db4cdc6a5895f3ba624d23563b7908df002d2606f43c6e7feaff5841c`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c0d0174a76dc9d34b1e6d7426a494fe303b36af8093ab1210b4f53ac64d61c`  
		Last Modified: Fri, 10 Feb 2023 22:00:04 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a416592926bca0b0deafaa886d747cb587ddc1b74d8f739ac2854d5e57314`  
		Last Modified: Fri, 10 Feb 2023 22:00:09 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec94ca3e0917562632b04892b735ef93abe25764f6ab4d745cba047193a314`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:3afcd7c4a9cd6eb73634f6129e7f3345b2a875988b4b446e08af836f15f3ca98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9681e63339ee6e7dea654db4cf715448b01424ff9a19b9860fd5edd96254fa63`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:10:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 22:10:34 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:10:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 22:10:39 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 22:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 22:10:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:10:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:43 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:10:44 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 22:11:02 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:11:04 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:11:07 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:11:07 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:11:10 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:11:10 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:11:11 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:11:11 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:11:11 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:11:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43027ea8f93d783e28c87470bd6f8dfa8a38caa6e59be6bde3fdc3adaf9e05c9`  
		Last Modified: Fri, 10 Feb 2023 22:12:48 GMT  
		Size: 57.5 MB (57518821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812d024d679c82bd86e3b448076cd0e2c051c3e855f61230a439ccbad8aae35`  
		Last Modified: Fri, 10 Feb 2023 22:12:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9920d19a9c6f90b45d7019c0799f6ec0423d7c5742a26315093c028b625da33`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1e85317a574bc98c9fa48eeb5a0a0de10a8012304acba65db2878efea8779`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a086a276cc700bb7070fa5ee6bd37e586495293f726db3021968bf2e98ed9a`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c40145aeb952661664e02252dbfdb815944d0ca2810df50d71b13d85fbe0dc`  
		Last Modified: Fri, 10 Feb 2023 22:12:43 GMT  
		Size: 119.2 MB (119192995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36806be8d83ec34fb0fb0cab52fd742b9d497959e7f7598d172d00fec74cdc`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:5a83ae61e42cdf265917c0901b79134a23e53b492e378282ad6ca527abe3e761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:5d3ed4fd9f9d4cdbd623c66c5f2860105b17a18dc81152fd50709a6ac470caab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e19cd7ca4a306326e953fe500c4dd7bcf5e01b828fb0e84fd9cea954021a4ed`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 11 Feb 2023 07:36:50 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:50 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 11 Feb 2023 07:36:51 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:52 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 11 Feb 2023 07:37:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:37:12 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:37:13 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:37:13 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:37:13 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:37:13 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:37:13 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6663e45425c152dfb7992b8c9eeb8d6cec3a4dc529df5805b63922a919b64`  
		Last Modified: Sat, 11 Feb 2023 07:38:13 GMT  
		Size: 61.4 MB (61364554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298fdbc8a6aaea5b1d47cf5e79516539019c8e4c801d07fab88568ea817933d2`  
		Last Modified: Sat, 11 Feb 2023 07:38:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6169c4b44f713d85daee9434e474d8ddb8ef418b07f2d84ed36b0ec3d86edf`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda69351f0fed8d72a5e23d7b509a47ad85c0e095b97d21c648c7a9488aa8116`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74363046ff94dc8eac9b9006983ab60391b31d9d704a149b1c0ef0c45eeb9b`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8497c92ada3f978eb9372afb70a400410a94485630824181b17ab5d0d07ecf`  
		Last Modified: Sat, 11 Feb 2023 07:38:09 GMT  
		Size: 119.2 MB (119192991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401586f5efd8c65188ba61cda06c3a90b327feb812fedb4c5892af335e5f118`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d27829cdf839117630b67e67dda1aa36aee9e38b33ad3c9900103c27fd927561
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d743d25eeb0209db92987de7cf880598ab7cdeb1f10e8dc15a80befa4634599b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:59:02 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:59:05 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 21:59:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:59:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 21:59:07 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:08 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:59:08 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 21:59:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:59:15 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:59:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:59:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:59:16 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:59:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:59:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6859fdd3217ce6cda78174b39b4159a001e759607691e5cd8ffd91a23e38dabf`  
		Last Modified: Fri, 10 Feb 2023 22:00:15 GMT  
		Size: 60.6 MB (60620702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a069538501b951d72a4315d077fb0d6693149fe6ecc98fdcc71c8f1c8b8b966a`  
		Last Modified: Fri, 10 Feb 2023 22:00:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf012f3ecb3cab9ab2cb88227277f4b401712ec5b1761fc017360232e4521d0`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c031db4cdc6a5895f3ba624d23563b7908df002d2606f43c6e7feaff5841c`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c0d0174a76dc9d34b1e6d7426a494fe303b36af8093ab1210b4f53ac64d61c`  
		Last Modified: Fri, 10 Feb 2023 22:00:04 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a416592926bca0b0deafaa886d747cb587ddc1b74d8f739ac2854d5e57314`  
		Last Modified: Fri, 10 Feb 2023 22:00:09 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec94ca3e0917562632b04892b735ef93abe25764f6ab4d745cba047193a314`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:3afcd7c4a9cd6eb73634f6129e7f3345b2a875988b4b446e08af836f15f3ca98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9681e63339ee6e7dea654db4cf715448b01424ff9a19b9860fd5edd96254fa63`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:10:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 22:10:34 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:10:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 22:10:39 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 22:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 22:10:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:10:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:43 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:10:44 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 22:11:02 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:11:04 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:11:07 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:11:07 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:11:10 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:11:10 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:11:11 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:11:11 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:11:11 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:11:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43027ea8f93d783e28c87470bd6f8dfa8a38caa6e59be6bde3fdc3adaf9e05c9`  
		Last Modified: Fri, 10 Feb 2023 22:12:48 GMT  
		Size: 57.5 MB (57518821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812d024d679c82bd86e3b448076cd0e2c051c3e855f61230a439ccbad8aae35`  
		Last Modified: Fri, 10 Feb 2023 22:12:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9920d19a9c6f90b45d7019c0799f6ec0423d7c5742a26315093c028b625da33`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1e85317a574bc98c9fa48eeb5a0a0de10a8012304acba65db2878efea8779`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a086a276cc700bb7070fa5ee6bd37e586495293f726db3021968bf2e98ed9a`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c40145aeb952661664e02252dbfdb815944d0ca2810df50d71b13d85fbe0dc`  
		Last Modified: Fri, 10 Feb 2023 22:12:43 GMT  
		Size: 119.2 MB (119192995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36806be8d83ec34fb0fb0cab52fd742b9d497959e7f7598d172d00fec74cdc`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:74600c1b8fdd9e9da6ea7d1846ed66fe53eb58b1f8010c18e1ae298ca8b3a7c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:852b5df555a8386f4fd700ce082cc5d7e71114541aef4dd4911ba29f3ede1792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235217428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dab908e3e1e86566a9dc2e1596e0607b8530e5403b271ce80ca9349e9ead4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:06 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 02 Mar 2023 03:18:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:08 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 02 Mar 2023 03:18:08 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:08 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 02 Mar 2023 03:18:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 02 Mar 2023 03:18:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 02 Mar 2023 03:18:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 02 Mar 2023 03:18:20 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:18:20 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:18:20 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:18:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b184c9242594a7a061169b3421fc262998de1c5a8915d9c6498e2a0ccbdec`  
		Last Modified: Thu, 02 Mar 2023 03:19:45 GMT  
		Size: 91.6 MB (91573680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16a7b46a4018d71f769d60de0e03b74b1956aec2bd85f107278a759042918cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9823443109d9c74449d689c0f969bedb664341da0b074eb5b9ca191377afb5`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c56556e15411a3080cb298dc4f120b64e46c2ebbd0345c878a0184f096aba`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 506.4 KB (506351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e594029d02a66ca0ec3a57cf6caca8deff2fd287f00d768510e497c6fda0c3cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228133fa44f5f22935c7e704e20a56d74b6e000411c94e4672441bcdc967c9e3`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29c2cd8efefaa621d032e36351382b6b83a9d1d48d2df20275d713cd0449b`  
		Last Modified: Thu, 02 Mar 2023 03:19:36 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3460cc22df94fcecdfd7a2b57b08d58ff845fd633a093b7c85eca8ffa9a3594`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8902dc37b5c4d6e783edf42d065a619344e60e432ab99982d40925778877fd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226708998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c825d83cc31c6a32cec944449692b27b880cff76bf3381802d28a76a891a5c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:44:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:00 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:00 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:03 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 01:45:04 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 01:45:05 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:05 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 01:45:08 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 01:45:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 01:45:10 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 01:45:10 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:10 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:10 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae5733be1a47f93cf4115c8eb5d708ebba97340bdd829e28046dc600693677`  
		Last Modified: Thu, 16 Mar 2023 01:46:30 GMT  
		Size: 86.1 MB (86072244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f734a0f60abf1e27fac341a223580695dfe5f73b334ff706732361b8184c045`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720974a9ce140f380e608ab07d8c0ef57f711bbdec59ef43f666f2dba7a58e4c`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6af71e6e130e039dbf9930a47790d5022d3c7caeea6e0b4c56011f460705e96`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 475.8 KB (475801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05332412e688d0adb5a302bf1e48e3dbffdb93791382f9db44c640864f87b4`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162842b43ce25faf3fe11d9ebed13d4abce346ca2247d4a82035dd4d0c3bacb`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e702678d0a20a29376f82c8f237e5dac8d61c8adb6c14cb015a030f9e51af59`  
		Last Modified: Thu, 16 Mar 2023 01:46:24 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f6a37ae7d6569119ec6010cb19ce29652e71dcef93be8303070a6304cbc67e`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad6a2eed1730df305984d2d08e2b6d05d664f5486666ff3d6ce2fcd62d7f3e68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234217649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1deb6a96b55e268c39555e677ecd02eaa45a10110c6b72b724d83a023de9b6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:11 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:00:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:00:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:00:22 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:00:25 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 03:00:26 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 03:00:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 03:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:00:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 03:00:35 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:00:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 03:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 03:00:47 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 03:00:49 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 03:00:49 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:00:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:00:50 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:00:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf534da892a5857363836b577335a4b6c17a5b42a1a7ea1ff52630df1c6ec3`  
		Last Modified: Thu, 16 Mar 2023 03:04:30 GMT  
		Size: 86.9 MB (86874102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86733899243167c2217ab5a8c14cc3e45516beb302d293a31b9766445e7515b1`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bd5f53e9da1a5f4b8e9693a01f1628e5ab2d15f651c6ef925739beb14d064b`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bccc4039a31c40a2b9b85bb4cb543a3efb9416fd195edbe23404565d37c381`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c590139130e876e3d5d93370b50f0548036e3de1bee12f237950a476b5ec20`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd9505d0a45154d01bbab1b4091b6e9e462466c514b6b8d4b87f8a11b2f658d`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd74d70744e2ec85d5265ef1c01012ac2cf6baffec913859a505dbbb449b073`  
		Last Modified: Thu, 16 Mar 2023 03:04:16 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5388d68c3974a11bcf5fff3dfa9dabc966f61e6c1bcf1a66374a8a1ca7ab8377`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:74600c1b8fdd9e9da6ea7d1846ed66fe53eb58b1f8010c18e1ae298ca8b3a7c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:852b5df555a8386f4fd700ce082cc5d7e71114541aef4dd4911ba29f3ede1792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235217428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dab908e3e1e86566a9dc2e1596e0607b8530e5403b271ce80ca9349e9ead4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:06 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:06 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 02 Mar 2023 03:18:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 02 Mar 2023 03:18:08 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 02 Mar 2023 03:18:08 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:08 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 02 Mar 2023 03:18:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 02 Mar 2023 03:18:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 02 Mar 2023 03:18:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 02 Mar 2023 03:18:20 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:18:20 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:18:20 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:18:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b184c9242594a7a061169b3421fc262998de1c5a8915d9c6498e2a0ccbdec`  
		Last Modified: Thu, 02 Mar 2023 03:19:45 GMT  
		Size: 91.6 MB (91573680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16a7b46a4018d71f769d60de0e03b74b1956aec2bd85f107278a759042918cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9823443109d9c74449d689c0f969bedb664341da0b074eb5b9ca191377afb5`  
		Last Modified: Thu, 02 Mar 2023 03:19:33 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c56556e15411a3080cb298dc4f120b64e46c2ebbd0345c878a0184f096aba`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 506.4 KB (506351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e594029d02a66ca0ec3a57cf6caca8deff2fd287f00d768510e497c6fda0c3cc`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228133fa44f5f22935c7e704e20a56d74b6e000411c94e4672441bcdc967c9e3`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29c2cd8efefaa621d032e36351382b6b83a9d1d48d2df20275d713cd0449b`  
		Last Modified: Thu, 02 Mar 2023 03:19:36 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3460cc22df94fcecdfd7a2b57b08d58ff845fd633a093b7c85eca8ffa9a3594`  
		Last Modified: Thu, 02 Mar 2023 03:19:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8902dc37b5c4d6e783edf42d065a619344e60e432ab99982d40925778877fd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226708998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c825d83cc31c6a32cec944449692b27b880cff76bf3381802d28a76a891a5c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:44:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:00 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:00 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:03 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 01:45:03 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 01:45:04 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:04 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 01:45:04 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 01:45:05 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:05 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 01:45:08 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 01:45:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 01:45:10 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 01:45:10 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:10 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:10 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae5733be1a47f93cf4115c8eb5d708ebba97340bdd829e28046dc600693677`  
		Last Modified: Thu, 16 Mar 2023 01:46:30 GMT  
		Size: 86.1 MB (86072244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f734a0f60abf1e27fac341a223580695dfe5f73b334ff706732361b8184c045`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720974a9ce140f380e608ab07d8c0ef57f711bbdec59ef43f666f2dba7a58e4c`  
		Last Modified: Thu, 16 Mar 2023 01:46:22 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6af71e6e130e039dbf9930a47790d5022d3c7caeea6e0b4c56011f460705e96`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 475.8 KB (475801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05332412e688d0adb5a302bf1e48e3dbffdb93791382f9db44c640864f87b4`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162842b43ce25faf3fe11d9ebed13d4abce346ca2247d4a82035dd4d0c3bacb`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e702678d0a20a29376f82c8f237e5dac8d61c8adb6c14cb015a030f9e51af59`  
		Last Modified: Thu, 16 Mar 2023 01:46:24 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f6a37ae7d6569119ec6010cb19ce29652e71dcef93be8303070a6304cbc67e`  
		Last Modified: Thu, 16 Mar 2023 01:46:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad6a2eed1730df305984d2d08e2b6d05d664f5486666ff3d6ce2fcd62d7f3e68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234217649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1deb6a96b55e268c39555e677ecd02eaa45a10110c6b72b724d83a023de9b6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:11 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:00:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:00:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:00:20 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:00:22 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:00:23 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:00:25 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 03:00:26 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 03:00:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 03:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:00:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 03:00:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 03:00:35 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:00:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 03:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 03:00:47 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 03:00:49 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 03:00:49 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:00:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:00:50 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:00:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf534da892a5857363836b577335a4b6c17a5b42a1a7ea1ff52630df1c6ec3`  
		Last Modified: Thu, 16 Mar 2023 03:04:30 GMT  
		Size: 86.9 MB (86874102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86733899243167c2217ab5a8c14cc3e45516beb302d293a31b9766445e7515b1`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bd5f53e9da1a5f4b8e9693a01f1628e5ab2d15f651c6ef925739beb14d064b`  
		Last Modified: Thu, 16 Mar 2023 03:04:11 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bccc4039a31c40a2b9b85bb4cb543a3efb9416fd195edbe23404565d37c381`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c590139130e876e3d5d93370b50f0548036e3de1bee12f237950a476b5ec20`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd9505d0a45154d01bbab1b4091b6e9e462466c514b6b8d4b87f8a11b2f658d`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd74d70744e2ec85d5265ef1c01012ac2cf6baffec913859a505dbbb449b073`  
		Last Modified: Thu, 16 Mar 2023 03:04:16 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5388d68c3974a11bcf5fff3dfa9dabc966f61e6c1bcf1a66374a8a1ca7ab8377`  
		Last Modified: Thu, 16 Mar 2023 03:04:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:d90b60ec75b897585175c6ef9b3bd346247ed412baa81f8dac0248d5072b4c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:571941485e105cf84e94a41c4ba2d70adc7485eca711c139581d538cda2b3695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232950406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c818075063cf50ec77f179e29187fdc568eb8d5b781f6e0c2295c119a6a5b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:56 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 02 Mar 2023 03:18:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:58 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:58 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 02 Mar 2023 03:19:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 02 Mar 2023 03:19:08 GMT
ENV HTTP_API=false
# Thu, 02 Mar 2023 03:19:08 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:19:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:19:09 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:19:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79eb0557cffad3694c73b9238f740363322edda3463516b85107dfd5f03943b`  
		Last Modified: Thu, 02 Mar 2023 03:20:10 GMT  
		Size: 91.6 MB (91573658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65108a5e0ec07ffe53e285cf5bf0ad0ea470da18c1aab99e8e8bcec75274e1`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879bcd0356cfb8fd5e06e48295068b03787757e3cd18e28aaa23097caca64b`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782965c7157ba1f09a12b9582dc4c36bcaf6869972f8ec062d55ac5d03db30ea`  
		Last Modified: Thu, 02 Mar 2023 03:19:57 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa204ac00dc80a7baf43c5cbd57e58dac7750c4461bee824e172e5b371bbc3a1`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed0500e0556e564ee3c061aab8ba437d6972a1601a4613e15745217d3e4e8`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 3.3 KB (3302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87037e492f742fa8c7655975c6bc8645dffa4b65af54b668397600a9df88bf67`  
		Last Modified: Thu, 02 Mar 2023 03:20:03 GMT  
		Size: 113.7 MB (113727920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada8b01266f7e1f58c7edbd36ac5b4be19e0964ad45faec4c0fa5d2fbd059c`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5bdabc3dd8ac152b0d4882b8790913ebe82d1df88ad9665f56a34964d85c6267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224401747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9798e89fb91eb41b6546e22b3e1a8bb4eee896d73859371b7a4556be5bc24f99`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:45:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:42 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:45 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 01:45:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:47 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:47 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 01:45:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 01:45:53 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 01:45:54 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:54 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:55 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554a400a3ae29c7fc55fd01a1e6f89137ca8d9d3b02bf899ed8219abd07e1993`  
		Last Modified: Thu, 16 Mar 2023 01:46:51 GMT  
		Size: 86.1 MB (86072279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b22cc42d586b93ed7f94332b6a66994a34f5c065fe9d2425ce49071b4658f`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11de9a3c7925a5396ee3523f43f15d472699921dd1a7a99f4259ad1060df5e62`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b9499c8ebe932301593bc3865ca3603ccd3e1385bf84b54dbb6af12137799a`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 859.6 KB (859579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37df609363a71f5ab61fa9eb2af4a07123bf3bcdaacaf717edf1d1fb186f6d9`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678d09a98290708b919069aef07aa2d3822b2f72cdc1032cfe9ec0a75a762c5`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63948bdb946efea19b4e746f7a71f6595db1a4887500954f4c34338537e4937`  
		Last Modified: Thu, 16 Mar 2023 01:46:46 GMT  
		Size: 113.7 MB (113727975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db3eecbce81b2ac2a9a5dab52e5473e81f09e6147a808a8f25321fe088866a1`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:d0d34aef89dee901c975420cfd3e18eed5a93fc22e9341faf17223e33f9f6a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231882623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e12e9971e36b9edfe3def161c83794858c7e19cdbfddf75737b4a66891febaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:02:32 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:02:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:02:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:02:42 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:02:43 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:02:44 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:02:45 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:02:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:02:47 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 03:02:48 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 03:02:49 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 03:02:50 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:02:53 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 03:03:06 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 03:03:09 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 03:03:12 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:03:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:03:14 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:03:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72676d8549372f1daaddbf5c057a44f82f8715421418692689296c3e6b6f18`  
		Last Modified: Thu, 16 Mar 2023 03:05:10 GMT  
		Size: 86.9 MB (86873898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133637599f2fe5d1949412e3f784798a9627667094b9afef054ec7aec8fbfc44`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4fae4d96045ab19d99c23311d702b17ad2744313c88c8409b7dc34c6fa2383`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4332c8a51f0dab0c9f4b7f58c974dbc19a5c7ccbdedbec5edb08171026865a9a`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 831.6 KB (831588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f9070dec5a5cb96a66f68859fb875729fef6e460ae727e62e5840b7472cb27`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbca5f6c45985a0e90f2ade072224613e89748d976c3e1bd6e6a3237b2e8fc9`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d108b0a9df94dad05287cf1abeff95905374642c3fac8ebe6491abec28cec`  
		Last Modified: Thu, 16 Mar 2023 03:04:59 GMT  
		Size: 113.7 MB (113727985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4034b6462f66f8eacbb1bf3610b0ac2ca03aa7235cc0b9d369afb2e594459`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:d90b60ec75b897585175c6ef9b3bd346247ed412baa81f8dac0248d5072b4c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:571941485e105cf84e94a41c4ba2d70adc7485eca711c139581d538cda2b3695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232950406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c818075063cf50ec77f179e29187fdc568eb8d5b781f6e0c2295c119a6a5b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 02 Mar 2023 03:18:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 02 Mar 2023 03:18:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 02 Mar 2023 03:18:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 02 Mar 2023 03:18:56 GMT
ARG BONITA_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BRANDING_VERSION
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_SHA256
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BASE_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ARG BONITA_URL
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 02 Mar 2023 03:18:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 02 Mar 2023 03:18:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 02 Mar 2023 03:18:58 GMT
RUN mkdir /opt/files
# Thu, 02 Mar 2023 03:18:58 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 02 Mar 2023 03:19:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 02 Mar 2023 03:19:08 GMT
ENV HTTP_API=false
# Thu, 02 Mar 2023 03:19:08 GMT
VOLUME [/opt/bonita]
# Thu, 02 Mar 2023 03:19:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 02 Mar 2023 03:19:09 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 03:19:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79eb0557cffad3694c73b9238f740363322edda3463516b85107dfd5f03943b`  
		Last Modified: Thu, 02 Mar 2023 03:20:10 GMT  
		Size: 91.6 MB (91573658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65108a5e0ec07ffe53e285cf5bf0ad0ea470da18c1aab99e8e8bcec75274e1`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879bcd0356cfb8fd5e06e48295068b03787757e3cd18e28aaa23097caca64b`  
		Last Modified: Thu, 02 Mar 2023 03:19:58 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782965c7157ba1f09a12b9582dc4c36bcaf6869972f8ec062d55ac5d03db30ea`  
		Last Modified: Thu, 02 Mar 2023 03:19:57 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa204ac00dc80a7baf43c5cbd57e58dac7750c4461bee824e172e5b371bbc3a1`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed0500e0556e564ee3c061aab8ba437d6972a1601a4613e15745217d3e4e8`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 3.3 KB (3302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87037e492f742fa8c7655975c6bc8645dffa4b65af54b668397600a9df88bf67`  
		Last Modified: Thu, 02 Mar 2023 03:20:03 GMT  
		Size: 113.7 MB (113727920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada8b01266f7e1f58c7edbd36ac5b4be19e0964ad45faec4c0fa5d2fbd059c`  
		Last Modified: Thu, 02 Mar 2023 03:19:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5bdabc3dd8ac152b0d4882b8790913ebe82d1df88ad9665f56a34964d85c6267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224401747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9798e89fb91eb41b6546e22b3e1a8bb4eee896d73859371b7a4556be5bc24f99`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:34 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 01:45:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:45:42 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 01:45:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 01:45:45 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 01:45:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 01:45:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 01:45:47 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 01:45:47 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 01:45:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 01:45:53 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 01:45:54 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 01:45:54 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 01:45:55 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 01:45:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554a400a3ae29c7fc55fd01a1e6f89137ca8d9d3b02bf899ed8219abd07e1993`  
		Last Modified: Thu, 16 Mar 2023 01:46:51 GMT  
		Size: 86.1 MB (86072279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b22cc42d586b93ed7f94332b6a66994a34f5c065fe9d2425ce49071b4658f`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11de9a3c7925a5396ee3523f43f15d472699921dd1a7a99f4259ad1060df5e62`  
		Last Modified: Thu, 16 Mar 2023 01:46:43 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b9499c8ebe932301593bc3865ca3603ccd3e1385bf84b54dbb6af12137799a`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 859.6 KB (859579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37df609363a71f5ab61fa9eb2af4a07123bf3bcdaacaf717edf1d1fb186f6d9`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678d09a98290708b919069aef07aa2d3822b2f72cdc1032cfe9ec0a75a762c5`  
		Last Modified: Thu, 16 Mar 2023 01:46:41 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63948bdb946efea19b4e746f7a71f6595db1a4887500954f4c34338537e4937`  
		Last Modified: Thu, 16 Mar 2023 01:46:46 GMT  
		Size: 113.7 MB (113727975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db3eecbce81b2ac2a9a5dab52e5473e81f09e6147a808a8f25321fe088866a1`  
		Last Modified: Thu, 16 Mar 2023 01:46:42 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:d0d34aef89dee901c975420cfd3e18eed5a93fc22e9341faf17223e33f9f6a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231882623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e12e9971e36b9edfe3def161c83794858c7e19cdbfddf75737b4a66891febaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:57:51 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 03:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:02:32 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 03:02:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 03:02:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 03:02:42 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 03:02:43 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 03:02:44 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 03:02:45 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 03:02:46 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 03:02:47 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 03:02:48 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 03:02:49 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 03:02:50 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 03:02:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 03:02:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 03:02:53 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 03:03:06 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 03:03:09 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 03:03:12 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 03:03:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 03:03:14 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 03:03:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72676d8549372f1daaddbf5c057a44f82f8715421418692689296c3e6b6f18`  
		Last Modified: Thu, 16 Mar 2023 03:05:10 GMT  
		Size: 86.9 MB (86873898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133637599f2fe5d1949412e3f784798a9627667094b9afef054ec7aec8fbfc44`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4fae4d96045ab19d99c23311d702b17ad2744313c88c8409b7dc34c6fa2383`  
		Last Modified: Thu, 16 Mar 2023 03:04:51 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4332c8a51f0dab0c9f4b7f58c974dbc19a5c7ccbdedbec5edb08171026865a9a`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 831.6 KB (831588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f9070dec5a5cb96a66f68859fb875729fef6e460ae727e62e5840b7472cb27`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbca5f6c45985a0e90f2ade072224613e89748d976c3e1bd6e6a3237b2e8fc9`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d108b0a9df94dad05287cf1abeff95905374642c3fac8ebe6491abec28cec`  
		Last Modified: Thu, 16 Mar 2023 03:04:59 GMT  
		Size: 113.7 MB (113727985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4034b6462f66f8eacbb1bf3610b0ac2ca03aa7235cc0b9d369afb2e594459`  
		Last Modified: Thu, 16 Mar 2023 03:04:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:2f3c5eed0c94710458be82864edbe4ba9178d8135c9df47799216985906b6002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:02b3824ad75e32956ee983c1496672784d05c33a9be1f0128785b8c39353a978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32baedb9bbed9762a558ee13a022cc8010e548f3b59d0f457c42e8b5ceacb36`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Sat, 11 Feb 2023 07:36:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:26 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_VERSION=7.14.0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BRANDING_VERSION=2022.1-u0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Sat, 11 Feb 2023 07:36:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:28 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:28 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Sat, 11 Feb 2023 07:36:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:36:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:36:39 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:36:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:36:39 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:36:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:36:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c230ac87c111c758dc330d34eec96b2fd040464085514c8bc299cc3ae6301bef`  
		Last Modified: Sat, 11 Feb 2023 07:37:49 GMT  
		Size: 57.5 MB (57457146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94688547e8089bcb2955a83b3c000f4626945038edf17b181125190ed03cb2`  
		Last Modified: Sat, 11 Feb 2023 07:37:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d3c8a6716925340bd1cba3509d4ed3ae9e214f42c3034e737f45e8976e10e`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762f5ac5ff165059fc8cb51b0ece4cc382c58bc04983a796e5df877f5800c95`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ea9043ed6c4923c0f23d917a58009babceba34bd649442325f0b361d86aa2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 3.0 KB (3030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c1ac5378dd5377fa6af775a4285f79537da5cc2e31082ddd1bf022e10c76b`  
		Last Modified: Sat, 11 Feb 2023 07:37:46 GMT  
		Size: 116.7 MB (116690797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eef05f4a0072c0d1417d0aeb36743fd44aef8f908913ab18244ff757658b7e2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4369e5cb8a74d976d78b4cdc4c8393f501cc63a2914e61e652ea4d9c8e0b1c25
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176202935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0d03b50d68ea6eba6c765b08a84d909c5a2968c58a0f53ceea419be6d4e26b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:58:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:58:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 21:58:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:58:47 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 21:58:48 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:58:48 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 21:58:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:58:56 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:58:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:58:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:58:57 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:58:57 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:58:57 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:58:57 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:58:57 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2109a84b98be453581984099b1e5905de15709f8462fd01ef9041a975f814`  
		Last Modified: Fri, 10 Feb 2023 21:59:49 GMT  
		Size: 56.8 MB (56780552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d915f6aab23e3a3243f320b98942b39e4269dda6727389cb292505d57d87070e`  
		Last Modified: Fri, 10 Feb 2023 21:59:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13344da817627abfaaa8f998dca6d0a93349f5ddcf1482d4b776cc634482722`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9c725a2f28d4e241d63208dcbef03c7263a01889033998aacae2aeacd8671`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a436099d21c84764dfe4832afa1166dd2ddf43f451d49e56e47eb787a51e3c`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55eb4882b2e4f60cc8a7a133b428594bcda8bf05708361f476857e093eb45b`  
		Last Modified: Fri, 10 Feb 2023 21:59:47 GMT  
		Size: 116.7 MB (116690810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5e9fd1bc9c10621aa7c5211a6b1be870cef856d036184db08a692c8b9aa953`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:0191aeef4a5882edad729e7ba9d3f866e05e9f7767dcbf4faa1c3abe4656a14d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172793970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cf165f9ce9e1a5741cbecbaa9df6eb357cbc2e0dfd8d0ebcb7d42d4023e924`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:52 GMT
ADD file:0db937922cfd604e84e5df7ed3bfe476af7113be3c4c1e216653f249fdacfd44 in / 
# Fri, 10 Feb 2023 21:20:53 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:09:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:09:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 22:09:31 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:09:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 22:09:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 22:09:38 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:40 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:09:40 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 22:09:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:10:00 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:10:01 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:10:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:10:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:10:04 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:10:06 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:10:07 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:10:07 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:10:08 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:10:08 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:10:09 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5b42622f88c38596f558fe14b894eadc782d1b003f25d0374cf41bc92e716959`  
		Last Modified: Fri, 10 Feb 2023 21:22:05 GMT  
		Size: 2.8 MB (2813687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b13d8f05b508a7505125aca30065be998cdcdfca17cae08199630f66f2a5e8`  
		Last Modified: Fri, 10 Feb 2023 22:12:14 GMT  
		Size: 53.3 MB (53279469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9541b2abe2c930f64fff252af8183fa8af7c1399a60f573966c284dc87cd102e`  
		Last Modified: Fri, 10 Feb 2023 22:12:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d999c19e37140fdfc6a79ddef921f4899f76153ac6f98ec4255ca7bbbe3836b6`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dff5215400cc8e206e0b8f5b659548d5dfc3248de04f06067851bc28a6ada54`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3033fffec12c9bdde2e22b8daa43f15df18b4a70c0e2ddaf82e290e98b81d`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d23e1786c784e08495019b2d059220016be2524706f6172eebcd6982a4d34`  
		Last Modified: Fri, 10 Feb 2023 22:12:10 GMT  
		Size: 116.7 MB (116690801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e978febf076cfc30ca2cb9b6e22a75956a313738f3aea8821c2a339a12a20`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:2f3c5eed0c94710458be82864edbe4ba9178d8135c9df47799216985906b6002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:02b3824ad75e32956ee983c1496672784d05c33a9be1f0128785b8c39353a978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32baedb9bbed9762a558ee13a022cc8010e548f3b59d0f457c42e8b5ceacb36`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Sat, 11 Feb 2023 07:36:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:26 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_VERSION=7.14.0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BRANDING_VERSION=2022.1-u0
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Sat, 11 Feb 2023 07:36:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Sat, 11 Feb 2023 07:36:28 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:28 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Sat, 11 Feb 2023 07:36:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:36:38 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:36:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:36:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:36:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:36:39 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:36:39 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:36:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:36:39 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:36:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:36:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c230ac87c111c758dc330d34eec96b2fd040464085514c8bc299cc3ae6301bef`  
		Last Modified: Sat, 11 Feb 2023 07:37:49 GMT  
		Size: 57.5 MB (57457146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94688547e8089bcb2955a83b3c000f4626945038edf17b181125190ed03cb2`  
		Last Modified: Sat, 11 Feb 2023 07:37:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d3c8a6716925340bd1cba3509d4ed3ae9e214f42c3034e737f45e8976e10e`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762f5ac5ff165059fc8cb51b0ece4cc382c58bc04983a796e5df877f5800c95`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ea9043ed6c4923c0f23d917a58009babceba34bd649442325f0b361d86aa2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 3.0 KB (3030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c1ac5378dd5377fa6af775a4285f79537da5cc2e31082ddd1bf022e10c76b`  
		Last Modified: Sat, 11 Feb 2023 07:37:46 GMT  
		Size: 116.7 MB (116690797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eef05f4a0072c0d1417d0aeb36743fd44aef8f908913ab18244ff757658b7e2`  
		Last Modified: Sat, 11 Feb 2023 07:37:40 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4369e5cb8a74d976d78b4cdc4c8393f501cc63a2914e61e652ea4d9c8e0b1c25
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176202935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0d03b50d68ea6eba6c765b08a84d909c5a2968c58a0f53ceea419be6d4e26b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:58:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:58:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 21:58:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:58:47 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 21:58:47 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 21:58:48 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:58:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 21:58:48 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:58:48 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 21:58:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:58:56 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:58:56 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:58:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:58:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:58:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:58:57 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:58:57 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:58:57 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:58:57 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:58:57 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2109a84b98be453581984099b1e5905de15709f8462fd01ef9041a975f814`  
		Last Modified: Fri, 10 Feb 2023 21:59:49 GMT  
		Size: 56.8 MB (56780552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d915f6aab23e3a3243f320b98942b39e4269dda6727389cb292505d57d87070e`  
		Last Modified: Fri, 10 Feb 2023 21:59:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13344da817627abfaaa8f998dca6d0a93349f5ddcf1482d4b776cc634482722`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9c725a2f28d4e241d63208dcbef03c7263a01889033998aacae2aeacd8671`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a436099d21c84764dfe4832afa1166dd2ddf43f451d49e56e47eb787a51e3c`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55eb4882b2e4f60cc8a7a133b428594bcda8bf05708361f476857e093eb45b`  
		Last Modified: Fri, 10 Feb 2023 21:59:47 GMT  
		Size: 116.7 MB (116690810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5e9fd1bc9c10621aa7c5211a6b1be870cef856d036184db08a692c8b9aa953`  
		Last Modified: Fri, 10 Feb 2023 21:59:41 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:0191aeef4a5882edad729e7ba9d3f866e05e9f7767dcbf4faa1c3abe4656a14d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172793970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cf165f9ce9e1a5741cbecbaa9df6eb357cbc2e0dfd8d0ebcb7d42d4023e924`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:52 GMT
ADD file:0db937922cfd604e84e5df7ed3bfe476af7113be3c4c1e216653f249fdacfd44 in / 
# Fri, 10 Feb 2023 21:20:53 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:09:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:09:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Fri, 10 Feb 2023 22:09:31 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:09:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:09:34 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:09:35 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BONITA_VERSION=7.14.0
# Fri, 10 Feb 2023 22:09:36 GMT
ENV BRANDING_VERSION=2022.1-u0
# Fri, 10 Feb 2023 22:09:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Fri, 10 Feb 2023 22:09:38 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:09:38 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Fri, 10 Feb 2023 22:09:40 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:09:40 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Fri, 10 Feb 2023 22:09:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:10:00 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:10:01 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:10:01 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:10:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:10:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:10:03 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:10:04 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:10:05 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:10:06 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:10:07 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:10:07 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:10:08 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:10:08 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:10:09 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5b42622f88c38596f558fe14b894eadc782d1b003f25d0374cf41bc92e716959`  
		Last Modified: Fri, 10 Feb 2023 21:22:05 GMT  
		Size: 2.8 MB (2813687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b13d8f05b508a7505125aca30065be998cdcdfca17cae08199630f66f2a5e8`  
		Last Modified: Fri, 10 Feb 2023 22:12:14 GMT  
		Size: 53.3 MB (53279469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9541b2abe2c930f64fff252af8183fa8af7c1399a60f573966c284dc87cd102e`  
		Last Modified: Fri, 10 Feb 2023 22:12:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d999c19e37140fdfc6a79ddef921f4899f76153ac6f98ec4255ca7bbbe3836b6`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dff5215400cc8e206e0b8f5b659548d5dfc3248de04f06067851bc28a6ada54`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3033fffec12c9bdde2e22b8daa43f15df18b4a70c0e2ddaf82e290e98b81d`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d23e1786c784e08495019b2d059220016be2524706f6172eebcd6982a4d34`  
		Last Modified: Fri, 10 Feb 2023 22:12:10 GMT  
		Size: 116.7 MB (116690801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e978febf076cfc30ca2cb9b6e22a75956a313738f3aea8821c2a339a12a20`  
		Last Modified: Fri, 10 Feb 2023 22:12:00 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:5a83ae61e42cdf265917c0901b79134a23e53b492e378282ad6ca527abe3e761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15` - linux; amd64

```console
$ docker pull bonita@sha256:5d3ed4fd9f9d4cdbd623c66c5f2860105b17a18dc81152fd50709a6ac470caab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e19cd7ca4a306326e953fe500c4dd7bcf5e01b828fb0e84fd9cea954021a4ed`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 11 Feb 2023 07:36:50 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:50 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 11 Feb 2023 07:36:51 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:52 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 11 Feb 2023 07:37:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:37:12 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:37:13 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:37:13 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:37:13 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:37:13 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:37:13 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6663e45425c152dfb7992b8c9eeb8d6cec3a4dc529df5805b63922a919b64`  
		Last Modified: Sat, 11 Feb 2023 07:38:13 GMT  
		Size: 61.4 MB (61364554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298fdbc8a6aaea5b1d47cf5e79516539019c8e4c801d07fab88568ea817933d2`  
		Last Modified: Sat, 11 Feb 2023 07:38:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6169c4b44f713d85daee9434e474d8ddb8ef418b07f2d84ed36b0ec3d86edf`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda69351f0fed8d72a5e23d7b509a47ad85c0e095b97d21c648c7a9488aa8116`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74363046ff94dc8eac9b9006983ab60391b31d9d704a149b1c0ef0c45eeb9b`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8497c92ada3f978eb9372afb70a400410a94485630824181b17ab5d0d07ecf`  
		Last Modified: Sat, 11 Feb 2023 07:38:09 GMT  
		Size: 119.2 MB (119192991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401586f5efd8c65188ba61cda06c3a90b327feb812fedb4c5892af335e5f118`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d27829cdf839117630b67e67dda1aa36aee9e38b33ad3c9900103c27fd927561
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d743d25eeb0209db92987de7cf880598ab7cdeb1f10e8dc15a80befa4634599b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:59:02 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:59:05 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 21:59:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:59:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 21:59:07 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:08 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:59:08 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 21:59:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:59:15 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:59:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:59:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:59:16 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:59:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:59:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6859fdd3217ce6cda78174b39b4159a001e759607691e5cd8ffd91a23e38dabf`  
		Last Modified: Fri, 10 Feb 2023 22:00:15 GMT  
		Size: 60.6 MB (60620702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a069538501b951d72a4315d077fb0d6693149fe6ecc98fdcc71c8f1c8b8b966a`  
		Last Modified: Fri, 10 Feb 2023 22:00:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf012f3ecb3cab9ab2cb88227277f4b401712ec5b1761fc017360232e4521d0`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c031db4cdc6a5895f3ba624d23563b7908df002d2606f43c6e7feaff5841c`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c0d0174a76dc9d34b1e6d7426a494fe303b36af8093ab1210b4f53ac64d61c`  
		Last Modified: Fri, 10 Feb 2023 22:00:04 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a416592926bca0b0deafaa886d747cb587ddc1b74d8f739ac2854d5e57314`  
		Last Modified: Fri, 10 Feb 2023 22:00:09 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec94ca3e0917562632b04892b735ef93abe25764f6ab4d745cba047193a314`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:3afcd7c4a9cd6eb73634f6129e7f3345b2a875988b4b446e08af836f15f3ca98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9681e63339ee6e7dea654db4cf715448b01424ff9a19b9860fd5edd96254fa63`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:10:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 22:10:34 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:10:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 22:10:39 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 22:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 22:10:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:10:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:43 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:10:44 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 22:11:02 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:11:04 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:11:07 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:11:07 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:11:10 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:11:10 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:11:11 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:11:11 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:11:11 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:11:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43027ea8f93d783e28c87470bd6f8dfa8a38caa6e59be6bde3fdc3adaf9e05c9`  
		Last Modified: Fri, 10 Feb 2023 22:12:48 GMT  
		Size: 57.5 MB (57518821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812d024d679c82bd86e3b448076cd0e2c051c3e855f61230a439ccbad8aae35`  
		Last Modified: Fri, 10 Feb 2023 22:12:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9920d19a9c6f90b45d7019c0799f6ec0423d7c5742a26315093c028b625da33`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1e85317a574bc98c9fa48eeb5a0a0de10a8012304acba65db2878efea8779`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a086a276cc700bb7070fa5ee6bd37e586495293f726db3021968bf2e98ed9a`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c40145aeb952661664e02252dbfdb815944d0ca2810df50d71b13d85fbe0dc`  
		Last Modified: Fri, 10 Feb 2023 22:12:43 GMT  
		Size: 119.2 MB (119192995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36806be8d83ec34fb0fb0cab52fd742b9d497959e7f7598d172d00fec74cdc`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:5a83ae61e42cdf265917c0901b79134a23e53b492e378282ad6ca527abe3e761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15.0` - linux; amd64

```console
$ docker pull bonita@sha256:5d3ed4fd9f9d4cdbd623c66c5f2860105b17a18dc81152fd50709a6ac470caab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e19cd7ca4a306326e953fe500c4dd7bcf5e01b828fb0e84fd9cea954021a4ed`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 11 Feb 2023 07:36:50 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:50 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 11 Feb 2023 07:36:51 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:52 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 11 Feb 2023 07:37:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:37:12 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:37:13 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:37:13 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:37:13 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:37:13 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:37:13 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6663e45425c152dfb7992b8c9eeb8d6cec3a4dc529df5805b63922a919b64`  
		Last Modified: Sat, 11 Feb 2023 07:38:13 GMT  
		Size: 61.4 MB (61364554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298fdbc8a6aaea5b1d47cf5e79516539019c8e4c801d07fab88568ea817933d2`  
		Last Modified: Sat, 11 Feb 2023 07:38:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6169c4b44f713d85daee9434e474d8ddb8ef418b07f2d84ed36b0ec3d86edf`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda69351f0fed8d72a5e23d7b509a47ad85c0e095b97d21c648c7a9488aa8116`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74363046ff94dc8eac9b9006983ab60391b31d9d704a149b1c0ef0c45eeb9b`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8497c92ada3f978eb9372afb70a400410a94485630824181b17ab5d0d07ecf`  
		Last Modified: Sat, 11 Feb 2023 07:38:09 GMT  
		Size: 119.2 MB (119192991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401586f5efd8c65188ba61cda06c3a90b327feb812fedb4c5892af335e5f118`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d27829cdf839117630b67e67dda1aa36aee9e38b33ad3c9900103c27fd927561
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d743d25eeb0209db92987de7cf880598ab7cdeb1f10e8dc15a80befa4634599b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:59:02 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:59:05 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 21:59:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:59:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 21:59:07 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:08 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:59:08 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 21:59:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:59:15 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:59:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:59:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:59:16 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:59:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:59:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6859fdd3217ce6cda78174b39b4159a001e759607691e5cd8ffd91a23e38dabf`  
		Last Modified: Fri, 10 Feb 2023 22:00:15 GMT  
		Size: 60.6 MB (60620702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a069538501b951d72a4315d077fb0d6693149fe6ecc98fdcc71c8f1c8b8b966a`  
		Last Modified: Fri, 10 Feb 2023 22:00:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf012f3ecb3cab9ab2cb88227277f4b401712ec5b1761fc017360232e4521d0`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c031db4cdc6a5895f3ba624d23563b7908df002d2606f43c6e7feaff5841c`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c0d0174a76dc9d34b1e6d7426a494fe303b36af8093ab1210b4f53ac64d61c`  
		Last Modified: Fri, 10 Feb 2023 22:00:04 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a416592926bca0b0deafaa886d747cb587ddc1b74d8f739ac2854d5e57314`  
		Last Modified: Fri, 10 Feb 2023 22:00:09 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec94ca3e0917562632b04892b735ef93abe25764f6ab4d745cba047193a314`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:3afcd7c4a9cd6eb73634f6129e7f3345b2a875988b4b446e08af836f15f3ca98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9681e63339ee6e7dea654db4cf715448b01424ff9a19b9860fd5edd96254fa63`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:10:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 22:10:34 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:10:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 22:10:39 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 22:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 22:10:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:10:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:43 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:10:44 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 22:11:02 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:11:04 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:11:07 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:11:07 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:11:10 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:11:10 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:11:11 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:11:11 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:11:11 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:11:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43027ea8f93d783e28c87470bd6f8dfa8a38caa6e59be6bde3fdc3adaf9e05c9`  
		Last Modified: Fri, 10 Feb 2023 22:12:48 GMT  
		Size: 57.5 MB (57518821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812d024d679c82bd86e3b448076cd0e2c051c3e855f61230a439ccbad8aae35`  
		Last Modified: Fri, 10 Feb 2023 22:12:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9920d19a9c6f90b45d7019c0799f6ec0423d7c5742a26315093c028b625da33`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1e85317a574bc98c9fa48eeb5a0a0de10a8012304acba65db2878efea8779`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a086a276cc700bb7070fa5ee6bd37e586495293f726db3021968bf2e98ed9a`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c40145aeb952661664e02252dbfdb815944d0ca2810df50d71b13d85fbe0dc`  
		Last Modified: Fri, 10 Feb 2023 22:12:43 GMT  
		Size: 119.2 MB (119192995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36806be8d83ec34fb0fb0cab52fd742b9d497959e7f7598d172d00fec74cdc`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:5a83ae61e42cdf265917c0901b79134a23e53b492e378282ad6ca527abe3e761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:5d3ed4fd9f9d4cdbd623c66c5f2860105b17a18dc81152fd50709a6ac470caab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e19cd7ca4a306326e953fe500c4dd7bcf5e01b828fb0e84fd9cea954021a4ed`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:36:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 11 Feb 2023 07:36:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 11 Feb 2023 07:36:50 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 11 Feb 2023 07:36:50 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BONITA_VERSION
# Sat, 11 Feb 2023 07:36:50 GMT
ARG BRANDING_VERSION
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_SHA256
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BASE_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ARG BONITA_URL
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 11 Feb 2023 07:36:51 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 11 Feb 2023 07:36:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 11 Feb 2023 07:36:52 GMT
RUN mkdir /opt/files
# Sat, 11 Feb 2023 07:36:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 11 Feb 2023 07:37:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 11 Feb 2023 07:37:12 GMT
ENV HTTP_API_PASSWORD=
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 11 Feb 2023 07:37:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 11 Feb 2023 07:37:12 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 11 Feb 2023 07:37:12 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 11 Feb 2023 07:37:13 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 11 Feb 2023 07:37:13 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 11 Feb 2023 07:37:13 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 11 Feb 2023 07:37:13 GMT
EXPOSE 8080 9000
# Sat, 11 Feb 2023 07:37:13 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 11 Feb 2023 07:37:13 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6663e45425c152dfb7992b8c9eeb8d6cec3a4dc529df5805b63922a919b64`  
		Last Modified: Sat, 11 Feb 2023 07:38:13 GMT  
		Size: 61.4 MB (61364554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298fdbc8a6aaea5b1d47cf5e79516539019c8e4c801d07fab88568ea817933d2`  
		Last Modified: Sat, 11 Feb 2023 07:38:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6169c4b44f713d85daee9434e474d8ddb8ef418b07f2d84ed36b0ec3d86edf`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda69351f0fed8d72a5e23d7b509a47ad85c0e095b97d21c648c7a9488aa8116`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74363046ff94dc8eac9b9006983ab60391b31d9d704a149b1c0ef0c45eeb9b`  
		Last Modified: Sat, 11 Feb 2023 07:38:03 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8497c92ada3f978eb9372afb70a400410a94485630824181b17ab5d0d07ecf`  
		Last Modified: Sat, 11 Feb 2023 07:38:09 GMT  
		Size: 119.2 MB (119192991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401586f5efd8c65188ba61cda06c3a90b327feb812fedb4c5892af335e5f118`  
		Last Modified: Sat, 11 Feb 2023 07:38:02 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d27829cdf839117630b67e67dda1aa36aee9e38b33ad3c9900103c27fd927561
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d743d25eeb0209db92987de7cf880598ab7cdeb1f10e8dc15a80befa4634599b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:59:02 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 21:59:05 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 21:59:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 21:59:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 21:59:07 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 21:59:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 21:59:08 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 21:59:08 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 21:59:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 21:59:15 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 21:59:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 21:59:15 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 21:59:15 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 21:59:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 21:59:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 21:59:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 21:59:16 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 21:59:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 21:59:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6859fdd3217ce6cda78174b39b4159a001e759607691e5cd8ffd91a23e38dabf`  
		Last Modified: Fri, 10 Feb 2023 22:00:15 GMT  
		Size: 60.6 MB (60620702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a069538501b951d72a4315d077fb0d6693149fe6ecc98fdcc71c8f1c8b8b966a`  
		Last Modified: Fri, 10 Feb 2023 22:00:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf012f3ecb3cab9ab2cb88227277f4b401712ec5b1761fc017360232e4521d0`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c031db4cdc6a5895f3ba624d23563b7908df002d2606f43c6e7feaff5841c`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c0d0174a76dc9d34b1e6d7426a494fe303b36af8093ab1210b4f53ac64d61c`  
		Last Modified: Fri, 10 Feb 2023 22:00:04 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a416592926bca0b0deafaa886d747cb587ddc1b74d8f739ac2854d5e57314`  
		Last Modified: Fri, 10 Feb 2023 22:00:09 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec94ca3e0917562632b04892b735ef93abe25764f6ab4d745cba047193a314`  
		Last Modified: Fri, 10 Feb 2023 22:00:05 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:3afcd7c4a9cd6eb73634f6129e7f3345b2a875988b4b446e08af836f15f3ca98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9681e63339ee6e7dea654db4cf715448b01424ff9a19b9860fd5edd96254fa63`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 10 Feb 2023 22:10:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 10 Feb 2023 22:10:34 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 10 Feb 2023 22:10:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BONITA_VERSION
# Fri, 10 Feb 2023 22:10:36 GMT
ARG BRANDING_VERSION
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BONITA_SHA256
# Fri, 10 Feb 2023 22:10:37 GMT
ARG BASE_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ARG BONITA_URL
# Fri, 10 Feb 2023 22:10:38 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 10 Feb 2023 22:10:39 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 10 Feb 2023 22:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 10 Feb 2023 22:10:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 10 Feb 2023 22:10:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 10 Feb 2023 22:10:43 GMT
RUN mkdir /opt/files
# Fri, 10 Feb 2023 22:10:44 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 10 Feb 2023 22:11:02 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 10 Feb 2023 22:11:04 GMT
ENV HTTP_API=false
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 10 Feb 2023 22:11:05 GMT
ENV HTTP_API_PASSWORD=
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 10 Feb 2023 22:11:06 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 10 Feb 2023 22:11:07 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 10 Feb 2023 22:11:07 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 10 Feb 2023 22:11:08 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 10 Feb 2023 22:11:09 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 10 Feb 2023 22:11:10 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 10 Feb 2023 22:11:10 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 10 Feb 2023 22:11:11 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 10 Feb 2023 22:11:11 GMT
EXPOSE 8080 9000
# Fri, 10 Feb 2023 22:11:11 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 10 Feb 2023 22:11:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43027ea8f93d783e28c87470bd6f8dfa8a38caa6e59be6bde3fdc3adaf9e05c9`  
		Last Modified: Fri, 10 Feb 2023 22:12:48 GMT  
		Size: 57.5 MB (57518821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812d024d679c82bd86e3b448076cd0e2c051c3e855f61230a439ccbad8aae35`  
		Last Modified: Fri, 10 Feb 2023 22:12:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9920d19a9c6f90b45d7019c0799f6ec0423d7c5742a26315093c028b625da33`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1e85317a574bc98c9fa48eeb5a0a0de10a8012304acba65db2878efea8779`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a086a276cc700bb7070fa5ee6bd37e586495293f726db3021968bf2e98ed9a`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c40145aeb952661664e02252dbfdb815944d0ca2810df50d71b13d85fbe0dc`  
		Last Modified: Fri, 10 Feb 2023 22:12:43 GMT  
		Size: 119.2 MB (119192995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36806be8d83ec34fb0fb0cab52fd742b9d497959e7f7598d172d00fec74cdc`  
		Last Modified: Fri, 10 Feb 2023 22:12:32 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
