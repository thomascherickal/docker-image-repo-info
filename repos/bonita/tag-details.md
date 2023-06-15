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
$ docker pull bonita@sha256:f274a61d7e41927b137bd8ed10403b7ee4fdc6b1255ad7cf5c1f7e83022b92e0
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
$ docker pull bonita@sha256:62315eb311feaed84162866583ee18f359dd4fce0fb4048a9e5c3d7785492547
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176256954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90395e96968561e7a1c5f90f9428cb61eabe62720397788e61de9bfcac03537e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:34 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 14 Jun 2023 22:34:36 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 14 Jun 2023 22:34:37 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:37 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 14 Jun 2023 22:34:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:34:44 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:34:45 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:34:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:34:45 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:34:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:34:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f02a107b075ca0cb50bad0d6974d4d655be34fc49a94a35d05bc13b4102cd4`  
		Last Modified: Wed, 14 Jun 2023 22:36:02 GMT  
		Size: 56.8 MB (56835295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b27266f5318ee8fe715adcbc2de4434a6d76a1c5a292c58ce739269099935e`  
		Last Modified: Wed, 14 Jun 2023 22:35:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f38fade0d6f0c0da7e5ffe7c9db179194f2d6d9e1f7044256f06786a7e5a8`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e215ce6bc763868e36369abf67f32e5e8e12958ffdc0d8719946744de5fd449`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f9e4878a362c5eaa06f4fa5f5131f409be8c9891c867289e66e2f09ed8f5ed`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b4f0760d7adacd2b3c0fdc75335e5f3168cf03600046ac7259085f8507b07d`  
		Last Modified: Wed, 14 Jun 2023 22:35:59 GMT  
		Size: 116.7 MB (116690839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b3d75c3d8a0b3e40f543ef23d3c2826031e79cde4bb72dc711b12ee87f6df`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:eaa13f4e315d4eafe157a4d261eff809e0b201dd3b1b08a66e67ea9aa1b47591
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172852046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df3b519c6ea96bb06f5fe9f8aa17b290b2643452c4b182d634d53ff12e4341a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:09 GMT
ADD file:ea78fdaa06626dcaebd3d0aabc846e66a19d82b02ecda2f2f1c33a9573b30599 in / 
# Thu, 15 Jun 2023 00:40:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:13:27 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 15 Jun 2023 02:13:30 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:13:31 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 15 Jun 2023 02:13:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:34 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:13:34 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 15 Jun 2023 02:13:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:13:48 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:13:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:13:52 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:13:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:13:52 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:13:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:13:53 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0d07e7f561c7480cbc0d1b69f8181f36e608d2787dd33b3b7630f522de5155e2`  
		Last Modified: Thu, 15 Jun 2023 00:40:58 GMT  
		Size: 2.8 MB (2812366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6986af4d616e1912ed0d86f954a33dbd3c048bfbfa3df2115a98623c765eea`  
		Last Modified: Thu, 15 Jun 2023 02:15:32 GMT  
		Size: 53.3 MB (53338882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea8bd0c1c2f2e455754faa288c9af4065a0c1a6733b5e680edd765f423791b`  
		Last Modified: Thu, 15 Jun 2023 02:15:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea7fa045a081de6b1d741949b4de0f90fb145bac904daa099f76c78a6fa8055`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16988511cff8d59816e7e7923fd0cced52e72b40a976b2cd51daba496e3924d8`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c05e7efc271c2acb671910f99ac719eaa590769ed0f318c28761e6bd02f6f00`  
		Last Modified: Thu, 15 Jun 2023 02:15:18 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4695bff5bba30485cd628ef35708148d708112fe91cfd74b793e47cbcb8f2b6`  
		Last Modified: Thu, 15 Jun 2023 02:15:27 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25fa8d20411912ec07a2af496f6997a1d132a6dc0c12a20a76dad74847c4d21`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:f274a61d7e41927b137bd8ed10403b7ee4fdc6b1255ad7cf5c1f7e83022b92e0
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
$ docker pull bonita@sha256:62315eb311feaed84162866583ee18f359dd4fce0fb4048a9e5c3d7785492547
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176256954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90395e96968561e7a1c5f90f9428cb61eabe62720397788e61de9bfcac03537e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:34 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 14 Jun 2023 22:34:36 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 14 Jun 2023 22:34:37 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:37 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 14 Jun 2023 22:34:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:34:44 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:34:45 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:34:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:34:45 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:34:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:34:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f02a107b075ca0cb50bad0d6974d4d655be34fc49a94a35d05bc13b4102cd4`  
		Last Modified: Wed, 14 Jun 2023 22:36:02 GMT  
		Size: 56.8 MB (56835295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b27266f5318ee8fe715adcbc2de4434a6d76a1c5a292c58ce739269099935e`  
		Last Modified: Wed, 14 Jun 2023 22:35:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f38fade0d6f0c0da7e5ffe7c9db179194f2d6d9e1f7044256f06786a7e5a8`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e215ce6bc763868e36369abf67f32e5e8e12958ffdc0d8719946744de5fd449`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f9e4878a362c5eaa06f4fa5f5131f409be8c9891c867289e66e2f09ed8f5ed`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b4f0760d7adacd2b3c0fdc75335e5f3168cf03600046ac7259085f8507b07d`  
		Last Modified: Wed, 14 Jun 2023 22:35:59 GMT  
		Size: 116.7 MB (116690839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b3d75c3d8a0b3e40f543ef23d3c2826031e79cde4bb72dc711b12ee87f6df`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:eaa13f4e315d4eafe157a4d261eff809e0b201dd3b1b08a66e67ea9aa1b47591
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172852046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df3b519c6ea96bb06f5fe9f8aa17b290b2643452c4b182d634d53ff12e4341a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:09 GMT
ADD file:ea78fdaa06626dcaebd3d0aabc846e66a19d82b02ecda2f2f1c33a9573b30599 in / 
# Thu, 15 Jun 2023 00:40:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:13:27 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 15 Jun 2023 02:13:30 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:13:31 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 15 Jun 2023 02:13:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:34 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:13:34 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 15 Jun 2023 02:13:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:13:48 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:13:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:13:52 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:13:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:13:52 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:13:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:13:53 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0d07e7f561c7480cbc0d1b69f8181f36e608d2787dd33b3b7630f522de5155e2`  
		Last Modified: Thu, 15 Jun 2023 00:40:58 GMT  
		Size: 2.8 MB (2812366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6986af4d616e1912ed0d86f954a33dbd3c048bfbfa3df2115a98623c765eea`  
		Last Modified: Thu, 15 Jun 2023 02:15:32 GMT  
		Size: 53.3 MB (53338882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea8bd0c1c2f2e455754faa288c9af4065a0c1a6733b5e680edd765f423791b`  
		Last Modified: Thu, 15 Jun 2023 02:15:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea7fa045a081de6b1d741949b4de0f90fb145bac904daa099f76c78a6fa8055`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16988511cff8d59816e7e7923fd0cced52e72b40a976b2cd51daba496e3924d8`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c05e7efc271c2acb671910f99ac719eaa590769ed0f318c28761e6bd02f6f00`  
		Last Modified: Thu, 15 Jun 2023 02:15:18 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4695bff5bba30485cd628ef35708148d708112fe91cfd74b793e47cbcb8f2b6`  
		Last Modified: Thu, 15 Jun 2023 02:15:27 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25fa8d20411912ec07a2af496f6997a1d132a6dc0c12a20a76dad74847c4d21`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:7d21b5032b5a11ea1ba468d7c1dc8aa60212d593c333628f38a741bbdaadf8d6
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
$ docker pull bonita@sha256:ea95c5e49084f352d30048f2357df95324e4a0e703312c1eb8795c619c48fc04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182580767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820f81fb11d9f9c6d20ac22b0dea18ddb3d92c1dda360e21ba145fda50a17f01`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 14 Jun 2023 22:34:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:56 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:15 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:15 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:15 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:15 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d297da91c8bdf5296576b8b9ba2dd4245ba16bd65725d0e6e7bc06f7aba5d3ad`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3b8245237342d17a7a9e101012c3b05de16baa934b59a632cb5d777220d44`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491972b6c388fd2883c13e157ff560f97bfcd9dea3812c87045a93e9eab9949`  
		Last Modified: Wed, 14 Jun 2023 22:36:20 GMT  
		Size: 119.2 MB (119192986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857c1d2ffc1812854b9422d41c79f735e4395f80b1a1f0dd5605094f360f14ae`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:5a51c68ed62aaa34d67273de19d59235730c58ee45022b325478ab5a865fe6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179573697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb555e5dd445167a023a2ee63da1985801110c292212478485d139f0e5d477f1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 15 Jun 2023 02:14:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:18 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:18 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:33 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:33 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:35 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:14:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:14:35 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:14:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:14:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62520dc5418447dd78b88c7bead906b4609496a3c6bdf81d6e3f448240ad41c0`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fd88da2b5f60c6a857fe3930853a30bb87a4c2756d45c33a2770456f6bd047`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf7bdfb905f59a9f5703375bde79bebc8f7f88c556c61cfd206a6366d516321`  
		Last Modified: Thu, 15 Jun 2023 02:15:55 GMT  
		Size: 119.2 MB (119192976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b299db4533008bb5533776bd1babedf0de77f6bf5ede2aa02a282cbe1b938c`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:7d21b5032b5a11ea1ba468d7c1dc8aa60212d593c333628f38a741bbdaadf8d6
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
$ docker pull bonita@sha256:ea95c5e49084f352d30048f2357df95324e4a0e703312c1eb8795c619c48fc04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182580767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820f81fb11d9f9c6d20ac22b0dea18ddb3d92c1dda360e21ba145fda50a17f01`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 14 Jun 2023 22:34:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:56 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:15 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:15 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:15 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:15 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d297da91c8bdf5296576b8b9ba2dd4245ba16bd65725d0e6e7bc06f7aba5d3ad`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3b8245237342d17a7a9e101012c3b05de16baa934b59a632cb5d777220d44`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491972b6c388fd2883c13e157ff560f97bfcd9dea3812c87045a93e9eab9949`  
		Last Modified: Wed, 14 Jun 2023 22:36:20 GMT  
		Size: 119.2 MB (119192986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857c1d2ffc1812854b9422d41c79f735e4395f80b1a1f0dd5605094f360f14ae`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:5a51c68ed62aaa34d67273de19d59235730c58ee45022b325478ab5a865fe6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179573697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb555e5dd445167a023a2ee63da1985801110c292212478485d139f0e5d477f1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 15 Jun 2023 02:14:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:18 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:18 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:33 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:33 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:35 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:14:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:14:35 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:14:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:14:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62520dc5418447dd78b88c7bead906b4609496a3c6bdf81d6e3f448240ad41c0`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fd88da2b5f60c6a857fe3930853a30bb87a4c2756d45c33a2770456f6bd047`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf7bdfb905f59a9f5703375bde79bebc8f7f88c556c61cfd206a6366d516321`  
		Last Modified: Thu, 15 Jun 2023 02:15:55 GMT  
		Size: 119.2 MB (119192976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b299db4533008bb5533776bd1babedf0de77f6bf5ede2aa02a282cbe1b938c`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1`

```console
$ docker pull bonita@sha256:62edaa3fb7d56f777da0201dd8a021b9363c77608d019383662462d8214f97fa
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
$ docker pull bonita@sha256:de307e1c30ec4048b070fcff754bb0a71209aa4ce2c32bae1fd8ddff5de45ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181568082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce39fd607136e2cf747e16e35ea7ed8646cd07c0a41f375f99c6df93827fe8e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_VERSION=8.0.0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BRANDING_VERSION=2023.1-u0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Wed, 14 Jun 2023 22:35:21 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:22 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:35:22 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:30 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:30 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:30 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a489ba903c8f36b195bb6acacb6b487fb0fc7cdc21526bccd022ab631cc76c3`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ad0831b7bcc19c72490be2fd152ac6238a484946049965f932a14bd64d2b7`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 3.0 KB (3042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0831d844e78da343cdc25c28f4400dec6fd6d0381afa81d20485bebe3a039`  
		Last Modified: Wed, 14 Jun 2023 22:36:41 GMT  
		Size: 118.2 MB (118180305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c1aa1efbe77104faeda5d6fb1925623fcd3e244145f4e553c1411c179e3cfd`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:8dfc2995c764321e5ca0de1e36cebd61eeccdd5093c9163203e4eff813ba73e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178561019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa36bd0a548abd7baa7d45cc2cc69152cab2cbc4464e6028f30c9a40f31597a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:39 GMT
ENV BONITA_VERSION=8.0.0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BRANDING_VERSION=2023.1-u0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Thu, 15 Jun 2023 02:14:40 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:42 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:55 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:59 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:15:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:15:00 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:15:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:15:01 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e6138af815e96a0f82b5b9dce971bdc05cf088da06deb7634759305df051ad`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05068c01ad423d9c268355d34a45847f46ed6398ca5d8de3684beb61df413988`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe2a7d56f73ec617880f563898f497d5fe3b6aaa7ae8b844ceb3344f4adf16`  
		Last Modified: Thu, 15 Jun 2023 02:16:24 GMT  
		Size: 118.2 MB (118180298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2ddbf70a4acc9354a263977f9db6636a169cff2a02fd6b15cbed90bea964c2`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1-u0`

```console
$ docker pull bonita@sha256:62edaa3fb7d56f777da0201dd8a021b9363c77608d019383662462d8214f97fa
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
$ docker pull bonita@sha256:de307e1c30ec4048b070fcff754bb0a71209aa4ce2c32bae1fd8ddff5de45ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181568082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce39fd607136e2cf747e16e35ea7ed8646cd07c0a41f375f99c6df93827fe8e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_VERSION=8.0.0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BRANDING_VERSION=2023.1-u0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Wed, 14 Jun 2023 22:35:21 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:22 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:35:22 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:30 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:30 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:30 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a489ba903c8f36b195bb6acacb6b487fb0fc7cdc21526bccd022ab631cc76c3`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ad0831b7bcc19c72490be2fd152ac6238a484946049965f932a14bd64d2b7`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 3.0 KB (3042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0831d844e78da343cdc25c28f4400dec6fd6d0381afa81d20485bebe3a039`  
		Last Modified: Wed, 14 Jun 2023 22:36:41 GMT  
		Size: 118.2 MB (118180305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c1aa1efbe77104faeda5d6fb1925623fcd3e244145f4e553c1411c179e3cfd`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8dfc2995c764321e5ca0de1e36cebd61eeccdd5093c9163203e4eff813ba73e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178561019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa36bd0a548abd7baa7d45cc2cc69152cab2cbc4464e6028f30c9a40f31597a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:39 GMT
ENV BONITA_VERSION=8.0.0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BRANDING_VERSION=2023.1-u0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Thu, 15 Jun 2023 02:14:40 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:42 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:55 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:59 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:15:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:15:00 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:15:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:15:01 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e6138af815e96a0f82b5b9dce971bdc05cf088da06deb7634759305df051ad`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05068c01ad423d9c268355d34a45847f46ed6398ca5d8de3684beb61df413988`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe2a7d56f73ec617880f563898f497d5fe3b6aaa7ae8b844ceb3344f4adf16`  
		Last Modified: Thu, 15 Jun 2023 02:16:24 GMT  
		Size: 118.2 MB (118180298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2ddbf70a4acc9354a263977f9db6636a169cff2a02fd6b15cbed90bea964c2`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 5.4 KB (5425 bytes)  
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
$ docker pull bonita@sha256:f274a61d7e41927b137bd8ed10403b7ee4fdc6b1255ad7cf5c1f7e83022b92e0
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
$ docker pull bonita@sha256:62315eb311feaed84162866583ee18f359dd4fce0fb4048a9e5c3d7785492547
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176256954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90395e96968561e7a1c5f90f9428cb61eabe62720397788e61de9bfcac03537e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:34 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 14 Jun 2023 22:34:36 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 14 Jun 2023 22:34:37 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:37 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 14 Jun 2023 22:34:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:34:44 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:34:45 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:34:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:34:45 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:34:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:34:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f02a107b075ca0cb50bad0d6974d4d655be34fc49a94a35d05bc13b4102cd4`  
		Last Modified: Wed, 14 Jun 2023 22:36:02 GMT  
		Size: 56.8 MB (56835295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b27266f5318ee8fe715adcbc2de4434a6d76a1c5a292c58ce739269099935e`  
		Last Modified: Wed, 14 Jun 2023 22:35:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f38fade0d6f0c0da7e5ffe7c9db179194f2d6d9e1f7044256f06786a7e5a8`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e215ce6bc763868e36369abf67f32e5e8e12958ffdc0d8719946744de5fd449`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f9e4878a362c5eaa06f4fa5f5131f409be8c9891c867289e66e2f09ed8f5ed`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b4f0760d7adacd2b3c0fdc75335e5f3168cf03600046ac7259085f8507b07d`  
		Last Modified: Wed, 14 Jun 2023 22:35:59 GMT  
		Size: 116.7 MB (116690839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b3d75c3d8a0b3e40f543ef23d3c2826031e79cde4bb72dc711b12ee87f6df`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:eaa13f4e315d4eafe157a4d261eff809e0b201dd3b1b08a66e67ea9aa1b47591
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172852046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df3b519c6ea96bb06f5fe9f8aa17b290b2643452c4b182d634d53ff12e4341a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:09 GMT
ADD file:ea78fdaa06626dcaebd3d0aabc846e66a19d82b02ecda2f2f1c33a9573b30599 in / 
# Thu, 15 Jun 2023 00:40:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:13:27 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 15 Jun 2023 02:13:30 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:13:31 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 15 Jun 2023 02:13:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:34 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:13:34 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 15 Jun 2023 02:13:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:13:48 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:13:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:13:52 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:13:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:13:52 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:13:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:13:53 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0d07e7f561c7480cbc0d1b69f8181f36e608d2787dd33b3b7630f522de5155e2`  
		Last Modified: Thu, 15 Jun 2023 00:40:58 GMT  
		Size: 2.8 MB (2812366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6986af4d616e1912ed0d86f954a33dbd3c048bfbfa3df2115a98623c765eea`  
		Last Modified: Thu, 15 Jun 2023 02:15:32 GMT  
		Size: 53.3 MB (53338882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea8bd0c1c2f2e455754faa288c9af4065a0c1a6733b5e680edd765f423791b`  
		Last Modified: Thu, 15 Jun 2023 02:15:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea7fa045a081de6b1d741949b4de0f90fb145bac904daa099f76c78a6fa8055`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16988511cff8d59816e7e7923fd0cced52e72b40a976b2cd51daba496e3924d8`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c05e7efc271c2acb671910f99ac719eaa590769ed0f318c28761e6bd02f6f00`  
		Last Modified: Thu, 15 Jun 2023 02:15:18 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4695bff5bba30485cd628ef35708148d708112fe91cfd74b793e47cbcb8f2b6`  
		Last Modified: Thu, 15 Jun 2023 02:15:27 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25fa8d20411912ec07a2af496f6997a1d132a6dc0c12a20a76dad74847c4d21`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:f274a61d7e41927b137bd8ed10403b7ee4fdc6b1255ad7cf5c1f7e83022b92e0
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
$ docker pull bonita@sha256:62315eb311feaed84162866583ee18f359dd4fce0fb4048a9e5c3d7785492547
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176256954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90395e96968561e7a1c5f90f9428cb61eabe62720397788e61de9bfcac03537e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:34 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 14 Jun 2023 22:34:36 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:36 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:36 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 14 Jun 2023 22:34:37 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 14 Jun 2023 22:34:37 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:37 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 14 Jun 2023 22:34:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:34:44 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:34:44 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:34:44 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:34:44 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:34:45 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:34:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:34:45 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:34:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:34:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f02a107b075ca0cb50bad0d6974d4d655be34fc49a94a35d05bc13b4102cd4`  
		Last Modified: Wed, 14 Jun 2023 22:36:02 GMT  
		Size: 56.8 MB (56835295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b27266f5318ee8fe715adcbc2de4434a6d76a1c5a292c58ce739269099935e`  
		Last Modified: Wed, 14 Jun 2023 22:35:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f38fade0d6f0c0da7e5ffe7c9db179194f2d6d9e1f7044256f06786a7e5a8`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e215ce6bc763868e36369abf67f32e5e8e12958ffdc0d8719946744de5fd449`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f9e4878a362c5eaa06f4fa5f5131f409be8c9891c867289e66e2f09ed8f5ed`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b4f0760d7adacd2b3c0fdc75335e5f3168cf03600046ac7259085f8507b07d`  
		Last Modified: Wed, 14 Jun 2023 22:35:59 GMT  
		Size: 116.7 MB (116690839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b3d75c3d8a0b3e40f543ef23d3c2826031e79cde4bb72dc711b12ee87f6df`  
		Last Modified: Wed, 14 Jun 2023 22:35:54 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:eaa13f4e315d4eafe157a4d261eff809e0b201dd3b1b08a66e67ea9aa1b47591
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172852046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df3b519c6ea96bb06f5fe9f8aa17b290b2643452c4b182d634d53ff12e4341a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:09 GMT
ADD file:ea78fdaa06626dcaebd3d0aabc846e66a19d82b02ecda2f2f1c33a9573b30599 in / 
# Thu, 15 Jun 2023 00:40:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:13:27 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 15 Jun 2023 02:13:30 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:13:31 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:13:31 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 15 Jun 2023 02:13:32 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 15 Jun 2023 02:13:33 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:13:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 15 Jun 2023 02:13:34 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:13:34 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 15 Jun 2023 02:13:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:13:48 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:13:49 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:13:49 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:13:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:13:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:13:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:13:52 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:13:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:13:52 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:13:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:13:53 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0d07e7f561c7480cbc0d1b69f8181f36e608d2787dd33b3b7630f522de5155e2`  
		Last Modified: Thu, 15 Jun 2023 00:40:58 GMT  
		Size: 2.8 MB (2812366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6986af4d616e1912ed0d86f954a33dbd3c048bfbfa3df2115a98623c765eea`  
		Last Modified: Thu, 15 Jun 2023 02:15:32 GMT  
		Size: 53.3 MB (53338882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea8bd0c1c2f2e455754faa288c9af4065a0c1a6733b5e680edd765f423791b`  
		Last Modified: Thu, 15 Jun 2023 02:15:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea7fa045a081de6b1d741949b4de0f90fb145bac904daa099f76c78a6fa8055`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16988511cff8d59816e7e7923fd0cced52e72b40a976b2cd51daba496e3924d8`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c05e7efc271c2acb671910f99ac719eaa590769ed0f318c28761e6bd02f6f00`  
		Last Modified: Thu, 15 Jun 2023 02:15:18 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4695bff5bba30485cd628ef35708148d708112fe91cfd74b793e47cbcb8f2b6`  
		Last Modified: Thu, 15 Jun 2023 02:15:27 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25fa8d20411912ec07a2af496f6997a1d132a6dc0c12a20a76dad74847c4d21`  
		Last Modified: Thu, 15 Jun 2023 02:15:17 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:7d21b5032b5a11ea1ba468d7c1dc8aa60212d593c333628f38a741bbdaadf8d6
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
$ docker pull bonita@sha256:ea95c5e49084f352d30048f2357df95324e4a0e703312c1eb8795c619c48fc04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182580767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820f81fb11d9f9c6d20ac22b0dea18ddb3d92c1dda360e21ba145fda50a17f01`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 14 Jun 2023 22:34:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:56 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:15 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:15 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:15 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:15 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d297da91c8bdf5296576b8b9ba2dd4245ba16bd65725d0e6e7bc06f7aba5d3ad`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3b8245237342d17a7a9e101012c3b05de16baa934b59a632cb5d777220d44`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491972b6c388fd2883c13e157ff560f97bfcd9dea3812c87045a93e9eab9949`  
		Last Modified: Wed, 14 Jun 2023 22:36:20 GMT  
		Size: 119.2 MB (119192986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857c1d2ffc1812854b9422d41c79f735e4395f80b1a1f0dd5605094f360f14ae`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:5a51c68ed62aaa34d67273de19d59235730c58ee45022b325478ab5a865fe6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179573697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb555e5dd445167a023a2ee63da1985801110c292212478485d139f0e5d477f1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 15 Jun 2023 02:14:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:18 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:18 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:33 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:33 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:35 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:14:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:14:35 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:14:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:14:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62520dc5418447dd78b88c7bead906b4609496a3c6bdf81d6e3f448240ad41c0`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fd88da2b5f60c6a857fe3930853a30bb87a4c2756d45c33a2770456f6bd047`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf7bdfb905f59a9f5703375bde79bebc8f7f88c556c61cfd206a6366d516321`  
		Last Modified: Thu, 15 Jun 2023 02:15:55 GMT  
		Size: 119.2 MB (119192976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b299db4533008bb5533776bd1babedf0de77f6bf5ede2aa02a282cbe1b938c`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:7d21b5032b5a11ea1ba468d7c1dc8aa60212d593c333628f38a741bbdaadf8d6
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
$ docker pull bonita@sha256:ea95c5e49084f352d30048f2357df95324e4a0e703312c1eb8795c619c48fc04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182580767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820f81fb11d9f9c6d20ac22b0dea18ddb3d92c1dda360e21ba145fda50a17f01`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_VERSION=7.15.0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BRANDING_VERSION=2022.2-u0
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Wed, 14 Jun 2023 22:34:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:34:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Wed, 14 Jun 2023 22:34:55 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:34:56 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:14 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:15 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:15 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:15 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:15 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d297da91c8bdf5296576b8b9ba2dd4245ba16bd65725d0e6e7bc06f7aba5d3ad`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3b8245237342d17a7a9e101012c3b05de16baa934b59a632cb5d777220d44`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491972b6c388fd2883c13e157ff560f97bfcd9dea3812c87045a93e9eab9949`  
		Last Modified: Wed, 14 Jun 2023 22:36:20 GMT  
		Size: 119.2 MB (119192986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857c1d2ffc1812854b9422d41c79f735e4395f80b1a1f0dd5605094f360f14ae`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:5a51c68ed62aaa34d67273de19d59235730c58ee45022b325478ab5a865fe6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179573697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb555e5dd445167a023a2ee63da1985801110c292212478485d139f0e5d477f1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_VERSION=7.15.0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BRANDING_VERSION=2022.2-u0
# Thu, 15 Jun 2023 02:14:16 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Thu, 15 Jun 2023 02:14:16 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Thu, 15 Jun 2023 02:14:18 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:18 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:32 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:33 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:33 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:33 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:34 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:35 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:14:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:14:35 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:14:36 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:14:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62520dc5418447dd78b88c7bead906b4609496a3c6bdf81d6e3f448240ad41c0`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fd88da2b5f60c6a857fe3930853a30bb87a4c2756d45c33a2770456f6bd047`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf7bdfb905f59a9f5703375bde79bebc8f7f88c556c61cfd206a6366d516321`  
		Last Modified: Thu, 15 Jun 2023 02:15:55 GMT  
		Size: 119.2 MB (119192976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b299db4533008bb5533776bd1babedf0de77f6bf5ede2aa02a282cbe1b938c`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0`

```console
$ docker pull bonita@sha256:62edaa3fb7d56f777da0201dd8a021b9363c77608d019383662462d8214f97fa
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
$ docker pull bonita@sha256:de307e1c30ec4048b070fcff754bb0a71209aa4ce2c32bae1fd8ddff5de45ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181568082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce39fd607136e2cf747e16e35ea7ed8646cd07c0a41f375f99c6df93827fe8e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_VERSION=8.0.0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BRANDING_VERSION=2023.1-u0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Wed, 14 Jun 2023 22:35:21 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:22 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:35:22 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:30 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:30 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:30 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a489ba903c8f36b195bb6acacb6b487fb0fc7cdc21526bccd022ab631cc76c3`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ad0831b7bcc19c72490be2fd152ac6238a484946049965f932a14bd64d2b7`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 3.0 KB (3042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0831d844e78da343cdc25c28f4400dec6fd6d0381afa81d20485bebe3a039`  
		Last Modified: Wed, 14 Jun 2023 22:36:41 GMT  
		Size: 118.2 MB (118180305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c1aa1efbe77104faeda5d6fb1925623fcd3e244145f4e553c1411c179e3cfd`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8dfc2995c764321e5ca0de1e36cebd61eeccdd5093c9163203e4eff813ba73e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178561019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa36bd0a548abd7baa7d45cc2cc69152cab2cbc4464e6028f30c9a40f31597a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:39 GMT
ENV BONITA_VERSION=8.0.0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BRANDING_VERSION=2023.1-u0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Thu, 15 Jun 2023 02:14:40 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:42 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:55 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:59 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:15:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:15:00 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:15:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:15:01 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e6138af815e96a0f82b5b9dce971bdc05cf088da06deb7634759305df051ad`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05068c01ad423d9c268355d34a45847f46ed6398ca5d8de3684beb61df413988`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe2a7d56f73ec617880f563898f497d5fe3b6aaa7ae8b844ceb3344f4adf16`  
		Last Modified: Thu, 15 Jun 2023 02:16:24 GMT  
		Size: 118.2 MB (118180298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2ddbf70a4acc9354a263977f9db6636a169cff2a02fd6b15cbed90bea964c2`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0.0`

```console
$ docker pull bonita@sha256:62edaa3fb7d56f777da0201dd8a021b9363c77608d019383662462d8214f97fa
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
$ docker pull bonita@sha256:de307e1c30ec4048b070fcff754bb0a71209aa4ce2c32bae1fd8ddff5de45ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181568082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce39fd607136e2cf747e16e35ea7ed8646cd07c0a41f375f99c6df93827fe8e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_VERSION=8.0.0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BRANDING_VERSION=2023.1-u0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Wed, 14 Jun 2023 22:35:21 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:22 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:35:22 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:30 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:30 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:30 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a489ba903c8f36b195bb6acacb6b487fb0fc7cdc21526bccd022ab631cc76c3`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ad0831b7bcc19c72490be2fd152ac6238a484946049965f932a14bd64d2b7`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 3.0 KB (3042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0831d844e78da343cdc25c28f4400dec6fd6d0381afa81d20485bebe3a039`  
		Last Modified: Wed, 14 Jun 2023 22:36:41 GMT  
		Size: 118.2 MB (118180305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c1aa1efbe77104faeda5d6fb1925623fcd3e244145f4e553c1411c179e3cfd`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8dfc2995c764321e5ca0de1e36cebd61eeccdd5093c9163203e4eff813ba73e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178561019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa36bd0a548abd7baa7d45cc2cc69152cab2cbc4464e6028f30c9a40f31597a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:39 GMT
ENV BONITA_VERSION=8.0.0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BRANDING_VERSION=2023.1-u0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Thu, 15 Jun 2023 02:14:40 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:42 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:55 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:59 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:15:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:15:00 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:15:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:15:01 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e6138af815e96a0f82b5b9dce971bdc05cf088da06deb7634759305df051ad`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05068c01ad423d9c268355d34a45847f46ed6398ca5d8de3684beb61df413988`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe2a7d56f73ec617880f563898f497d5fe3b6aaa7ae8b844ceb3344f4adf16`  
		Last Modified: Thu, 15 Jun 2023 02:16:24 GMT  
		Size: 118.2 MB (118180298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2ddbf70a4acc9354a263977f9db6636a169cff2a02fd6b15cbed90bea964c2`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:62edaa3fb7d56f777da0201dd8a021b9363c77608d019383662462d8214f97fa
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
$ docker pull bonita@sha256:de307e1c30ec4048b070fcff754bb0a71209aa4ce2c32bae1fd8ddff5de45ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181568082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce39fd607136e2cf747e16e35ea7ed8646cd07c0a41f375f99c6df93827fe8e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:34:47 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jun 2023 22:34:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Wed, 14 Jun 2023 22:34:54 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jun 2023 22:34:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BRANDING_VERSION
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BONITA_SHA256
# Wed, 14 Jun 2023 22:34:54 GMT
ARG BASE_URL
# Wed, 14 Jun 2023 22:34:55 GMT
ARG BONITA_URL
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_VERSION=8.0.0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BRANDING_VERSION=2023.1-u0
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Wed, 14 Jun 2023 22:35:21 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jun 2023 22:35:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Wed, 14 Jun 2023 22:35:22 GMT
RUN mkdir /opt/files
# Wed, 14 Jun 2023 22:35:22 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Wed, 14 Jun 2023 22:35:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_API_PASSWORD=
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 14 Jun 2023 22:35:29 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 14 Jun 2023 22:35:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 14 Jun 2023 22:35:29 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 14 Jun 2023 22:35:29 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 14 Jun 2023 22:35:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 14 Jun 2023 22:35:30 GMT
EXPOSE 8080 9000
# Wed, 14 Jun 2023 22:35:30 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 14 Jun 2023 22:35:30 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85088a83388e2b7484a43a43ca562a9abd87d37bed39d17660d1c14a13b2c7f7`  
		Last Modified: Wed, 14 Jun 2023 22:36:23 GMT  
		Size: 60.7 MB (60669846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ee490393db9e6fe8f134ec7fb2a9038feb15c160d67e3a7b8447f2e71da2`  
		Last Modified: Wed, 14 Jun 2023 22:36:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04719c3db371bc753cc300f49a4a33f4b03baa3b94dc0537590dc741acd3ea8`  
		Last Modified: Wed, 14 Jun 2023 22:36:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a489ba903c8f36b195bb6acacb6b487fb0fc7cdc21526bccd022ab631cc76c3`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ad0831b7bcc19c72490be2fd152ac6238a484946049965f932a14bd64d2b7`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 3.0 KB (3042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0831d844e78da343cdc25c28f4400dec6fd6d0381afa81d20485bebe3a039`  
		Last Modified: Wed, 14 Jun 2023 22:36:41 GMT  
		Size: 118.2 MB (118180305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c1aa1efbe77104faeda5d6fb1925623fcd3e244145f4e553c1411c179e3cfd`  
		Last Modified: Wed, 14 Jun 2023 22:36:36 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:8dfc2995c764321e5ca0de1e36cebd61eeccdd5093c9163203e4eff813ba73e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178561019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa36bd0a548abd7baa7d45cc2cc69152cab2cbc4464e6028f30c9a40f31597a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:13:58 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 15 Jun 2023 02:14:10 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Thu, 15 Jun 2023 02:14:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 15 Jun 2023 02:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 15 Jun 2023 02:14:14 GMT
ARG BONITA_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BRANDING_VERSION
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_SHA256
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BASE_URL
# Thu, 15 Jun 2023 02:14:15 GMT
ARG BONITA_URL
# Thu, 15 Jun 2023 02:14:39 GMT
ENV BONITA_VERSION=8.0.0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BRANDING_VERSION=2023.1-u0
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Thu, 15 Jun 2023 02:14:40 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 15 Jun 2023 02:14:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Thu, 15 Jun 2023 02:14:42 GMT
RUN mkdir /opt/files
# Thu, 15 Jun 2023 02:14:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Thu, 15 Jun 2023 02:14:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 15 Jun 2023 02:14:55 GMT
ENV HTTP_API=false
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 15 Jun 2023 02:14:56 GMT
ENV HTTP_API_PASSWORD=
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 15 Jun 2023 02:14:57 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 15 Jun 2023 02:14:57 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 15 Jun 2023 02:14:58 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 15 Jun 2023 02:14:59 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 15 Jun 2023 02:14:59 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 15 Jun 2023 02:15:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 15 Jun 2023 02:15:00 GMT
EXPOSE 8080 9000
# Thu, 15 Jun 2023 02:15:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 15 Jun 2023 02:15:01 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0c5fc81f776ecd1b977b8b6d65b74ac41f458f7e7d1140a858fc57454a948`  
		Last Modified: Thu, 15 Jun 2023 02:16:00 GMT  
		Size: 57.6 MB (57568420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e74ae83df0e1ea8c87fe5fc2c8966af2b070bf21d69091db700360f550c2`  
		Last Modified: Thu, 15 Jun 2023 02:15:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47ac2f2664d093a77e9faa55e5f8c31dae9dd4dc660e646209f7545999f496e`  
		Last Modified: Thu, 15 Jun 2023 02:15:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e6138af815e96a0f82b5b9dce971bdc05cf088da06deb7634759305df051ad`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05068c01ad423d9c268355d34a45847f46ed6398ca5d8de3684beb61df413988`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe2a7d56f73ec617880f563898f497d5fe3b6aaa7ae8b844ceb3344f4adf16`  
		Last Modified: Thu, 15 Jun 2023 02:16:24 GMT  
		Size: 118.2 MB (118180298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2ddbf70a4acc9354a263977f9db6636a169cff2a02fd6b15cbed90bea964c2`  
		Last Modified: Thu, 15 Jun 2023 02:16:14 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
