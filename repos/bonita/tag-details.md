<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:2022.1`](#bonita20221)
-	[`bonita:2022.1-u0`](#bonita20221-u0)
-	[`bonita:2022.2`](#bonita20222)
-	[`bonita:2022.2-u0`](#bonita20222-u0)
-	[`bonita:2023.1`](#bonita20231)
-	[`bonita:2023.1-u0`](#bonita20231-u0)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:7.14`](#bonita714)
-	[`bonita:7.14.0`](#bonita7140)
-	[`bonita:7.15`](#bonita715)
-	[`bonita:7.15.0`](#bonita7150)
-	[`bonita:8.0`](#bonita80)
-	[`bonita:8.0.0`](#bonita800)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:754feb1463a456b4a15fb00cb44606c328fe595e1fe160e58987c5713fbb9829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:d3504d49046b6cbb431ec90bb344f254f1a8e0b9736d168e22abcd30ffed7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234327184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badd28134ec7f563679eee944b08edf0f1687d1f2c778833509d8434f488a0f9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:19:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 01:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:20:05 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 01:20:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 01:20:08 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 01:20:09 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 01:20:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 01:20:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 01:20:16 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 01:20:16 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 01:20:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 01:20:17 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 01:20:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66009a2dbd6b13b48c03e620dc0d49a27b5fd5edd522481589da4ec83c526`  
		Last Modified: Fri, 02 Jun 2023 01:20:50 GMT  
		Size: 92.9 MB (92944178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be42761d56458b3876044f47c056acb8beb77ca5b5bad37a9377ae92724a7ac`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb0bf1a3506f2d3fd5fa116d38b8a133731f7ac253a756e8b48310c57fc73e`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14cd509ef9279b4e10131ecedefb2116b8fb29d8be7e1b1267eb13dfcf74d5b`  
		Last Modified: Fri, 02 Jun 2023 01:20:37 GMT  
		Size: 930.5 KB (930480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd80966488eec8a1d3be3122b746c2c605603cc3f7019eb872fd907f6dbae88`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e518b308f8e6b58f7d547b813759d11befdd2ac0bceb06ba3bce753939fb3f`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6965e6c2ffddd5132fee5c085f652709db0942fc286553c4601fcf605e7326de`  
		Last Modified: Fri, 02 Jun 2023 01:20:42 GMT  
		Size: 113.7 MB (113727967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc69d5b1c719b5e1f5a1477c02c2c69a9ebd8eb6d0b33da3a2c1b8247d10a2a5`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9983867912dae3c0340ff770602729b3b3728753ff40591cf211bcf38007a1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225676099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c63596f96f08e3dbf506c6c90b2929d5eab4dd3ef5ef84cfd25e65fde9644c9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:15:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 01 Jun 2023 23:17:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:17:02 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 01 Jun 2023 23:17:02 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 01 Jun 2023 23:17:04 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 01 Jun 2023 23:17:04 GMT
ARG BONITA_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BRANDING_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_SHA256
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BASE_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 01 Jun 2023 23:17:05 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:06 GMT
RUN mkdir /opt/files
# Thu, 01 Jun 2023 23:17:06 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 01 Jun 2023 23:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 01 Jun 2023 23:17:12 GMT
ENV HTTP_API=false
# Thu, 01 Jun 2023 23:17:13 GMT
VOLUME [/opt/bonita]
# Thu, 01 Jun 2023 23:17:13 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 01 Jun 2023 23:17:14 GMT
EXPOSE 8080
# Thu, 01 Jun 2023 23:17:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cfb67ef19b8d2442c508e04ab003d707b523f2ee8ae03c1ab1442758c12151`  
		Last Modified: Thu, 01 Jun 2023 23:17:52 GMT  
		Size: 87.3 MB (87340452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cad99b019eb859855f0d5c5825fea4757b9db91cc08ca9a3a1f4d4a421af80`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7c4b0a95b024d8689af7e62cab40303010e087a7907688d123171498db739`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a54bfcbabd0acd81e503fcd692852f94d0aefa37a592ea953045c67950963f5`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 859.6 KB (859575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed5bfbccc4f433c508ec71aeb81d2ab4aff36fed3bf9b0e355adbd42cd498d`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e1d827d0df165a6bc58709c2722e34ec7976e92aec1888870bdc42c3e5567`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23cd8e1319350f37efb6e02fa81d4e29025bf431c34d5bf98127806953fab3`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 113.7 MB (113727966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84800ffb6ef7fb85e38cf09a031bb365b6912b0aa61e2b5218f8f37e2b40850b`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:1949f2403c4d7a781614ae9b7a8a716eed78a87a8e012651d581a6d1f3ddfa06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232985950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae317f218b8b7ee80349d683feb133e81432da9e14d7b77d720c685747b9a8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:33:21 GMT
ARG RELEASE
# Tue, 30 May 2023 09:33:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:33:24 GMT
ADD file:0c5b3fc2318612ae30bebd058c1384994f4ee2f836b73d82bd9792993ad4b37c in / 
# Tue, 30 May 2023 09:33:24 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:28:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 00:29:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:29:59 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 00:30:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 00:30:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 00:30:10 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 00:30:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 00:30:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:16 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 00:30:17 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 00:30:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 00:30:31 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 00:30:33 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 00:30:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 00:30:36 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 00:30:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49256ef3d1f127247e9cadfee1ca345b4b6585dff311b5c0fc3777af0e54ee53`  
		Last Modified: Fri, 02 Jun 2023 00:31:28 GMT  
		Size: 88.0 MB (87975153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893f2f244d24ee4eab61ab5d5d344b0b596f6c6f7c438639aa2440f5f33139a`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d988ef5354d9dc58e1f01fcc0483e464f90d80b4e05fb71f327f2a9d04ddb985`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51c4bbd59329b063041df3dea6d77e971af5a4898a7d32e64abbc6935ea326f`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 831.6 KB (831582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517fe5b6144300fd21daab747302312e6d709d3e02392b92dd6077ba729c24aa`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cecde10743623c27be6b2b22d2edf85e42a018ed6f68328c390c3d2c74e1b`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43eb7eca356175acd59ed691dfd2043419d378762c6a2d7281a568060a52f5`  
		Last Modified: Fri, 02 Jun 2023 00:31:16 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3a1bc7c331800cb4e8345bf46b00a92b3b113cb71166f8d39137c0172240ac`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:754feb1463a456b4a15fb00cb44606c328fe595e1fe160e58987c5713fbb9829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:d3504d49046b6cbb431ec90bb344f254f1a8e0b9736d168e22abcd30ffed7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234327184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badd28134ec7f563679eee944b08edf0f1687d1f2c778833509d8434f488a0f9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:19:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 01:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:20:05 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 01:20:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 01:20:08 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 01:20:09 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 01:20:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 01:20:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 01:20:16 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 01:20:16 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 01:20:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 01:20:17 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 01:20:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66009a2dbd6b13b48c03e620dc0d49a27b5fd5edd522481589da4ec83c526`  
		Last Modified: Fri, 02 Jun 2023 01:20:50 GMT  
		Size: 92.9 MB (92944178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be42761d56458b3876044f47c056acb8beb77ca5b5bad37a9377ae92724a7ac`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb0bf1a3506f2d3fd5fa116d38b8a133731f7ac253a756e8b48310c57fc73e`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14cd509ef9279b4e10131ecedefb2116b8fb29d8be7e1b1267eb13dfcf74d5b`  
		Last Modified: Fri, 02 Jun 2023 01:20:37 GMT  
		Size: 930.5 KB (930480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd80966488eec8a1d3be3122b746c2c605603cc3f7019eb872fd907f6dbae88`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e518b308f8e6b58f7d547b813759d11befdd2ac0bceb06ba3bce753939fb3f`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6965e6c2ffddd5132fee5c085f652709db0942fc286553c4601fcf605e7326de`  
		Last Modified: Fri, 02 Jun 2023 01:20:42 GMT  
		Size: 113.7 MB (113727967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc69d5b1c719b5e1f5a1477c02c2c69a9ebd8eb6d0b33da3a2c1b8247d10a2a5`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9983867912dae3c0340ff770602729b3b3728753ff40591cf211bcf38007a1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225676099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c63596f96f08e3dbf506c6c90b2929d5eab4dd3ef5ef84cfd25e65fde9644c9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:15:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 01 Jun 2023 23:17:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:17:02 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 01 Jun 2023 23:17:02 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 01 Jun 2023 23:17:04 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 01 Jun 2023 23:17:04 GMT
ARG BONITA_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BRANDING_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_SHA256
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BASE_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 01 Jun 2023 23:17:05 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:06 GMT
RUN mkdir /opt/files
# Thu, 01 Jun 2023 23:17:06 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 01 Jun 2023 23:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 01 Jun 2023 23:17:12 GMT
ENV HTTP_API=false
# Thu, 01 Jun 2023 23:17:13 GMT
VOLUME [/opt/bonita]
# Thu, 01 Jun 2023 23:17:13 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 01 Jun 2023 23:17:14 GMT
EXPOSE 8080
# Thu, 01 Jun 2023 23:17:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cfb67ef19b8d2442c508e04ab003d707b523f2ee8ae03c1ab1442758c12151`  
		Last Modified: Thu, 01 Jun 2023 23:17:52 GMT  
		Size: 87.3 MB (87340452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cad99b019eb859855f0d5c5825fea4757b9db91cc08ca9a3a1f4d4a421af80`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7c4b0a95b024d8689af7e62cab40303010e087a7907688d123171498db739`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a54bfcbabd0acd81e503fcd692852f94d0aefa37a592ea953045c67950963f5`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 859.6 KB (859575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed5bfbccc4f433c508ec71aeb81d2ab4aff36fed3bf9b0e355adbd42cd498d`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e1d827d0df165a6bc58709c2722e34ec7976e92aec1888870bdc42c3e5567`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23cd8e1319350f37efb6e02fa81d4e29025bf431c34d5bf98127806953fab3`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 113.7 MB (113727966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84800ffb6ef7fb85e38cf09a031bb365b6912b0aa61e2b5218f8f37e2b40850b`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1949f2403c4d7a781614ae9b7a8a716eed78a87a8e012651d581a6d1f3ddfa06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232985950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae317f218b8b7ee80349d683feb133e81432da9e14d7b77d720c685747b9a8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:33:21 GMT
ARG RELEASE
# Tue, 30 May 2023 09:33:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:33:24 GMT
ADD file:0c5b3fc2318612ae30bebd058c1384994f4ee2f836b73d82bd9792993ad4b37c in / 
# Tue, 30 May 2023 09:33:24 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:28:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 00:29:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:29:59 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 00:30:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 00:30:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 00:30:10 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 00:30:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 00:30:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:16 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 00:30:17 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 00:30:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 00:30:31 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 00:30:33 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 00:30:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 00:30:36 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 00:30:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49256ef3d1f127247e9cadfee1ca345b4b6585dff311b5c0fc3777af0e54ee53`  
		Last Modified: Fri, 02 Jun 2023 00:31:28 GMT  
		Size: 88.0 MB (87975153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893f2f244d24ee4eab61ab5d5d344b0b596f6c6f7c438639aa2440f5f33139a`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d988ef5354d9dc58e1f01fcc0483e464f90d80b4e05fb71f327f2a9d04ddb985`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51c4bbd59329b063041df3dea6d77e971af5a4898a7d32e64abbc6935ea326f`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 831.6 KB (831582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517fe5b6144300fd21daab747302312e6d709d3e02392b92dd6077ba729c24aa`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cecde10743623c27be6b2b22d2edf85e42a018ed6f68328c390c3d2c74e1b`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43eb7eca356175acd59ed691dfd2043419d378762c6a2d7281a568060a52f5`  
		Last Modified: Fri, 02 Jun 2023 00:31:16 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3a1bc7c331800cb4e8345bf46b00a92b3b113cb71166f8d39137c0172240ac`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:2f735038a55734c095a1b0a7a0d6db998c2332986bd63f0dc70b0d682b242abc
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
$ docker pull bonita@sha256:922afdf664466e046802dd5d60a46ef82f05e9ea3e8e76eda13f100f953aee02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176203755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6caa653b79441f7668e7da11cb600ac225b93e7086b067ec7459002f7ece4ada`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:06 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:09 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 05:51:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 05:51:11 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:12 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:12 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 05:51:17 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:18 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:19 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:19 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:19 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:19 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9633968f2b76653a1731171b48837f0f059be3a086d64a84fe3bfc3f582caf`  
		Last Modified: Thu, 30 Mar 2023 05:51:56 GMT  
		Size: 56.8 MB (56780911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2e6e43136282099aa049a600819979642881459f55bec974a9a7cd37ffd1f`  
		Last Modified: Thu, 30 Mar 2023 05:51:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6390ecc3fc3944ad1ea0677151ab1ebb5355cb8d28a730979f3257b0f5a4be`  
		Last Modified: Thu, 30 Mar 2023 05:51:49 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a48c1eee700151e4eec0b8b1b35b123f7fc04ebae351e18e152ff1fde19a33`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48439eeb1bafdf9671d1d9285c58a7ab430b1bf070797b3623d16745b356b1`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5be80a7f1b3fc1eb835761193bdcc42d92859d2efc017e53d5a23a763d36260`  
		Last Modified: Thu, 30 Mar 2023 05:51:54 GMT  
		Size: 116.7 MB (116690823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00bd02a6e799bd532faa9a8adc1ce0357423338600dcc5f5de8e2a182083e23`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:8096a362306e6a1cd6891e24af7d9dfa72c2ec5d053572b64d409e01595356b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172794707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7077ea5d022f9eb983c88f5ffda8d41a7bde60bcb350d2d5565f7a2e63206f44`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:40:23 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 04:40:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:40:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:40:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 04:40:29 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:31 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:40:31 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 04:40:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:40:46 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:40:49 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:40:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:40:49 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:40:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:40:50 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe5b2e5d6c91cd07691e33b55ee8ab4a42339c253b85223086537e22cd9ee8`  
		Last Modified: Thu, 30 Mar 2023 04:42:05 GMT  
		Size: 53.3 MB (53280126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6169e8ab3d09a2862c220fc3a0b74e6813f4c08c29059f690bffc0d842791261`  
		Last Modified: Thu, 30 Mar 2023 04:41:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7747a4442b7241d927e3ca9a728886dcfd1f851091907785d0926d7582035`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8579a613124ddb0bd4f9f7444e13e53305038a68c320a701d519a16a8e9c7c3`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ddd590826d9bcb211875d04ac978b3099975f316f65f3617868df0ecc4a9e7`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 3.0 KB (3028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2877df4be38b6e4250b4f7237da7fb7a8fb346f8a6c671d8bfbc13d17d0a`  
		Last Modified: Thu, 30 Mar 2023 04:42:01 GMT  
		Size: 116.7 MB (116690808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a612dfb1bb261deeaa92d05ceefd51ef28086e0dc75a6716a3ad894345d597d`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:2f735038a55734c095a1b0a7a0d6db998c2332986bd63f0dc70b0d682b242abc
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
$ docker pull bonita@sha256:922afdf664466e046802dd5d60a46ef82f05e9ea3e8e76eda13f100f953aee02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176203755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6caa653b79441f7668e7da11cb600ac225b93e7086b067ec7459002f7ece4ada`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:06 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:09 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 05:51:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 05:51:11 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:12 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:12 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 05:51:17 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:18 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:19 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:19 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:19 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:19 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9633968f2b76653a1731171b48837f0f059be3a086d64a84fe3bfc3f582caf`  
		Last Modified: Thu, 30 Mar 2023 05:51:56 GMT  
		Size: 56.8 MB (56780911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2e6e43136282099aa049a600819979642881459f55bec974a9a7cd37ffd1f`  
		Last Modified: Thu, 30 Mar 2023 05:51:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6390ecc3fc3944ad1ea0677151ab1ebb5355cb8d28a730979f3257b0f5a4be`  
		Last Modified: Thu, 30 Mar 2023 05:51:49 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a48c1eee700151e4eec0b8b1b35b123f7fc04ebae351e18e152ff1fde19a33`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48439eeb1bafdf9671d1d9285c58a7ab430b1bf070797b3623d16745b356b1`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5be80a7f1b3fc1eb835761193bdcc42d92859d2efc017e53d5a23a763d36260`  
		Last Modified: Thu, 30 Mar 2023 05:51:54 GMT  
		Size: 116.7 MB (116690823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00bd02a6e799bd532faa9a8adc1ce0357423338600dcc5f5de8e2a182083e23`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8096a362306e6a1cd6891e24af7d9dfa72c2ec5d053572b64d409e01595356b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172794707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7077ea5d022f9eb983c88f5ffda8d41a7bde60bcb350d2d5565f7a2e63206f44`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:40:23 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 04:40:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:40:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:40:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 04:40:29 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:31 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:40:31 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 04:40:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:40:46 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:40:49 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:40:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:40:49 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:40:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:40:50 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe5b2e5d6c91cd07691e33b55ee8ab4a42339c253b85223086537e22cd9ee8`  
		Last Modified: Thu, 30 Mar 2023 04:42:05 GMT  
		Size: 53.3 MB (53280126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6169e8ab3d09a2862c220fc3a0b74e6813f4c08c29059f690bffc0d842791261`  
		Last Modified: Thu, 30 Mar 2023 04:41:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7747a4442b7241d927e3ca9a728886dcfd1f851091907785d0926d7582035`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8579a613124ddb0bd4f9f7444e13e53305038a68c320a701d519a16a8e9c7c3`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ddd590826d9bcb211875d04ac978b3099975f316f65f3617868df0ecc4a9e7`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 3.0 KB (3028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2877df4be38b6e4250b4f7237da7fb7a8fb346f8a6c671d8bfbc13d17d0a`  
		Last Modified: Thu, 30 Mar 2023 04:42:01 GMT  
		Size: 116.7 MB (116690808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a612dfb1bb261deeaa92d05ceefd51ef28086e0dc75a6716a3ad894345d597d`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:6e6bbc573fa42d39fb3347ed7635f374d02bb13072423afff1f239bc13aa2187
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
$ docker pull bonita@sha256:50be732d7cfee295ebd60456a4bd1d991f108a6f0ce8de1443c9ea8e3028b438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c2ed1e3fdb6184b528d8cf5b791ce6d36b1ac83950f88d7c2c7af62012e941`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 05:51:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:28 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:28 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 05:51:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:36 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:36 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18c88094be7ba5f11f545dc567664be26ea74e315150b4058ee7aacbee8045f`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda896840a9627845bd404732f82eefd96b641d24a46331cea9b617f9888abde`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a3f3a9484f4bd5c12a1f88d20e0841baf33777c411f2056a6be1eaca234a9`  
		Last Modified: Thu, 30 Mar 2023 05:52:14 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676425ccabf86db6a54c5e02a8fbcf0eeb15fd61d316f55e82dceaf1f55b51c0`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:50011c015d339747e2197d89c01ce5c43d70787b17c5258550ed72a32837a698
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b19e4053185eab694f5cc4560198a7844f99c72ed0466c76634201974c14988`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 04:41:14 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:15 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:41:15 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 04:41:27 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:41:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:41:33 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:41:33 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:41:33 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:41:34 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:41:34 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da411f5e57228fc6ab3c2c80db68f2b17b12757d9358a6e5aa62c4773db299`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f55f0c0813a9eccaeb6c9520bf21732bc9ca0fc4fefd6b9663623e0892add7`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad699058479ff506d709f063ad09e1b477d3e9559b2a64efa9f4ffcad9be51`  
		Last Modified: Thu, 30 Mar 2023 04:42:28 GMT  
		Size: 119.2 MB (119193021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73194802a67d20f44ac1983e818bbb1b6b5311e5a6e62993a74804dd2d06ea9d`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:6e6bbc573fa42d39fb3347ed7635f374d02bb13072423afff1f239bc13aa2187
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
$ docker pull bonita@sha256:50be732d7cfee295ebd60456a4bd1d991f108a6f0ce8de1443c9ea8e3028b438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c2ed1e3fdb6184b528d8cf5b791ce6d36b1ac83950f88d7c2c7af62012e941`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 05:51:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:28 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:28 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 05:51:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:36 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:36 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18c88094be7ba5f11f545dc567664be26ea74e315150b4058ee7aacbee8045f`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda896840a9627845bd404732f82eefd96b641d24a46331cea9b617f9888abde`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a3f3a9484f4bd5c12a1f88d20e0841baf33777c411f2056a6be1eaca234a9`  
		Last Modified: Thu, 30 Mar 2023 05:52:14 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676425ccabf86db6a54c5e02a8fbcf0eeb15fd61d316f55e82dceaf1f55b51c0`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:50011c015d339747e2197d89c01ce5c43d70787b17c5258550ed72a32837a698
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b19e4053185eab694f5cc4560198a7844f99c72ed0466c76634201974c14988`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 04:41:14 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:15 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:41:15 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 04:41:27 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:41:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:41:33 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:41:33 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:41:33 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:41:34 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:41:34 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da411f5e57228fc6ab3c2c80db68f2b17b12757d9358a6e5aa62c4773db299`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f55f0c0813a9eccaeb6c9520bf21732bc9ca0fc4fefd6b9663623e0892add7`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad699058479ff506d709f063ad09e1b477d3e9559b2a64efa9f4ffcad9be51`  
		Last Modified: Thu, 30 Mar 2023 04:42:28 GMT  
		Size: 119.2 MB (119193021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73194802a67d20f44ac1983e818bbb1b6b5311e5a6e62993a74804dd2d06ea9d`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1`

```console
$ docker pull bonita@sha256:11f53452b17e141a0c5fdc15578a1e3d0dba68d5c164253fcdcf314995be930d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2023.1` - linux; amd64

```console
$ docker pull bonita@sha256:671e25712bfc85accf4dc1ed5c634189a22cbe822aff8b96b20530fb9eaa5fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182362741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9b487300e970a4c211866c39542dce65173437ff1e5ed81e3dcb757acea0b8`
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
# Fri, 12 May 2023 23:21:11 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:21:12 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:21:12 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:21:12 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:21:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:21:20 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:21:20 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:21:20 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:21:20 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:21:20 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:21:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:21:20 GMT
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
	-	`sha256:fc024f2018f095be1f969500043d752fea087126f5e717898f989bbac61d9648`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3abbfe454b6771aa95ee693d8cfdadf037b5ada933d6166199726f63416401`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2b891bcd8514ebd87acc138b21f94fc7887a6b7be1d9447a0c48715f6c8`  
		Last Modified: Fri, 12 May 2023 23:21:43 GMT  
		Size: 118.2 MB (118180349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f83ff9c63c97121b9869fd09818516ec942220882952acc577d9fcf5be2176`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e986c19aa412b1939cd9e024f952407dde3cfc9bd55f1d2c7167698ffb3e7a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181520385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d8bc7d90e9b3e7c7c20c5728addd3ee3e63c05c4ea28e2f0bd924c5156e4ac`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:40:28 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:40:28 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:40:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:40:29 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:40:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:40:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:40:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:40:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:40:36 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:40:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:40:36 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:40:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:40:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11673db2efafcb36686ba9eaa4f032539371359afaa89493f178cfd965ca42ea`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f59596b02df4ba2281fb8cab9daf79fc8c0f35d7e68df47e9a7faf42a99a679`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c5729859f84e96b19636a3075d1898856fc585a3f3340cab01cbe5d64953e`  
		Last Modified: Fri, 12 May 2023 23:40:55 GMT  
		Size: 118.2 MB (118180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b54b8456e5db77a19f5cf047f9edfcdb00d3bc5c799b5cd66b2015fdfebef5`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:2efca8654cb0857363866bd85862926480ab68bfc613e0b94719c6d43b2b63bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178513984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d37bdafe7d4e5dc51a8949cac9203924d086fd6463e9a221e7dae89dfc2f821`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:16:24 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:16:25 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:16:25 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:16:25 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:27 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:16:27 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:16:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:16:41 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:16:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:16:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:16:45 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:16:46 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:16:46 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:16:47 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:16:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4caf1742a2ac14b306ff6452757d52d0901199c2ec158d720f19e45814f979`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f335bc5712f928f5123f04d81e8ace34f8816375451e908c97681bf28cf573fd`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 3.0 KB (3041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f1cdc1b30dc0a3c9f9d526851338a1cd2d98aa8eed74439c6e2dffd94c815`  
		Last Modified: Fri, 12 May 2023 23:17:20 GMT  
		Size: 118.2 MB (118180260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bddbcc08c63b72dc1302495dd5d2555ee89a1e701b9753aa0b912dd800c216`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1-u0`

```console
$ docker pull bonita@sha256:11f53452b17e141a0c5fdc15578a1e3d0dba68d5c164253fcdcf314995be930d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2023.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:671e25712bfc85accf4dc1ed5c634189a22cbe822aff8b96b20530fb9eaa5fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182362741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9b487300e970a4c211866c39542dce65173437ff1e5ed81e3dcb757acea0b8`
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
# Fri, 12 May 2023 23:21:11 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:21:12 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:21:12 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:21:12 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:21:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:21:20 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:21:20 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:21:20 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:21:20 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:21:20 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:21:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:21:20 GMT
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
	-	`sha256:fc024f2018f095be1f969500043d752fea087126f5e717898f989bbac61d9648`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3abbfe454b6771aa95ee693d8cfdadf037b5ada933d6166199726f63416401`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2b891bcd8514ebd87acc138b21f94fc7887a6b7be1d9447a0c48715f6c8`  
		Last Modified: Fri, 12 May 2023 23:21:43 GMT  
		Size: 118.2 MB (118180349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f83ff9c63c97121b9869fd09818516ec942220882952acc577d9fcf5be2176`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e986c19aa412b1939cd9e024f952407dde3cfc9bd55f1d2c7167698ffb3e7a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181520385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d8bc7d90e9b3e7c7c20c5728addd3ee3e63c05c4ea28e2f0bd924c5156e4ac`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:40:28 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:40:28 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:40:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:40:29 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:40:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:40:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:40:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:40:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:40:36 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:40:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:40:36 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:40:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:40:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11673db2efafcb36686ba9eaa4f032539371359afaa89493f178cfd965ca42ea`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f59596b02df4ba2281fb8cab9daf79fc8c0f35d7e68df47e9a7faf42a99a679`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c5729859f84e96b19636a3075d1898856fc585a3f3340cab01cbe5d64953e`  
		Last Modified: Fri, 12 May 2023 23:40:55 GMT  
		Size: 118.2 MB (118180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b54b8456e5db77a19f5cf047f9edfcdb00d3bc5c799b5cd66b2015fdfebef5`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:2efca8654cb0857363866bd85862926480ab68bfc613e0b94719c6d43b2b63bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178513984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d37bdafe7d4e5dc51a8949cac9203924d086fd6463e9a221e7dae89dfc2f821`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:16:24 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:16:25 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:16:25 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:16:25 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:27 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:16:27 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:16:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:16:41 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:16:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:16:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:16:45 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:16:46 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:16:46 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:16:47 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:16:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4caf1742a2ac14b306ff6452757d52d0901199c2ec158d720f19e45814f979`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f335bc5712f928f5123f04d81e8ace34f8816375451e908c97681bf28cf573fd`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 3.0 KB (3041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f1cdc1b30dc0a3c9f9d526851338a1cd2d98aa8eed74439c6e2dffd94c815`  
		Last Modified: Fri, 12 May 2023 23:17:20 GMT  
		Size: 118.2 MB (118180260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bddbcc08c63b72dc1302495dd5d2555ee89a1e701b9753aa0b912dd800c216`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:754feb1463a456b4a15fb00cb44606c328fe595e1fe160e58987c5713fbb9829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:d3504d49046b6cbb431ec90bb344f254f1a8e0b9736d168e22abcd30ffed7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234327184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badd28134ec7f563679eee944b08edf0f1687d1f2c778833509d8434f488a0f9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:19:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 01:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:20:05 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 01:20:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 01:20:08 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 01:20:09 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 01:20:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 01:20:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 01:20:16 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 01:20:16 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 01:20:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 01:20:17 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 01:20:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66009a2dbd6b13b48c03e620dc0d49a27b5fd5edd522481589da4ec83c526`  
		Last Modified: Fri, 02 Jun 2023 01:20:50 GMT  
		Size: 92.9 MB (92944178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be42761d56458b3876044f47c056acb8beb77ca5b5bad37a9377ae92724a7ac`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb0bf1a3506f2d3fd5fa116d38b8a133731f7ac253a756e8b48310c57fc73e`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14cd509ef9279b4e10131ecedefb2116b8fb29d8be7e1b1267eb13dfcf74d5b`  
		Last Modified: Fri, 02 Jun 2023 01:20:37 GMT  
		Size: 930.5 KB (930480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd80966488eec8a1d3be3122b746c2c605603cc3f7019eb872fd907f6dbae88`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e518b308f8e6b58f7d547b813759d11befdd2ac0bceb06ba3bce753939fb3f`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6965e6c2ffddd5132fee5c085f652709db0942fc286553c4601fcf605e7326de`  
		Last Modified: Fri, 02 Jun 2023 01:20:42 GMT  
		Size: 113.7 MB (113727967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc69d5b1c719b5e1f5a1477c02c2c69a9ebd8eb6d0b33da3a2c1b8247d10a2a5`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9983867912dae3c0340ff770602729b3b3728753ff40591cf211bcf38007a1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225676099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c63596f96f08e3dbf506c6c90b2929d5eab4dd3ef5ef84cfd25e65fde9644c9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:15:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 01 Jun 2023 23:17:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:17:02 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 01 Jun 2023 23:17:02 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 01 Jun 2023 23:17:04 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 01 Jun 2023 23:17:04 GMT
ARG BONITA_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BRANDING_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_SHA256
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BASE_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 01 Jun 2023 23:17:05 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:06 GMT
RUN mkdir /opt/files
# Thu, 01 Jun 2023 23:17:06 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 01 Jun 2023 23:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 01 Jun 2023 23:17:12 GMT
ENV HTTP_API=false
# Thu, 01 Jun 2023 23:17:13 GMT
VOLUME [/opt/bonita]
# Thu, 01 Jun 2023 23:17:13 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 01 Jun 2023 23:17:14 GMT
EXPOSE 8080
# Thu, 01 Jun 2023 23:17:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cfb67ef19b8d2442c508e04ab003d707b523f2ee8ae03c1ab1442758c12151`  
		Last Modified: Thu, 01 Jun 2023 23:17:52 GMT  
		Size: 87.3 MB (87340452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cad99b019eb859855f0d5c5825fea4757b9db91cc08ca9a3a1f4d4a421af80`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7c4b0a95b024d8689af7e62cab40303010e087a7907688d123171498db739`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a54bfcbabd0acd81e503fcd692852f94d0aefa37a592ea953045c67950963f5`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 859.6 KB (859575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed5bfbccc4f433c508ec71aeb81d2ab4aff36fed3bf9b0e355adbd42cd498d`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e1d827d0df165a6bc58709c2722e34ec7976e92aec1888870bdc42c3e5567`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23cd8e1319350f37efb6e02fa81d4e29025bf431c34d5bf98127806953fab3`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 113.7 MB (113727966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84800ffb6ef7fb85e38cf09a031bb365b6912b0aa61e2b5218f8f37e2b40850b`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:1949f2403c4d7a781614ae9b7a8a716eed78a87a8e012651d581a6d1f3ddfa06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232985950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae317f218b8b7ee80349d683feb133e81432da9e14d7b77d720c685747b9a8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:33:21 GMT
ARG RELEASE
# Tue, 30 May 2023 09:33:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:33:24 GMT
ADD file:0c5b3fc2318612ae30bebd058c1384994f4ee2f836b73d82bd9792993ad4b37c in / 
# Tue, 30 May 2023 09:33:24 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:28:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 00:29:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:29:59 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 00:30:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 00:30:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 00:30:10 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 00:30:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 00:30:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:16 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 00:30:17 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 00:30:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 00:30:31 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 00:30:33 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 00:30:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 00:30:36 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 00:30:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49256ef3d1f127247e9cadfee1ca345b4b6585dff311b5c0fc3777af0e54ee53`  
		Last Modified: Fri, 02 Jun 2023 00:31:28 GMT  
		Size: 88.0 MB (87975153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893f2f244d24ee4eab61ab5d5d344b0b596f6c6f7c438639aa2440f5f33139a`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d988ef5354d9dc58e1f01fcc0483e464f90d80b4e05fb71f327f2a9d04ddb985`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51c4bbd59329b063041df3dea6d77e971af5a4898a7d32e64abbc6935ea326f`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 831.6 KB (831582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517fe5b6144300fd21daab747302312e6d709d3e02392b92dd6077ba729c24aa`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cecde10743623c27be6b2b22d2edf85e42a018ed6f68328c390c3d2c74e1b`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43eb7eca356175acd59ed691dfd2043419d378762c6a2d7281a568060a52f5`  
		Last Modified: Fri, 02 Jun 2023 00:31:16 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3a1bc7c331800cb4e8345bf46b00a92b3b113cb71166f8d39137c0172240ac`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:754feb1463a456b4a15fb00cb44606c328fe595e1fe160e58987c5713fbb9829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:d3504d49046b6cbb431ec90bb344f254f1a8e0b9736d168e22abcd30ffed7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234327184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badd28134ec7f563679eee944b08edf0f1687d1f2c778833509d8434f488a0f9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:19:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 01:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:20:05 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 01:20:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 01:20:08 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 01:20:08 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 01:20:09 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 01:20:09 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 01:20:09 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 01:20:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 01:20:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 01:20:16 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 01:20:16 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 01:20:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 01:20:17 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 01:20:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66009a2dbd6b13b48c03e620dc0d49a27b5fd5edd522481589da4ec83c526`  
		Last Modified: Fri, 02 Jun 2023 01:20:50 GMT  
		Size: 92.9 MB (92944178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be42761d56458b3876044f47c056acb8beb77ca5b5bad37a9377ae92724a7ac`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb0bf1a3506f2d3fd5fa116d38b8a133731f7ac253a756e8b48310c57fc73e`  
		Last Modified: Fri, 02 Jun 2023 01:20:38 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14cd509ef9279b4e10131ecedefb2116b8fb29d8be7e1b1267eb13dfcf74d5b`  
		Last Modified: Fri, 02 Jun 2023 01:20:37 GMT  
		Size: 930.5 KB (930480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd80966488eec8a1d3be3122b746c2c605603cc3f7019eb872fd907f6dbae88`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e518b308f8e6b58f7d547b813759d11befdd2ac0bceb06ba3bce753939fb3f`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6965e6c2ffddd5132fee5c085f652709db0942fc286553c4601fcf605e7326de`  
		Last Modified: Fri, 02 Jun 2023 01:20:42 GMT  
		Size: 113.7 MB (113727967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc69d5b1c719b5e1f5a1477c02c2c69a9ebd8eb6d0b33da3a2c1b8247d10a2a5`  
		Last Modified: Fri, 02 Jun 2023 01:20:36 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9983867912dae3c0340ff770602729b3b3728753ff40591cf211bcf38007a1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225676099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c63596f96f08e3dbf506c6c90b2929d5eab4dd3ef5ef84cfd25e65fde9644c9`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:15:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 01 Jun 2023 23:17:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:17:02 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 01 Jun 2023 23:17:02 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 01 Jun 2023 23:17:04 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 01 Jun 2023 23:17:04 GMT
ARG BONITA_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BRANDING_VERSION
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_SHA256
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BASE_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ARG BONITA_URL
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 01 Jun 2023 23:17:05 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 01 Jun 2023 23:17:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 01 Jun 2023 23:17:06 GMT
RUN mkdir /opt/files
# Thu, 01 Jun 2023 23:17:06 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 01 Jun 2023 23:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 01 Jun 2023 23:17:12 GMT
ENV HTTP_API=false
# Thu, 01 Jun 2023 23:17:13 GMT
VOLUME [/opt/bonita]
# Thu, 01 Jun 2023 23:17:13 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 01 Jun 2023 23:17:14 GMT
EXPOSE 8080
# Thu, 01 Jun 2023 23:17:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cfb67ef19b8d2442c508e04ab003d707b523f2ee8ae03c1ab1442758c12151`  
		Last Modified: Thu, 01 Jun 2023 23:17:52 GMT  
		Size: 87.3 MB (87340452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cad99b019eb859855f0d5c5825fea4757b9db91cc08ca9a3a1f4d4a421af80`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7c4b0a95b024d8689af7e62cab40303010e087a7907688d123171498db739`  
		Last Modified: Thu, 01 Jun 2023 23:17:43 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a54bfcbabd0acd81e503fcd692852f94d0aefa37a592ea953045c67950963f5`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 859.6 KB (859575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed5bfbccc4f433c508ec71aeb81d2ab4aff36fed3bf9b0e355adbd42cd498d`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e1d827d0df165a6bc58709c2722e34ec7976e92aec1888870bdc42c3e5567`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23cd8e1319350f37efb6e02fa81d4e29025bf431c34d5bf98127806953fab3`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 113.7 MB (113727966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84800ffb6ef7fb85e38cf09a031bb365b6912b0aa61e2b5218f8f37e2b40850b`  
		Last Modified: Thu, 01 Jun 2023 23:17:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1949f2403c4d7a781614ae9b7a8a716eed78a87a8e012651d581a6d1f3ddfa06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232985950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae317f218b8b7ee80349d683feb133e81432da9e14d7b77d720c685747b9a8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 30 May 2023 09:33:21 GMT
ARG RELEASE
# Tue, 30 May 2023 09:33:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:33:21 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:33:24 GMT
ADD file:0c5b3fc2318612ae30bebd058c1384994f4ee2f836b73d82bd9792993ad4b37c in / 
# Tue, 30 May 2023 09:33:24 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:28:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 02 Jun 2023 00:29:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:29:59 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 02 Jun 2023 00:30:03 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 02 Jun 2023 00:30:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BONITA_VERSION
# Fri, 02 Jun 2023 00:30:08 GMT
ARG BRANDING_VERSION
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_SHA256
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BASE_URL
# Fri, 02 Jun 2023 00:30:09 GMT
ARG BONITA_URL
# Fri, 02 Jun 2023 00:30:10 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 02 Jun 2023 00:30:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 02 Jun 2023 00:30:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Jun 2023 00:30:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 02 Jun 2023 00:30:16 GMT
RUN mkdir /opt/files
# Fri, 02 Jun 2023 00:30:17 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 02 Jun 2023 00:30:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 02 Jun 2023 00:30:31 GMT
ENV HTTP_API=false
# Fri, 02 Jun 2023 00:30:33 GMT
VOLUME [/opt/bonita]
# Fri, 02 Jun 2023 00:30:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 02 Jun 2023 00:30:36 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 00:30:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49256ef3d1f127247e9cadfee1ca345b4b6585dff311b5c0fc3777af0e54ee53`  
		Last Modified: Fri, 02 Jun 2023 00:31:28 GMT  
		Size: 88.0 MB (87975153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893f2f244d24ee4eab61ab5d5d344b0b596f6c6f7c438639aa2440f5f33139a`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d988ef5354d9dc58e1f01fcc0483e464f90d80b4e05fb71f327f2a9d04ddb985`  
		Last Modified: Fri, 02 Jun 2023 00:31:09 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51c4bbd59329b063041df3dea6d77e971af5a4898a7d32e64abbc6935ea326f`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 831.6 KB (831582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517fe5b6144300fd21daab747302312e6d709d3e02392b92dd6077ba729c24aa`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cecde10743623c27be6b2b22d2edf85e42a018ed6f68328c390c3d2c74e1b`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43eb7eca356175acd59ed691dfd2043419d378762c6a2d7281a568060a52f5`  
		Last Modified: Fri, 02 Jun 2023 00:31:16 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3a1bc7c331800cb4e8345bf46b00a92b3b113cb71166f8d39137c0172240ac`  
		Last Modified: Fri, 02 Jun 2023 00:31:07 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:2f735038a55734c095a1b0a7a0d6db998c2332986bd63f0dc70b0d682b242abc
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
$ docker pull bonita@sha256:922afdf664466e046802dd5d60a46ef82f05e9ea3e8e76eda13f100f953aee02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176203755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6caa653b79441f7668e7da11cb600ac225b93e7086b067ec7459002f7ece4ada`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:06 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:09 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 05:51:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 05:51:11 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:12 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:12 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 05:51:17 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:18 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:19 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:19 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:19 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:19 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9633968f2b76653a1731171b48837f0f059be3a086d64a84fe3bfc3f582caf`  
		Last Modified: Thu, 30 Mar 2023 05:51:56 GMT  
		Size: 56.8 MB (56780911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2e6e43136282099aa049a600819979642881459f55bec974a9a7cd37ffd1f`  
		Last Modified: Thu, 30 Mar 2023 05:51:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6390ecc3fc3944ad1ea0677151ab1ebb5355cb8d28a730979f3257b0f5a4be`  
		Last Modified: Thu, 30 Mar 2023 05:51:49 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a48c1eee700151e4eec0b8b1b35b123f7fc04ebae351e18e152ff1fde19a33`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48439eeb1bafdf9671d1d9285c58a7ab430b1bf070797b3623d16745b356b1`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5be80a7f1b3fc1eb835761193bdcc42d92859d2efc017e53d5a23a763d36260`  
		Last Modified: Thu, 30 Mar 2023 05:51:54 GMT  
		Size: 116.7 MB (116690823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00bd02a6e799bd532faa9a8adc1ce0357423338600dcc5f5de8e2a182083e23`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:8096a362306e6a1cd6891e24af7d9dfa72c2ec5d053572b64d409e01595356b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172794707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7077ea5d022f9eb983c88f5ffda8d41a7bde60bcb350d2d5565f7a2e63206f44`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:40:23 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 04:40:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:40:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:40:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 04:40:29 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:31 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:40:31 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 04:40:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:40:46 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:40:49 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:40:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:40:49 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:40:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:40:50 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe5b2e5d6c91cd07691e33b55ee8ab4a42339c253b85223086537e22cd9ee8`  
		Last Modified: Thu, 30 Mar 2023 04:42:05 GMT  
		Size: 53.3 MB (53280126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6169e8ab3d09a2862c220fc3a0b74e6813f4c08c29059f690bffc0d842791261`  
		Last Modified: Thu, 30 Mar 2023 04:41:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7747a4442b7241d927e3ca9a728886dcfd1f851091907785d0926d7582035`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8579a613124ddb0bd4f9f7444e13e53305038a68c320a701d519a16a8e9c7c3`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ddd590826d9bcb211875d04ac978b3099975f316f65f3617868df0ecc4a9e7`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 3.0 KB (3028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2877df4be38b6e4250b4f7237da7fb7a8fb346f8a6c671d8bfbc13d17d0a`  
		Last Modified: Thu, 30 Mar 2023 04:42:01 GMT  
		Size: 116.7 MB (116690808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a612dfb1bb261deeaa92d05ceefd51ef28086e0dc75a6716a3ad894345d597d`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:2f735038a55734c095a1b0a7a0d6db998c2332986bd63f0dc70b0d682b242abc
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
$ docker pull bonita@sha256:922afdf664466e046802dd5d60a46ef82f05e9ea3e8e76eda13f100f953aee02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176203755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6caa653b79441f7668e7da11cb600ac225b93e7086b067ec7459002f7ece4ada`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:06 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:09 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 05:51:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 05:51:11 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 05:51:12 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:12 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 05:51:17 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:18 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:18 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:18 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:19 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:19 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:19 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:19 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:19 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9633968f2b76653a1731171b48837f0f059be3a086d64a84fe3bfc3f582caf`  
		Last Modified: Thu, 30 Mar 2023 05:51:56 GMT  
		Size: 56.8 MB (56780911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2e6e43136282099aa049a600819979642881459f55bec974a9a7cd37ffd1f`  
		Last Modified: Thu, 30 Mar 2023 05:51:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6390ecc3fc3944ad1ea0677151ab1ebb5355cb8d28a730979f3257b0f5a4be`  
		Last Modified: Thu, 30 Mar 2023 05:51:49 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a48c1eee700151e4eec0b8b1b35b123f7fc04ebae351e18e152ff1fde19a33`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48439eeb1bafdf9671d1d9285c58a7ab430b1bf070797b3623d16745b356b1`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5be80a7f1b3fc1eb835761193bdcc42d92859d2efc017e53d5a23a763d36260`  
		Last Modified: Thu, 30 Mar 2023 05:51:54 GMT  
		Size: 116.7 MB (116690823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00bd02a6e799bd532faa9a8adc1ce0357423338600dcc5f5de8e2a182083e23`  
		Last Modified: Thu, 30 Mar 2023 05:51:48 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8096a362306e6a1cd6891e24af7d9dfa72c2ec5d053572b64d409e01595356b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172794707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7077ea5d022f9eb983c88f5ffda8d41a7bde60bcb350d2d5565f7a2e63206f44`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:40:23 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 30 Mar 2023 04:40:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:40:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:40:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:40:28 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 30 Mar 2023 04:40:29 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 30 Mar 2023 04:40:29 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 30 Mar 2023 04:40:31 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:40:31 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 30 Mar 2023 04:40:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:40:45 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:40:46 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:40:46 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:40:47 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:40:48 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:40:49 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:40:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:40:49 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:40:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:40:50 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe5b2e5d6c91cd07691e33b55ee8ab4a42339c253b85223086537e22cd9ee8`  
		Last Modified: Thu, 30 Mar 2023 04:42:05 GMT  
		Size: 53.3 MB (53280126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6169e8ab3d09a2862c220fc3a0b74e6813f4c08c29059f690bffc0d842791261`  
		Last Modified: Thu, 30 Mar 2023 04:41:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7747a4442b7241d927e3ca9a728886dcfd1f851091907785d0926d7582035`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8579a613124ddb0bd4f9f7444e13e53305038a68c320a701d519a16a8e9c7c3`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ddd590826d9bcb211875d04ac978b3099975f316f65f3617868df0ecc4a9e7`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 3.0 KB (3028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2877df4be38b6e4250b4f7237da7fb7a8fb346f8a6c671d8bfbc13d17d0a`  
		Last Modified: Thu, 30 Mar 2023 04:42:01 GMT  
		Size: 116.7 MB (116690808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a612dfb1bb261deeaa92d05ceefd51ef28086e0dc75a6716a3ad894345d597d`  
		Last Modified: Thu, 30 Mar 2023 04:41:51 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:6e6bbc573fa42d39fb3347ed7635f374d02bb13072423afff1f239bc13aa2187
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
$ docker pull bonita@sha256:50be732d7cfee295ebd60456a4bd1d991f108a6f0ce8de1443c9ea8e3028b438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c2ed1e3fdb6184b528d8cf5b791ce6d36b1ac83950f88d7c2c7af62012e941`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 05:51:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:28 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:28 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 05:51:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:36 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:36 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18c88094be7ba5f11f545dc567664be26ea74e315150b4058ee7aacbee8045f`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda896840a9627845bd404732f82eefd96b641d24a46331cea9b617f9888abde`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a3f3a9484f4bd5c12a1f88d20e0841baf33777c411f2056a6be1eaca234a9`  
		Last Modified: Thu, 30 Mar 2023 05:52:14 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676425ccabf86db6a54c5e02a8fbcf0eeb15fd61d316f55e82dceaf1f55b51c0`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:50011c015d339747e2197d89c01ce5c43d70787b17c5258550ed72a32837a698
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b19e4053185eab694f5cc4560198a7844f99c72ed0466c76634201974c14988`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 04:41:14 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:15 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:41:15 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 04:41:27 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:41:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:41:33 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:41:33 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:41:33 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:41:34 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:41:34 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da411f5e57228fc6ab3c2c80db68f2b17b12757d9358a6e5aa62c4773db299`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f55f0c0813a9eccaeb6c9520bf21732bc9ca0fc4fefd6b9663623e0892add7`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad699058479ff506d709f063ad09e1b477d3e9559b2a64efa9f4ffcad9be51`  
		Last Modified: Thu, 30 Mar 2023 04:42:28 GMT  
		Size: 119.2 MB (119193021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73194802a67d20f44ac1983e818bbb1b6b5311e5a6e62993a74804dd2d06ea9d`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:6e6bbc573fa42d39fb3347ed7635f374d02bb13072423afff1f239bc13aa2187
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
$ docker pull bonita@sha256:50be732d7cfee295ebd60456a4bd1d991f108a6f0ce8de1443c9ea8e3028b438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182533069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c2ed1e3fdb6184b528d8cf5b791ce6d36b1ac83950f88d7c2c7af62012e941`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 05:51:27 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 05:51:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 05:51:28 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 05:51:28 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 05:51:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 05:51:35 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 05:51:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 05:51:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 05:51:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 05:51:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 05:51:36 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 05:51:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 05:51:36 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 05:51:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 05:51:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18c88094be7ba5f11f545dc567664be26ea74e315150b4058ee7aacbee8045f`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda896840a9627845bd404732f82eefd96b641d24a46331cea9b617f9888abde`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a3f3a9484f4bd5c12a1f88d20e0841baf33777c411f2056a6be1eaca234a9`  
		Last Modified: Thu, 30 Mar 2023 05:52:14 GMT  
		Size: 119.2 MB (119192990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676425ccabf86db6a54c5e02a8fbcf0eeb15fd61d316f55e82dceaf1f55b51c0`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:50011c015d339747e2197d89c01ce5c43d70787b17c5258550ed72a32837a698
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179526750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b19e4053185eab694f5cc4560198a7844f99c72ed0466c76634201974c14988`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 30 Mar 2023 04:41:13 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 30 Mar 2023 04:41:14 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 30 Mar 2023 04:41:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 30 Mar 2023 04:41:15 GMT
RUN mkdir /opt/files
# Thu, 30 Mar 2023 04:41:15 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 30 Mar 2023 04:41:27 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API=false
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 30 Mar 2023 04:41:29 GMT
ENV HTTP_API_PASSWORD=
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 30 Mar 2023 04:41:30 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 30 Mar 2023 04:41:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 30 Mar 2023 04:41:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 30 Mar 2023 04:41:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 30 Mar 2023 04:41:33 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 30 Mar 2023 04:41:33 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 30 Mar 2023 04:41:33 GMT
EXPOSE 8080 9000
# Thu, 30 Mar 2023 04:41:34 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 30 Mar 2023 04:41:34 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da411f5e57228fc6ab3c2c80db68f2b17b12757d9358a6e5aa62c4773db299`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f55f0c0813a9eccaeb6c9520bf21732bc9ca0fc4fefd6b9663623e0892add7`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad699058479ff506d709f063ad09e1b477d3e9559b2a64efa9f4ffcad9be51`  
		Last Modified: Thu, 30 Mar 2023 04:42:28 GMT  
		Size: 119.2 MB (119193021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73194802a67d20f44ac1983e818bbb1b6b5311e5a6e62993a74804dd2d06ea9d`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0`

```console
$ docker pull bonita@sha256:11f53452b17e141a0c5fdc15578a1e3d0dba68d5c164253fcdcf314995be930d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:8.0` - linux; amd64

```console
$ docker pull bonita@sha256:671e25712bfc85accf4dc1ed5c634189a22cbe822aff8b96b20530fb9eaa5fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182362741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9b487300e970a4c211866c39542dce65173437ff1e5ed81e3dcb757acea0b8`
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
# Fri, 12 May 2023 23:21:11 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:21:12 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:21:12 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:21:12 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:21:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:21:20 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:21:20 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:21:20 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:21:20 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:21:20 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:21:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:21:20 GMT
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
	-	`sha256:fc024f2018f095be1f969500043d752fea087126f5e717898f989bbac61d9648`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3abbfe454b6771aa95ee693d8cfdadf037b5ada933d6166199726f63416401`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2b891bcd8514ebd87acc138b21f94fc7887a6b7be1d9447a0c48715f6c8`  
		Last Modified: Fri, 12 May 2023 23:21:43 GMT  
		Size: 118.2 MB (118180349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f83ff9c63c97121b9869fd09818516ec942220882952acc577d9fcf5be2176`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e986c19aa412b1939cd9e024f952407dde3cfc9bd55f1d2c7167698ffb3e7a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181520385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d8bc7d90e9b3e7c7c20c5728addd3ee3e63c05c4ea28e2f0bd924c5156e4ac`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:40:28 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:40:28 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:40:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:40:29 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:40:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:40:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:40:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:40:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:40:36 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:40:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:40:36 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:40:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:40:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11673db2efafcb36686ba9eaa4f032539371359afaa89493f178cfd965ca42ea`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f59596b02df4ba2281fb8cab9daf79fc8c0f35d7e68df47e9a7faf42a99a679`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c5729859f84e96b19636a3075d1898856fc585a3f3340cab01cbe5d64953e`  
		Last Modified: Fri, 12 May 2023 23:40:55 GMT  
		Size: 118.2 MB (118180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b54b8456e5db77a19f5cf047f9edfcdb00d3bc5c799b5cd66b2015fdfebef5`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:2efca8654cb0857363866bd85862926480ab68bfc613e0b94719c6d43b2b63bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178513984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d37bdafe7d4e5dc51a8949cac9203924d086fd6463e9a221e7dae89dfc2f821`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:16:24 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:16:25 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:16:25 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:16:25 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:27 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:16:27 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:16:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:16:41 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:16:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:16:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:16:45 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:16:46 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:16:46 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:16:47 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:16:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4caf1742a2ac14b306ff6452757d52d0901199c2ec158d720f19e45814f979`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f335bc5712f928f5123f04d81e8ace34f8816375451e908c97681bf28cf573fd`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 3.0 KB (3041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f1cdc1b30dc0a3c9f9d526851338a1cd2d98aa8eed74439c6e2dffd94c815`  
		Last Modified: Fri, 12 May 2023 23:17:20 GMT  
		Size: 118.2 MB (118180260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bddbcc08c63b72dc1302495dd5d2555ee89a1e701b9753aa0b912dd800c216`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0.0`

```console
$ docker pull bonita@sha256:11f53452b17e141a0c5fdc15578a1e3d0dba68d5c164253fcdcf314995be930d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:8.0.0` - linux; amd64

```console
$ docker pull bonita@sha256:671e25712bfc85accf4dc1ed5c634189a22cbe822aff8b96b20530fb9eaa5fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182362741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9b487300e970a4c211866c39542dce65173437ff1e5ed81e3dcb757acea0b8`
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
# Fri, 12 May 2023 23:21:11 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:21:12 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:21:12 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:21:12 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:21:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:21:20 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:21:20 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:21:20 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:21:20 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:21:20 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:21:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:21:20 GMT
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
	-	`sha256:fc024f2018f095be1f969500043d752fea087126f5e717898f989bbac61d9648`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3abbfe454b6771aa95ee693d8cfdadf037b5ada933d6166199726f63416401`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2b891bcd8514ebd87acc138b21f94fc7887a6b7be1d9447a0c48715f6c8`  
		Last Modified: Fri, 12 May 2023 23:21:43 GMT  
		Size: 118.2 MB (118180349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f83ff9c63c97121b9869fd09818516ec942220882952acc577d9fcf5be2176`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e986c19aa412b1939cd9e024f952407dde3cfc9bd55f1d2c7167698ffb3e7a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181520385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d8bc7d90e9b3e7c7c20c5728addd3ee3e63c05c4ea28e2f0bd924c5156e4ac`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:40:28 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:40:28 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:40:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:40:29 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:40:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:40:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:40:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:40:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:40:36 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:40:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:40:36 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:40:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:40:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11673db2efafcb36686ba9eaa4f032539371359afaa89493f178cfd965ca42ea`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f59596b02df4ba2281fb8cab9daf79fc8c0f35d7e68df47e9a7faf42a99a679`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c5729859f84e96b19636a3075d1898856fc585a3f3340cab01cbe5d64953e`  
		Last Modified: Fri, 12 May 2023 23:40:55 GMT  
		Size: 118.2 MB (118180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b54b8456e5db77a19f5cf047f9edfcdb00d3bc5c799b5cd66b2015fdfebef5`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:2efca8654cb0857363866bd85862926480ab68bfc613e0b94719c6d43b2b63bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178513984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d37bdafe7d4e5dc51a8949cac9203924d086fd6463e9a221e7dae89dfc2f821`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:16:24 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:16:25 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:16:25 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:16:25 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:27 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:16:27 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:16:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:16:41 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:16:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:16:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:16:45 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:16:46 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:16:46 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:16:47 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:16:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4caf1742a2ac14b306ff6452757d52d0901199c2ec158d720f19e45814f979`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f335bc5712f928f5123f04d81e8ace34f8816375451e908c97681bf28cf573fd`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 3.0 KB (3041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f1cdc1b30dc0a3c9f9d526851338a1cd2d98aa8eed74439c6e2dffd94c815`  
		Last Modified: Fri, 12 May 2023 23:17:20 GMT  
		Size: 118.2 MB (118180260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bddbcc08c63b72dc1302495dd5d2555ee89a1e701b9753aa0b912dd800c216`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:11f53452b17e141a0c5fdc15578a1e3d0dba68d5c164253fcdcf314995be930d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:671e25712bfc85accf4dc1ed5c634189a22cbe822aff8b96b20530fb9eaa5fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182362741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9b487300e970a4c211866c39542dce65173437ff1e5ed81e3dcb757acea0b8`
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
# Fri, 12 May 2023 23:21:11 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:21:12 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:21:12 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:21:12 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:21:12 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:21:12 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:21:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:21:19 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:21:19 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:21:20 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:21:20 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:21:20 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:21:20 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:21:20 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:21:20 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:21:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:21:20 GMT
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
	-	`sha256:fc024f2018f095be1f969500043d752fea087126f5e717898f989bbac61d9648`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3abbfe454b6771aa95ee693d8cfdadf037b5ada933d6166199726f63416401`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2b891bcd8514ebd87acc138b21f94fc7887a6b7be1d9447a0c48715f6c8`  
		Last Modified: Fri, 12 May 2023 23:21:43 GMT  
		Size: 118.2 MB (118180349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f83ff9c63c97121b9869fd09818516ec942220882952acc577d9fcf5be2176`  
		Last Modified: Fri, 12 May 2023 23:21:37 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e986c19aa412b1939cd9e024f952407dde3cfc9bd55f1d2c7167698ffb3e7a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181520385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d8bc7d90e9b3e7c7c20c5728addd3ee3e63c05c4ea28e2f0bd924c5156e4ac`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:51:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 05:51:25 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 05:51:26 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 05:51:27 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 05:51:27 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:40:28 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:40:28 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:40:28 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:40:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:40:29 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:40:29 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:40:34 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:40:35 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:40:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:40:35 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:40:35 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:40:35 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:40:36 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:40:36 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:40:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:40:36 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:40:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:40:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bbf643df1280e20f957edd46b2e71f4e8b9b10089468b0f6fc0f76fbe90b6`  
		Last Modified: Thu, 30 Mar 2023 05:52:16 GMT  
		Size: 60.6 MB (60620704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99825908ee88cc2e0df06b6ee7b243b2f337c9738fc702a0219aca6c23b16f15`  
		Last Modified: Thu, 30 Mar 2023 05:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3d8821b728bb52febe23bade4432048a89df5efc3104a97d23a9f695a13f2`  
		Last Modified: Thu, 30 Mar 2023 05:52:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11673db2efafcb36686ba9eaa4f032539371359afaa89493f178cfd965ca42ea`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f59596b02df4ba2281fb8cab9daf79fc8c0f35d7e68df47e9a7faf42a99a679`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c5729859f84e96b19636a3075d1898856fc585a3f3340cab01cbe5d64953e`  
		Last Modified: Fri, 12 May 2023 23:40:55 GMT  
		Size: 118.2 MB (118180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b54b8456e5db77a19f5cf047f9edfcdb00d3bc5c799b5cd66b2015fdfebef5`  
		Last Modified: Fri, 12 May 2023 23:40:49 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:2efca8654cb0857363866bd85862926480ab68bfc613e0b94719c6d43b2b63bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178513984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d37bdafe7d4e5dc51a8949cac9203924d086fd6463e9a221e7dae89dfc2f821`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:40:56 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 30 Mar 2023 04:41:07 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 30 Mar 2023 04:41:10 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 30 Mar 2023 04:41:11 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BONITA_VERSION
# Thu, 30 Mar 2023 04:41:11 GMT
ARG BRANDING_VERSION
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_SHA256
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BASE_URL
# Thu, 30 Mar 2023 04:41:12 GMT
ARG BONITA_URL
# Fri, 12 May 2023 23:16:24 GMT
ENV BONITA_VERSION=8.0.0
# Fri, 12 May 2023 23:16:25 GMT
ENV BRANDING_VERSION=2023.1-u0
# Fri, 12 May 2023 23:16:25 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Fri, 12 May 2023 23:16:25 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 12 May 2023 23:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Fri, 12 May 2023 23:16:27 GMT
RUN mkdir /opt/files
# Fri, 12 May 2023 23:16:27 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 12 May 2023 23:16:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 12 May 2023 23:16:41 GMT
ENV HTTP_API=false
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 12 May 2023 23:16:42 GMT
ENV HTTP_API_PASSWORD=
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 12 May 2023 23:16:43 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 12 May 2023 23:16:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 12 May 2023 23:16:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 12 May 2023 23:16:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 12 May 2023 23:16:45 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 12 May 2023 23:16:45 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 12 May 2023 23:16:46 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 12 May 2023 23:16:46 GMT
EXPOSE 8080 9000
# Fri, 12 May 2023 23:16:47 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 12 May 2023 23:16:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1a9ce88a6ff3344045d3eac3f3036bb2690eb3d53b0dba8a61bcb24f6c140`  
		Last Modified: Thu, 30 Mar 2023 04:42:33 GMT  
		Size: 57.5 MB (57519030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d739edd95d1b6654cc5ecb847fb534dc1f0509cfc5802b974b546462e20e3`  
		Last Modified: Thu, 30 Mar 2023 04:42:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aba4e17582878d5308fdd9b245e71be39a5fa9b8ee3c493f0c283da5306cff5`  
		Last Modified: Thu, 30 Mar 2023 04:42:18 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4caf1742a2ac14b306ff6452757d52d0901199c2ec158d720f19e45814f979`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f335bc5712f928f5123f04d81e8ace34f8816375451e908c97681bf28cf573fd`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 3.0 KB (3041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f1cdc1b30dc0a3c9f9d526851338a1cd2d98aa8eed74439c6e2dffd94c815`  
		Last Modified: Fri, 12 May 2023 23:17:20 GMT  
		Size: 118.2 MB (118180260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bddbcc08c63b72dc1302495dd5d2555ee89a1e701b9753aa0b912dd800c216`  
		Last Modified: Fri, 12 May 2023 23:17:10 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
