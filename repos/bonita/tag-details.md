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
$ docker pull bonita@sha256:f9e95db3ab59cc61627f2eed7e84a2ea2f04c94521e0d8746fdc23cc690467e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:6eaa1fb580767948d15189924ea67ce29dda00825092fe8210486ff3c6dfe880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235216950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4218f2dce95d1dae7a319125bed5e991d24de75c660d9b871344bf7a223ec10e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 05:59:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:59:46 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 05:59:47 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 05:59:51 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 05:59:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 05:59:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 05:59:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 05:59:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 05:59:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 05:59:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 05:59:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 05:59:59 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 05:59:59 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 05:59:59 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 05:59:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee265581e5366db514e23a384b911cda0f9c363fa43fbe61d9a078144842348`  
		Last Modified: Thu, 16 Mar 2023 06:01:23 GMT  
		Size: 91.6 MB (91573608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118f94543a26610f3fbf24c30fcaf2e9fb506eab857b4bdb7e48681ba7294184`  
		Last Modified: Thu, 16 Mar 2023 06:01:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dee1a9e7ccb576f42cefde2c9c8385a553acd46bf427503a7acd6086a52332`  
		Last Modified: Thu, 16 Mar 2023 06:01:11 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e886697dc08275694ae1077c5fb5be0686820ab8ae8c5eab42f495f2bacd2f7b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 506.3 KB (506349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a787f0370132ee1d401d61ef5b091d16384af1b74fbf8985af7dc3a5db37b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f40a083d51997ee5d62422f33eb6978e7f85a64df1b043cac754ba9eef57`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3840cb7fedf97ff3e5da0bad9ee8b7068489daccc79ae65e851b938fd76d43`  
		Last Modified: Thu, 16 Mar 2023 06:01:14 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f00af1d0cab73ff2f584bf32ed54b1d061013dfdfb1c115af3c851a0e85fe4`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:a476bdd1736cf5748c31142efbb78460ca23ceff4f3c98d42285ce323b615717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:b5a15b6f4236c07d91bc8a15ba58ba1af3a0e55175f87356c64fdbd49280a044
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232951731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6accf34fa1516c04f17e99609941c2fc8f802ffeff8e81b8ec3e2a8af2428`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 06:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:00:31 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 06:00:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 06:00:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 06:00:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:36 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 06:00:36 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 06:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 06:00:43 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 06:00:43 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 06:00:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 06:00:43 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:00:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f5b5634eceab29aa31adc5c56f9a81fe07d7cca613319b516cc31033972a18`  
		Last Modified: Thu, 16 Mar 2023 06:01:48 GMT  
		Size: 91.6 MB (91575386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f317b0dbce9fb62da73d7607d8ff6df3484afd680ba1ca4a7c5188f0d1270a`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b679751f21835ab889feb8be1cda5b1b873017599e586e28ec9042e9165e6bc`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164fa45e320629e7154eead72d8d03cb1efe9bff85b44cc83d38f5f1638f8e2`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 930.5 KB (930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d68a2b4124eceedf0f2f926ec0035126d837a94ef0d97dd9359868ef60a7ee3`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d40280cad65a1a8381ffc1bbbecb3a4d5beb3c9fa124dc6bdddf32cea5f52f`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7782337e8c596ce9228a2572ca83ee829e53b3c92d674eb75d499f0baa0c18`  
		Last Modified: Thu, 16 Mar 2023 06:01:41 GMT  
		Size: 113.7 MB (113727923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe99488669a33c8bb585187bdb97d7f26e1f61c53428404e0324af403573615`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:a476bdd1736cf5748c31142efbb78460ca23ceff4f3c98d42285ce323b615717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:b5a15b6f4236c07d91bc8a15ba58ba1af3a0e55175f87356c64fdbd49280a044
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232951731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6accf34fa1516c04f17e99609941c2fc8f802ffeff8e81b8ec3e2a8af2428`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 06:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:00:31 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 06:00:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 06:00:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 06:00:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:36 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 06:00:36 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 06:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 06:00:43 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 06:00:43 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 06:00:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 06:00:43 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:00:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f5b5634eceab29aa31adc5c56f9a81fe07d7cca613319b516cc31033972a18`  
		Last Modified: Thu, 16 Mar 2023 06:01:48 GMT  
		Size: 91.6 MB (91575386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f317b0dbce9fb62da73d7607d8ff6df3484afd680ba1ca4a7c5188f0d1270a`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b679751f21835ab889feb8be1cda5b1b873017599e586e28ec9042e9165e6bc`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164fa45e320629e7154eead72d8d03cb1efe9bff85b44cc83d38f5f1638f8e2`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 930.5 KB (930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d68a2b4124eceedf0f2f926ec0035126d837a94ef0d97dd9359868ef60a7ee3`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d40280cad65a1a8381ffc1bbbecb3a4d5beb3c9fa124dc6bdddf32cea5f52f`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7782337e8c596ce9228a2572ca83ee829e53b3c92d674eb75d499f0baa0c18`  
		Last Modified: Thu, 16 Mar 2023 06:01:41 GMT  
		Size: 113.7 MB (113727923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe99488669a33c8bb585187bdb97d7f26e1f61c53428404e0324af403573615`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:41e516fcfe334fbd9053f5f01d0948737cc196f627dc15235a62381e344f384b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:a1ccd82572d3cea69ff128a1f0cf5bb8c2c2e1a7d85c0621ecb6667dfa4de685
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b479822b92815da5889c0308d04150baccf9bc96e20b573794591c5ebf117b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:10 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 29 Mar 2023 19:39:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:15 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 29 Mar 2023 19:39:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:17 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:17 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 29 Mar 2023 19:39:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:24 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:24 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:24 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:24 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:24 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2666ba441be1767da2823e544db134b89cb95dc347f0f8c78d02d3b92df2ebb`  
		Last Modified: Wed, 29 Mar 2023 19:40:05 GMT  
		Size: 57.5 MB (57457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfff05dd96c97d623121529a73533e2bd45834192768fc656321f7f3c39247d4`  
		Last Modified: Wed, 29 Mar 2023 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db18fab688f196e53eb9e1fd16ecf4eb49bdd379d41ab5ca8460485f6152474`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c890f701ed8bc70f0ba7cf0e2eab589f43858032947fa674560bd1a0fb2ac4`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7de9dc0e78a9ae7cd0722701ba9f8a9d1c3c6706f40de47489620d099f44d`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29bed39c194420fd271c38c0b1e2535f60bf659d655424ce33375ce64b7e9b7`  
		Last Modified: Wed, 29 Mar 2023 19:40:02 GMT  
		Size: 116.7 MB (116690862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c80aa7d440bb9c99ed5df3193d56b98d1c7ea3df896b59ada232ede3b4a9dc`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
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
$ docker pull bonita@sha256:41e516fcfe334fbd9053f5f01d0948737cc196f627dc15235a62381e344f384b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:a1ccd82572d3cea69ff128a1f0cf5bb8c2c2e1a7d85c0621ecb6667dfa4de685
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b479822b92815da5889c0308d04150baccf9bc96e20b573794591c5ebf117b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:10 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 29 Mar 2023 19:39:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:15 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 29 Mar 2023 19:39:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:17 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:17 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 29 Mar 2023 19:39:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:24 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:24 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:24 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:24 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:24 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2666ba441be1767da2823e544db134b89cb95dc347f0f8c78d02d3b92df2ebb`  
		Last Modified: Wed, 29 Mar 2023 19:40:05 GMT  
		Size: 57.5 MB (57457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfff05dd96c97d623121529a73533e2bd45834192768fc656321f7f3c39247d4`  
		Last Modified: Wed, 29 Mar 2023 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db18fab688f196e53eb9e1fd16ecf4eb49bdd379d41ab5ca8460485f6152474`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c890f701ed8bc70f0ba7cf0e2eab589f43858032947fa674560bd1a0fb2ac4`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7de9dc0e78a9ae7cd0722701ba9f8a9d1c3c6706f40de47489620d099f44d`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29bed39c194420fd271c38c0b1e2535f60bf659d655424ce33375ce64b7e9b7`  
		Last Modified: Wed, 29 Mar 2023 19:40:02 GMT  
		Size: 116.7 MB (116690862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c80aa7d440bb9c99ed5df3193d56b98d1c7ea3df896b59ada232ede3b4a9dc`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
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
$ docker pull bonita@sha256:257e3d7b55fafb6e0e2d6036737e339ca701b60a9e726d6d162c3cdfa8186a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2` - linux; amd64

```console
$ docker pull bonita@sha256:8971d1dfb1e4d550ca38490924975fa577ba78de765e8e533d08bf70ce9c3228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dad69ebf2477156b895ac85935a941f6fff8f3d840bc2849875407da179d32`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 29 Mar 2023 19:39:31 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 29 Mar 2023 19:39:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 29 Mar 2023 19:39:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:40 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:41 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:41 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:41 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:41 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:41 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf8558e44ebd0c789639d1e91bce5f38e5d686fe977ff425b0ba6e2e8d07fb`  
		Last Modified: Wed, 29 Mar 2023 19:40:27 GMT  
		Size: 61.4 MB (61364567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b6692696671d44cb11b440a82d46830e4f71412837cfc078d782614e7c4a2a`  
		Last Modified: Wed, 29 Mar 2023 19:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdac19de1788430d9599b3df6f8882fe08a8fee298f592a6197081c47e5f938`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2581cb0a1cee4e2a73c01d647b8d50cbefc5090f56e3a0f6097a9103da3f94d`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2467cbd1b049581a6774c4c677129f17a9339470522e235bf9466fbc32f173`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 3.0 KB (3039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2afbc32782248fad4ae627e2be4d29459783d7f354b1ceebd10a9462052e026`  
		Last Modified: Wed, 29 Mar 2023 19:40:23 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f59069ee262d533c6aae7be69b2ae2602f1dd420356e05ca6503c6e0272116`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 5.4 KB (5418 bytes)  
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
$ docker pull bonita@sha256:257e3d7b55fafb6e0e2d6036737e339ca701b60a9e726d6d162c3cdfa8186a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:8971d1dfb1e4d550ca38490924975fa577ba78de765e8e533d08bf70ce9c3228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dad69ebf2477156b895ac85935a941f6fff8f3d840bc2849875407da179d32`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 29 Mar 2023 19:39:31 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 29 Mar 2023 19:39:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 29 Mar 2023 19:39:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:40 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:41 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:41 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:41 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:41 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:41 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf8558e44ebd0c789639d1e91bce5f38e5d686fe977ff425b0ba6e2e8d07fb`  
		Last Modified: Wed, 29 Mar 2023 19:40:27 GMT  
		Size: 61.4 MB (61364567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b6692696671d44cb11b440a82d46830e4f71412837cfc078d782614e7c4a2a`  
		Last Modified: Wed, 29 Mar 2023 19:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdac19de1788430d9599b3df6f8882fe08a8fee298f592a6197081c47e5f938`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2581cb0a1cee4e2a73c01d647b8d50cbefc5090f56e3a0f6097a9103da3f94d`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2467cbd1b049581a6774c4c677129f17a9339470522e235bf9466fbc32f173`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 3.0 KB (3039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2afbc32782248fad4ae627e2be4d29459783d7f354b1ceebd10a9462052e026`  
		Last Modified: Wed, 29 Mar 2023 19:40:23 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f59069ee262d533c6aae7be69b2ae2602f1dd420356e05ca6503c6e0272116`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 5.4 KB (5418 bytes)  
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
$ docker pull bonita@sha256:f9e95db3ab59cc61627f2eed7e84a2ea2f04c94521e0d8746fdc23cc690467e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:6eaa1fb580767948d15189924ea67ce29dda00825092fe8210486ff3c6dfe880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235216950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4218f2dce95d1dae7a319125bed5e991d24de75c660d9b871344bf7a223ec10e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 05:59:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:59:46 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 05:59:47 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 05:59:51 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 05:59:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 05:59:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 05:59:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 05:59:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 05:59:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 05:59:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 05:59:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 05:59:59 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 05:59:59 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 05:59:59 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 05:59:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee265581e5366db514e23a384b911cda0f9c363fa43fbe61d9a078144842348`  
		Last Modified: Thu, 16 Mar 2023 06:01:23 GMT  
		Size: 91.6 MB (91573608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118f94543a26610f3fbf24c30fcaf2e9fb506eab857b4bdb7e48681ba7294184`  
		Last Modified: Thu, 16 Mar 2023 06:01:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dee1a9e7ccb576f42cefde2c9c8385a553acd46bf427503a7acd6086a52332`  
		Last Modified: Thu, 16 Mar 2023 06:01:11 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e886697dc08275694ae1077c5fb5be0686820ab8ae8c5eab42f495f2bacd2f7b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 506.3 KB (506349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a787f0370132ee1d401d61ef5b091d16384af1b74fbf8985af7dc3a5db37b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f40a083d51997ee5d62422f33eb6978e7f85a64df1b043cac754ba9eef57`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3840cb7fedf97ff3e5da0bad9ee8b7068489daccc79ae65e851b938fd76d43`  
		Last Modified: Thu, 16 Mar 2023 06:01:14 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f00af1d0cab73ff2f584bf32ed54b1d061013dfdfb1c115af3c851a0e85fe4`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:f9e95db3ab59cc61627f2eed7e84a2ea2f04c94521e0d8746fdc23cc690467e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:6eaa1fb580767948d15189924ea67ce29dda00825092fe8210486ff3c6dfe880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235216950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4218f2dce95d1dae7a319125bed5e991d24de75c660d9b871344bf7a223ec10e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 05:59:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:59:46 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 05:59:47 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 05:59:51 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 16 Mar 2023 05:59:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 05:59:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 16 Mar 2023 05:59:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 16 Mar 2023 05:59:53 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 05:59:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 16 Mar 2023 05:59:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 16 Mar 2023 05:59:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 16 Mar 2023 05:59:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 16 Mar 2023 05:59:59 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 05:59:59 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 05:59:59 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 05:59:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee265581e5366db514e23a384b911cda0f9c363fa43fbe61d9a078144842348`  
		Last Modified: Thu, 16 Mar 2023 06:01:23 GMT  
		Size: 91.6 MB (91573608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118f94543a26610f3fbf24c30fcaf2e9fb506eab857b4bdb7e48681ba7294184`  
		Last Modified: Thu, 16 Mar 2023 06:01:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dee1a9e7ccb576f42cefde2c9c8385a553acd46bf427503a7acd6086a52332`  
		Last Modified: Thu, 16 Mar 2023 06:01:11 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e886697dc08275694ae1077c5fb5be0686820ab8ae8c5eab42f495f2bacd2f7b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 506.3 KB (506349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a787f0370132ee1d401d61ef5b091d16384af1b74fbf8985af7dc3a5db37b`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f40a083d51997ee5d62422f33eb6978e7f85a64df1b043cac754ba9eef57`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3840cb7fedf97ff3e5da0bad9ee8b7068489daccc79ae65e851b938fd76d43`  
		Last Modified: Thu, 16 Mar 2023 06:01:14 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f00af1d0cab73ff2f584bf32ed54b1d061013dfdfb1c115af3c851a0e85fe4`  
		Last Modified: Thu, 16 Mar 2023 06:01:10 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:a476bdd1736cf5748c31142efbb78460ca23ceff4f3c98d42285ce323b615717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:b5a15b6f4236c07d91bc8a15ba58ba1af3a0e55175f87356c64fdbd49280a044
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232951731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6accf34fa1516c04f17e99609941c2fc8f802ffeff8e81b8ec3e2a8af2428`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 06:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:00:31 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 06:00:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 06:00:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 06:00:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:36 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 06:00:36 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 06:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 06:00:43 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 06:00:43 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 06:00:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 06:00:43 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:00:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f5b5634eceab29aa31adc5c56f9a81fe07d7cca613319b516cc31033972a18`  
		Last Modified: Thu, 16 Mar 2023 06:01:48 GMT  
		Size: 91.6 MB (91575386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f317b0dbce9fb62da73d7607d8ff6df3484afd680ba1ca4a7c5188f0d1270a`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b679751f21835ab889feb8be1cda5b1b873017599e586e28ec9042e9165e6bc`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164fa45e320629e7154eead72d8d03cb1efe9bff85b44cc83d38f5f1638f8e2`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 930.5 KB (930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d68a2b4124eceedf0f2f926ec0035126d837a94ef0d97dd9359868ef60a7ee3`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d40280cad65a1a8381ffc1bbbecb3a4d5beb3c9fa124dc6bdddf32cea5f52f`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7782337e8c596ce9228a2572ca83ee829e53b3c92d674eb75d499f0baa0c18`  
		Last Modified: Thu, 16 Mar 2023 06:01:41 GMT  
		Size: 113.7 MB (113727923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe99488669a33c8bb585187bdb97d7f26e1f61c53428404e0324af403573615`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:a476bdd1736cf5748c31142efbb78460ca23ceff4f3c98d42285ce323b615717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:b5a15b6f4236c07d91bc8a15ba58ba1af3a0e55175f87356c64fdbd49280a044
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232951731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6accf34fa1516c04f17e99609941c2fc8f802ffeff8e81b8ec3e2a8af2428`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:59:01 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 16 Mar 2023 06:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:00:31 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Mar 2023 06:00:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Mar 2023 06:00:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BRANDING_VERSION
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_SHA256
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BASE_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ARG BONITA_URL
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 16 Mar 2023 06:00:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 16 Mar 2023 06:00:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 16 Mar 2023 06:00:36 GMT
RUN mkdir /opt/files
# Thu, 16 Mar 2023 06:00:36 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 16 Mar 2023 06:00:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 16 Mar 2023 06:00:43 GMT
ENV HTTP_API=false
# Thu, 16 Mar 2023 06:00:43 GMT
VOLUME [/opt/bonita]
# Thu, 16 Mar 2023 06:00:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 16 Mar 2023 06:00:43 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:00:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f5b5634eceab29aa31adc5c56f9a81fe07d7cca613319b516cc31033972a18`  
		Last Modified: Thu, 16 Mar 2023 06:01:48 GMT  
		Size: 91.6 MB (91575386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f317b0dbce9fb62da73d7607d8ff6df3484afd680ba1ca4a7c5188f0d1270a`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b679751f21835ab889feb8be1cda5b1b873017599e586e28ec9042e9165e6bc`  
		Last Modified: Thu, 16 Mar 2023 06:01:37 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164fa45e320629e7154eead72d8d03cb1efe9bff85b44cc83d38f5f1638f8e2`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 930.5 KB (930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d68a2b4124eceedf0f2f926ec0035126d837a94ef0d97dd9359868ef60a7ee3`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d40280cad65a1a8381ffc1bbbecb3a4d5beb3c9fa124dc6bdddf32cea5f52f`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7782337e8c596ce9228a2572ca83ee829e53b3c92d674eb75d499f0baa0c18`  
		Last Modified: Thu, 16 Mar 2023 06:01:41 GMT  
		Size: 113.7 MB (113727923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe99488669a33c8bb585187bdb97d7f26e1f61c53428404e0324af403573615`  
		Last Modified: Thu, 16 Mar 2023 06:01:35 GMT  
		Size: 1.7 KB (1712 bytes)  
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
$ docker pull bonita@sha256:41e516fcfe334fbd9053f5f01d0948737cc196f627dc15235a62381e344f384b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:a1ccd82572d3cea69ff128a1f0cf5bb8c2c2e1a7d85c0621ecb6667dfa4de685
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b479822b92815da5889c0308d04150baccf9bc96e20b573794591c5ebf117b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:10 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 29 Mar 2023 19:39:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:15 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 29 Mar 2023 19:39:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:17 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:17 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 29 Mar 2023 19:39:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:24 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:24 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:24 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:24 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:24 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2666ba441be1767da2823e544db134b89cb95dc347f0f8c78d02d3b92df2ebb`  
		Last Modified: Wed, 29 Mar 2023 19:40:05 GMT  
		Size: 57.5 MB (57457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfff05dd96c97d623121529a73533e2bd45834192768fc656321f7f3c39247d4`  
		Last Modified: Wed, 29 Mar 2023 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db18fab688f196e53eb9e1fd16ecf4eb49bdd379d41ab5ca8460485f6152474`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c890f701ed8bc70f0ba7cf0e2eab589f43858032947fa674560bd1a0fb2ac4`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7de9dc0e78a9ae7cd0722701ba9f8a9d1c3c6706f40de47489620d099f44d`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29bed39c194420fd271c38c0b1e2535f60bf659d655424ce33375ce64b7e9b7`  
		Last Modified: Wed, 29 Mar 2023 19:40:02 GMT  
		Size: 116.7 MB (116690862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c80aa7d440bb9c99ed5df3193d56b98d1c7ea3df896b59ada232ede3b4a9dc`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
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
$ docker pull bonita@sha256:41e516fcfe334fbd9053f5f01d0948737cc196f627dc15235a62381e344f384b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:a1ccd82572d3cea69ff128a1f0cf5bb8c2c2e1a7d85c0621ecb6667dfa4de685
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176984625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b479822b92815da5889c0308d04150baccf9bc96e20b573794591c5ebf117b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:10 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 29 Mar 2023 19:39:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:15 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:15 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 29 Mar 2023 19:39:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 29 Mar 2023 19:39:17 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:17 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 29 Mar 2023 19:39:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:23 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:23 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:23 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:24 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:24 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:24 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:24 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:24 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:24 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2666ba441be1767da2823e544db134b89cb95dc347f0f8c78d02d3b92df2ebb`  
		Last Modified: Wed, 29 Mar 2023 19:40:05 GMT  
		Size: 57.5 MB (57457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfff05dd96c97d623121529a73533e2bd45834192768fc656321f7f3c39247d4`  
		Last Modified: Wed, 29 Mar 2023 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db18fab688f196e53eb9e1fd16ecf4eb49bdd379d41ab5ca8460485f6152474`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c890f701ed8bc70f0ba7cf0e2eab589f43858032947fa674560bd1a0fb2ac4`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7de9dc0e78a9ae7cd0722701ba9f8a9d1c3c6706f40de47489620d099f44d`  
		Last Modified: Wed, 29 Mar 2023 19:39:55 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29bed39c194420fd271c38c0b1e2535f60bf659d655424ce33375ce64b7e9b7`  
		Last Modified: Wed, 29 Mar 2023 19:40:02 GMT  
		Size: 116.7 MB (116690862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c80aa7d440bb9c99ed5df3193d56b98d1c7ea3df896b59ada232ede3b4a9dc`  
		Last Modified: Wed, 29 Mar 2023 19:39:56 GMT  
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
$ docker pull bonita@sha256:257e3d7b55fafb6e0e2d6036737e339ca701b60a9e726d6d162c3cdfa8186a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15` - linux; amd64

```console
$ docker pull bonita@sha256:8971d1dfb1e4d550ca38490924975fa577ba78de765e8e533d08bf70ce9c3228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dad69ebf2477156b895ac85935a941f6fff8f3d840bc2849875407da179d32`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 29 Mar 2023 19:39:31 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 29 Mar 2023 19:39:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 29 Mar 2023 19:39:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:40 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:41 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:41 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:41 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:41 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:41 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf8558e44ebd0c789639d1e91bce5f38e5d686fe977ff425b0ba6e2e8d07fb`  
		Last Modified: Wed, 29 Mar 2023 19:40:27 GMT  
		Size: 61.4 MB (61364567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b6692696671d44cb11b440a82d46830e4f71412837cfc078d782614e7c4a2a`  
		Last Modified: Wed, 29 Mar 2023 19:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdac19de1788430d9599b3df6f8882fe08a8fee298f592a6197081c47e5f938`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2581cb0a1cee4e2a73c01d647b8d50cbefc5090f56e3a0f6097a9103da3f94d`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2467cbd1b049581a6774c4c677129f17a9339470522e235bf9466fbc32f173`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 3.0 KB (3039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2afbc32782248fad4ae627e2be4d29459783d7f354b1ceebd10a9462052e026`  
		Last Modified: Wed, 29 Mar 2023 19:40:23 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f59069ee262d533c6aae7be69b2ae2602f1dd420356e05ca6503c6e0272116`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 5.4 KB (5418 bytes)  
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
$ docker pull bonita@sha256:257e3d7b55fafb6e0e2d6036737e339ca701b60a9e726d6d162c3cdfa8186a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15.0` - linux; amd64

```console
$ docker pull bonita@sha256:8971d1dfb1e4d550ca38490924975fa577ba78de765e8e533d08bf70ce9c3228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dad69ebf2477156b895ac85935a941f6fff8f3d840bc2849875407da179d32`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 29 Mar 2023 19:39:31 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 29 Mar 2023 19:39:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 29 Mar 2023 19:39:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:40 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:41 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:41 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:41 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:41 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:41 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf8558e44ebd0c789639d1e91bce5f38e5d686fe977ff425b0ba6e2e8d07fb`  
		Last Modified: Wed, 29 Mar 2023 19:40:27 GMT  
		Size: 61.4 MB (61364567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b6692696671d44cb11b440a82d46830e4f71412837cfc078d782614e7c4a2a`  
		Last Modified: Wed, 29 Mar 2023 19:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdac19de1788430d9599b3df6f8882fe08a8fee298f592a6197081c47e5f938`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2581cb0a1cee4e2a73c01d647b8d50cbefc5090f56e3a0f6097a9103da3f94d`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2467cbd1b049581a6774c4c677129f17a9339470522e235bf9466fbc32f173`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 3.0 KB (3039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2afbc32782248fad4ae627e2be4d29459783d7f354b1ceebd10a9462052e026`  
		Last Modified: Wed, 29 Mar 2023 19:40:23 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f59069ee262d533c6aae7be69b2ae2602f1dd420356e05ca6503c6e0272116`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 5.4 KB (5418 bytes)  
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
$ docker pull bonita@sha256:257e3d7b55fafb6e0e2d6036737e339ca701b60a9e726d6d162c3cdfa8186a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:8971d1dfb1e4d550ca38490924975fa577ba78de765e8e533d08bf70ce9c3228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183375373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dad69ebf2477156b895ac85935a941f6fff8f3d840bc2849875407da179d32`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:39:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 29 Mar 2023 19:39:31 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 29 Mar 2023 19:39:31 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 29 Mar 2023 19:39:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BRANDING_VERSION
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_SHA256
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BASE_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ARG BONITA_URL
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 29 Mar 2023 19:39:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 29 Mar 2023 19:39:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 29 Mar 2023 19:39:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 29 Mar 2023 19:39:33 GMT
RUN mkdir /opt/files
# Wed, 29 Mar 2023 19:39:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 29 Mar 2023 19:39:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 29 Mar 2023 19:39:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 29 Mar 2023 19:39:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 29 Mar 2023 19:39:40 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 29 Mar 2023 19:39:40 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 29 Mar 2023 19:39:41 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 29 Mar 2023 19:39:41 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 29 Mar 2023 19:39:41 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 29 Mar 2023 19:39:41 GMT
EXPOSE 8080 9000
# Wed, 29 Mar 2023 19:39:41 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 29 Mar 2023 19:39:41 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf8558e44ebd0c789639d1e91bce5f38e5d686fe977ff425b0ba6e2e8d07fb`  
		Last Modified: Wed, 29 Mar 2023 19:40:27 GMT  
		Size: 61.4 MB (61364567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b6692696671d44cb11b440a82d46830e4f71412837cfc078d782614e7c4a2a`  
		Last Modified: Wed, 29 Mar 2023 19:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdac19de1788430d9599b3df6f8882fe08a8fee298f592a6197081c47e5f938`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2581cb0a1cee4e2a73c01d647b8d50cbefc5090f56e3a0f6097a9103da3f94d`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2467cbd1b049581a6774c4c677129f17a9339470522e235bf9466fbc32f173`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 3.0 KB (3039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2afbc32782248fad4ae627e2be4d29459783d7f354b1ceebd10a9462052e026`  
		Last Modified: Wed, 29 Mar 2023 19:40:23 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f59069ee262d533c6aae7be69b2ae2602f1dd420356e05ca6503c6e0272116`  
		Last Modified: Wed, 29 Mar 2023 19:40:17 GMT  
		Size: 5.4 KB (5418 bytes)  
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
