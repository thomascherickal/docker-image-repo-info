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
$ docker pull bonita@sha256:ce650e5acc90966d76ebb0c0968f5d2fe9d1b62d69cae93bdd808bce9f52f6b9
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
$ docker pull bonita@sha256:ee1f85da1a0601a58c08f5b38954b807e58e77f1c15f856c6e65c6d7069d9f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232986008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f8cedb264ee64d6eea033731ad0d9e827931e355389b1670d4603868da35a`
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
# Sat, 16 Sep 2023 02:35:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 16 Sep 2023 02:38:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:38:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 16 Sep 2023 02:38:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 16 Sep 2023 02:38:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BONITA_VERSION
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BRANDING_VERSION
# Sat, 16 Sep 2023 02:38:36 GMT
ARG BONITA_SHA256
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BASE_URL
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BONITA_URL
# Sat, 16 Sep 2023 02:38:38 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 16 Sep 2023 02:38:40 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 16 Sep 2023 02:38:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:42 GMT
RUN mkdir /opt/files
# Sat, 16 Sep 2023 02:38:42 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 16 Sep 2023 02:38:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 16 Sep 2023 02:38:57 GMT
ENV HTTP_API=false
# Sat, 16 Sep 2023 02:39:00 GMT
VOLUME [/opt/bonita]
# Sat, 16 Sep 2023 02:39:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 16 Sep 2023 02:39:03 GMT
EXPOSE 8080
# Sat, 16 Sep 2023 02:39:06 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ceefc23d77069ec288df034168091e2b853c1486fed391d1dae80c8dd41319`  
		Last Modified: Sat, 16 Sep 2023 02:39:59 GMT  
		Size: 88.0 MB (87975233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05285767062ecf2a4dbeac7e3b295a6f16b85aaed73b43d053de02361fd4ee9`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85527ce4335f69446508c3a5ec215a176f774bb26f0e289f01f869b03a3f000`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b04b643d05b9d28651f17e0200b452ec28cb6c1a34562fb14ea01d4bf6563e`  
		Last Modified: Sat, 16 Sep 2023 02:39:38 GMT  
		Size: 831.6 KB (831580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58368109f9a398b225bcf828cfe5e4e1872efadae44c7f24b8ea71a490296db6`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba19de21f79dddd4b1496ced7970f008404bb0a6a0207e5d46a86964b546b2f`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65d3fdfff12c9f01cbb893d222cf4ffa59d774f4d34d06769fd273dcfb5d25d`  
		Last Modified: Sat, 16 Sep 2023 02:39:47 GMT  
		Size: 113.7 MB (113727900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86765eaed4922054440ad8df162f88c7bb68e20fe40dc037bf19ac523b0f1c`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:ce650e5acc90966d76ebb0c0968f5d2fe9d1b62d69cae93bdd808bce9f52f6b9
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
$ docker pull bonita@sha256:ee1f85da1a0601a58c08f5b38954b807e58e77f1c15f856c6e65c6d7069d9f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232986008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f8cedb264ee64d6eea033731ad0d9e827931e355389b1670d4603868da35a`
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
# Sat, 16 Sep 2023 02:35:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 16 Sep 2023 02:38:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:38:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 16 Sep 2023 02:38:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 16 Sep 2023 02:38:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BONITA_VERSION
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BRANDING_VERSION
# Sat, 16 Sep 2023 02:38:36 GMT
ARG BONITA_SHA256
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BASE_URL
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BONITA_URL
# Sat, 16 Sep 2023 02:38:38 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 16 Sep 2023 02:38:40 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 16 Sep 2023 02:38:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:42 GMT
RUN mkdir /opt/files
# Sat, 16 Sep 2023 02:38:42 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 16 Sep 2023 02:38:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 16 Sep 2023 02:38:57 GMT
ENV HTTP_API=false
# Sat, 16 Sep 2023 02:39:00 GMT
VOLUME [/opt/bonita]
# Sat, 16 Sep 2023 02:39:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 16 Sep 2023 02:39:03 GMT
EXPOSE 8080
# Sat, 16 Sep 2023 02:39:06 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ceefc23d77069ec288df034168091e2b853c1486fed391d1dae80c8dd41319`  
		Last Modified: Sat, 16 Sep 2023 02:39:59 GMT  
		Size: 88.0 MB (87975233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05285767062ecf2a4dbeac7e3b295a6f16b85aaed73b43d053de02361fd4ee9`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85527ce4335f69446508c3a5ec215a176f774bb26f0e289f01f869b03a3f000`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b04b643d05b9d28651f17e0200b452ec28cb6c1a34562fb14ea01d4bf6563e`  
		Last Modified: Sat, 16 Sep 2023 02:39:38 GMT  
		Size: 831.6 KB (831580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58368109f9a398b225bcf828cfe5e4e1872efadae44c7f24b8ea71a490296db6`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba19de21f79dddd4b1496ced7970f008404bb0a6a0207e5d46a86964b546b2f`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65d3fdfff12c9f01cbb893d222cf4ffa59d774f4d34d06769fd273dcfb5d25d`  
		Last Modified: Sat, 16 Sep 2023 02:39:47 GMT  
		Size: 113.7 MB (113727900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86765eaed4922054440ad8df162f88c7bb68e20fe40dc037bf19ac523b0f1c`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:0d6f649407ee9b40f24f9a8bbac431843e22863a123b153ca8afa7964c9b4bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:6e37d19ba7a73cc342791e067ad974cfc70347a321f616a19b3ec8c971ffbe16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (177040226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa8920bdd5ea7b71a112b5142807009cdab7c52af6d9d21f67b12bb90278874`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:32 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:06:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:35 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:35 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:06:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:06:42 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:06:42 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:06:42 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:06:42 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:06:42 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:06:42 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491d5be99740a01bcf6d3effb2b65d751b17d2ce36f155ba6e3c0521ede5e1d`  
		Last Modified: Mon, 07 Aug 2023 20:07:39 GMT  
		Size: 57.5 MB (57513412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30944d8a02f5aa5b2df9f55d0e0e82cfbd301c2057b67968bdd9e6278834bdb3`  
		Last Modified: Mon, 07 Aug 2023 20:07:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b00d5cad62077e567e605de19de03ce072b5efcf28764a5b999dfc683edd1d9`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a201e4e46d2a7ee3d82944df44fbf4e83d69c84681f4b24420fb2d30618160`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd73cf062c66955f65d4d88518b2a9cc3ba90796d1b207b072790673baf6c75`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d182af21cdc26f2b23380091129b2e067e23a9ca9b9bfb47f1391db7df30931`  
		Last Modified: Mon, 07 Aug 2023 20:07:38 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c246e558fc4337d3476fd12619e376e64fbcb7767ca1e4f6a3bc04aa0aeb84b6`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:6768275ab183968bc57c60d1210dbd69047ea3151b2c74b0538c2d977a50801a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176262304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77da72567897e840c32222400f0c37efe6d8f91b53cdd65829232793d4df59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:11 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:19:12 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:13 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:19:13 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:14 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:20 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:21 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:21 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:21 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:21 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:21 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6299790359d70e22ca5255c4872a38bd76e660ac1965ec8839f329be49d6e0`  
		Last Modified: Mon, 07 Aug 2023 20:20:16 GMT  
		Size: 56.8 MB (56840636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde2f410764c8dd4d5aa4a1e1caaff936f4898b469567d3dce09cc2300c5fde9`  
		Last Modified: Mon, 07 Aug 2023 20:20:10 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a183615725bfd5df3507cc028f03a5d86895505fc81290d7fb5f25bdcd4a1c42`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4165241bb0894ac4336af593255778a69aad074d322b204628ed70d99670e49a`  
		Last Modified: Mon, 07 Aug 2023 20:20:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199352acfce239654f25a59c26d9d05f3a93e427bbf47f698e39aacbc25217f2`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878b92dc2b304cf31e868ad0c75f587f5e24a694694d1514ce7b6c81928e6fb`  
		Last Modified: Mon, 07 Aug 2023 20:20:15 GMT  
		Size: 116.7 MB (116690782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d442b6da1ed8b4b083b9748e14406f2f2c13c101acf077c2d11f07881dc6978`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:1d5b0c9579dad3f66b7d124ce485847e1a2254ed409e507512406f07b55f895f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172856836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf46b64638d0900b2bbf92002ef0548c4c9c55a7bc36c6cba38c15677c946fe2`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:00:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:00:55 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 21:00:59 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:01:01 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:01:04 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 21:01:06 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 21:01:06 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:09 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:01:10 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 21:01:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:01:27 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:01:27 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:01:28 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:01:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:01:30 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:01:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:01:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:01:34 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:01:35 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:01:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:01:36 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:01:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:01:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe564fb084b8a137bdb596c1b68b8890678cdac546872bf82d294938eb3057`  
		Last Modified: Mon, 07 Aug 2023 21:04:27 GMT  
		Size: 53.3 MB (53343673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83921fa265cc0f40ea202268c6acb0eff121e5dc980a79df9985247720c770ed`  
		Last Modified: Mon, 07 Aug 2023 21:04:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21a83293f73c86467ff15f689ee8e4ce09d1c66a4c582eba1ee5cb8f7299140`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab32330ed110ba514fb91cd76b73cc1efc3877a2fa29184d20693c4154236c1a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ca03c355c306ff1792fa6e7de3965c4ba98c28ba98c7d5e12dc86a618229a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 3.0 KB (3035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d77c5027597e89c08f48e2afd57b1ca00aa142c5bd4390158f609879841fda`  
		Last Modified: Mon, 07 Aug 2023 21:04:23 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798423f69137bef5850ea909ff5c3665124e306aa787d5278d2bd1a01f25438`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:0d6f649407ee9b40f24f9a8bbac431843e22863a123b153ca8afa7964c9b4bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:6e37d19ba7a73cc342791e067ad974cfc70347a321f616a19b3ec8c971ffbe16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (177040226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa8920bdd5ea7b71a112b5142807009cdab7c52af6d9d21f67b12bb90278874`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:32 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:06:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:35 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:35 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:06:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:06:42 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:06:42 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:06:42 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:06:42 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:06:42 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:06:42 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491d5be99740a01bcf6d3effb2b65d751b17d2ce36f155ba6e3c0521ede5e1d`  
		Last Modified: Mon, 07 Aug 2023 20:07:39 GMT  
		Size: 57.5 MB (57513412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30944d8a02f5aa5b2df9f55d0e0e82cfbd301c2057b67968bdd9e6278834bdb3`  
		Last Modified: Mon, 07 Aug 2023 20:07:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b00d5cad62077e567e605de19de03ce072b5efcf28764a5b999dfc683edd1d9`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a201e4e46d2a7ee3d82944df44fbf4e83d69c84681f4b24420fb2d30618160`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd73cf062c66955f65d4d88518b2a9cc3ba90796d1b207b072790673baf6c75`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d182af21cdc26f2b23380091129b2e067e23a9ca9b9bfb47f1391db7df30931`  
		Last Modified: Mon, 07 Aug 2023 20:07:38 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c246e558fc4337d3476fd12619e376e64fbcb7767ca1e4f6a3bc04aa0aeb84b6`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:6768275ab183968bc57c60d1210dbd69047ea3151b2c74b0538c2d977a50801a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176262304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77da72567897e840c32222400f0c37efe6d8f91b53cdd65829232793d4df59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:11 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:19:12 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:13 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:19:13 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:14 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:20 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:21 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:21 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:21 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:21 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:21 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6299790359d70e22ca5255c4872a38bd76e660ac1965ec8839f329be49d6e0`  
		Last Modified: Mon, 07 Aug 2023 20:20:16 GMT  
		Size: 56.8 MB (56840636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde2f410764c8dd4d5aa4a1e1caaff936f4898b469567d3dce09cc2300c5fde9`  
		Last Modified: Mon, 07 Aug 2023 20:20:10 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a183615725bfd5df3507cc028f03a5d86895505fc81290d7fb5f25bdcd4a1c42`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4165241bb0894ac4336af593255778a69aad074d322b204628ed70d99670e49a`  
		Last Modified: Mon, 07 Aug 2023 20:20:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199352acfce239654f25a59c26d9d05f3a93e427bbf47f698e39aacbc25217f2`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878b92dc2b304cf31e868ad0c75f587f5e24a694694d1514ce7b6c81928e6fb`  
		Last Modified: Mon, 07 Aug 2023 20:20:15 GMT  
		Size: 116.7 MB (116690782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d442b6da1ed8b4b083b9748e14406f2f2c13c101acf077c2d11f07881dc6978`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1d5b0c9579dad3f66b7d124ce485847e1a2254ed409e507512406f07b55f895f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172856836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf46b64638d0900b2bbf92002ef0548c4c9c55a7bc36c6cba38c15677c946fe2`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:00:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:00:55 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 21:00:59 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:01:01 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:01:04 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 21:01:06 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 21:01:06 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:09 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:01:10 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 21:01:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:01:27 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:01:27 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:01:28 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:01:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:01:30 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:01:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:01:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:01:34 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:01:35 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:01:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:01:36 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:01:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:01:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe564fb084b8a137bdb596c1b68b8890678cdac546872bf82d294938eb3057`  
		Last Modified: Mon, 07 Aug 2023 21:04:27 GMT  
		Size: 53.3 MB (53343673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83921fa265cc0f40ea202268c6acb0eff121e5dc980a79df9985247720c770ed`  
		Last Modified: Mon, 07 Aug 2023 21:04:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21a83293f73c86467ff15f689ee8e4ce09d1c66a4c582eba1ee5cb8f7299140`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab32330ed110ba514fb91cd76b73cc1efc3877a2fa29184d20693c4154236c1a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ca03c355c306ff1792fa6e7de3965c4ba98c28ba98c7d5e12dc86a618229a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 3.0 KB (3035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d77c5027597e89c08f48e2afd57b1ca00aa142c5bd4390158f609879841fda`  
		Last Modified: Mon, 07 Aug 2023 21:04:23 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798423f69137bef5850ea909ff5c3665124e306aa787d5278d2bd1a01f25438`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:ce3955d69f0b929db8c250e08929e906516ab3a7e7c5f36f8c7e0dda070c55e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2` - linux; amd64

```console
$ docker pull bonita@sha256:f1fbe76950249c5337b55456fc18828247e4a3692974573200a791465a73ef74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b7611f8a0d2511c02c992106aae05a369cd0bff59d23996d7a7558ac1ad75e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:06:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:59 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:00 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:00 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:00 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f54b3848aa87b54f37b2617641a73c10f3216e0fd40148ed17133629e3049`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c71bc0606a895255d2eb2c361edcc8a23c8108927ff33ee46595e7c8d5f6ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a5f962946fe88df7bd30bb6c59e5e4c0986f279dd0919f181b549ac4918309`  
		Last Modified: Mon, 07 Aug 2023 20:08:02 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb216d93fdd6e9836d94e5386c614c769d8e9f57264691f41052669dcc92ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e57219ac1417379d5585406bd938c05e051cd9ae1166b38507c56e1e0457c164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182727752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4afdbd8f51abd988fbcf83c66924ed89d1b4ddbb900c4f66f7aaf6dc3fadb89`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:19:30 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:31 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:31 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:39 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174d3ec451ae1e32a30c269130a1218cdbb11e6a864747d61a3a52a56806a77`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40c3379221adff40aef931c8d365089db87f2f45f8d0d0111922f4a13ddd3e6`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b405b04cb2b38e739e5e0121716cb3d2da0c624fcc3b50eab483a08b181fad8`  
		Last Modified: Mon, 07 Aug 2023 20:20:38 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda41b68ecdc2c2773ec69bf2348cacc451459ec7d4c503314b17c596a1bceb`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:f5a933c88fdf02b581885836758b76cada3a4493a67ac9798d37db2e2d58fc55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179748862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4428669dd49dc614e811672b9ec19c5a4d218916cc0e4df36523ede15bfc02a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 21:02:12 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:02:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:15 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:02:16 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:02:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:02:32 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:02:33 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:02:34 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:02:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:02:39 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:02:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:02:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:02:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:02:44 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:02:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:02:46 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:02:46 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:02:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04243d83b1b02f7bc4fd9e6b0cbc675f11b14dbdbb7834577d916797351f5f`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333e5557ff1ac5c9d56f0d8515beb1f0d32804d48d6ef2cf6c1c27212226d057`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3078da64cb0ef825f9ac8dee1aac789092494816150c5004496220679590742`  
		Last Modified: Mon, 07 Aug 2023 21:05:01 GMT  
		Size: 119.2 MB (119192982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eb3d4f22b8bb78ac888e934545fb42cae178f993793cdcf14323f38d82a8c9`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:ce3955d69f0b929db8c250e08929e906516ab3a7e7c5f36f8c7e0dda070c55e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:f1fbe76950249c5337b55456fc18828247e4a3692974573200a791465a73ef74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b7611f8a0d2511c02c992106aae05a369cd0bff59d23996d7a7558ac1ad75e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:06:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:59 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:00 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:00 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:00 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f54b3848aa87b54f37b2617641a73c10f3216e0fd40148ed17133629e3049`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c71bc0606a895255d2eb2c361edcc8a23c8108927ff33ee46595e7c8d5f6ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a5f962946fe88df7bd30bb6c59e5e4c0986f279dd0919f181b549ac4918309`  
		Last Modified: Mon, 07 Aug 2023 20:08:02 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb216d93fdd6e9836d94e5386c614c769d8e9f57264691f41052669dcc92ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e57219ac1417379d5585406bd938c05e051cd9ae1166b38507c56e1e0457c164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182727752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4afdbd8f51abd988fbcf83c66924ed89d1b4ddbb900c4f66f7aaf6dc3fadb89`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:19:30 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:31 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:31 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:39 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174d3ec451ae1e32a30c269130a1218cdbb11e6a864747d61a3a52a56806a77`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40c3379221adff40aef931c8d365089db87f2f45f8d0d0111922f4a13ddd3e6`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b405b04cb2b38e739e5e0121716cb3d2da0c624fcc3b50eab483a08b181fad8`  
		Last Modified: Mon, 07 Aug 2023 20:20:38 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda41b68ecdc2c2773ec69bf2348cacc451459ec7d4c503314b17c596a1bceb`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:f5a933c88fdf02b581885836758b76cada3a4493a67ac9798d37db2e2d58fc55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179748862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4428669dd49dc614e811672b9ec19c5a4d218916cc0e4df36523ede15bfc02a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 21:02:12 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:02:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:15 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:02:16 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:02:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:02:32 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:02:33 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:02:34 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:02:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:02:39 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:02:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:02:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:02:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:02:44 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:02:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:02:46 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:02:46 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:02:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04243d83b1b02f7bc4fd9e6b0cbc675f11b14dbdbb7834577d916797351f5f`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333e5557ff1ac5c9d56f0d8515beb1f0d32804d48d6ef2cf6c1c27212226d057`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3078da64cb0ef825f9ac8dee1aac789092494816150c5004496220679590742`  
		Last Modified: Mon, 07 Aug 2023 21:05:01 GMT  
		Size: 119.2 MB (119192982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eb3d4f22b8bb78ac888e934545fb42cae178f993793cdcf14323f38d82a8c9`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1`

```console
$ docker pull bonita@sha256:d4d00069b4011987600893478398014bd45712ef4ba803efc52ca139572bbbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2023.1` - linux; amd64

```console
$ docker pull bonita@sha256:0cec6e4c2cf0db75e2f8fbd10b65bd66d338483915505bb5732b8c7fac8b53ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182573608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:661e975084498f43ab55e0e7942291cd493ba0fcfc7a4b734658b3404291fd28`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:07:03 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:04 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:07:04 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:07:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:07:11 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:12 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:12 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:12 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f09bfbc4303e7ca9221650d6108ef24c989fe3234712ceb4cc438aafed6631`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b4856b17cf945155623a8ba6fa0fc4d34d716bff12a76aa69a0aa9fc800647`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f03e393c6062c5f5230b28ad2b86b79c2bca72b74a37c319143daaecf3e17`  
		Last Modified: Mon, 07 Aug 2023 20:08:52 GMT  
		Size: 118.2 MB (118180289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b30e288dc8d22588e6e14b31cf608e4165dd5cc5ed02a6ba74f05b705e9f`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7bdb78322790eaed16dfe674441022acda2f1a3449b7e9dbfa88c00d3a27b60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181715072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca4844028b13e1e0f43430ee74c0956374cd15a9b96022cc698f3039f92669`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:42 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:48 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:49 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:49 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:49 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cddfa8ba0254f1108ae328eae229c7adc124e1d77558c9fb4d7d89b6b91f38`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60b6d238d22066f45902030974fce87391e836e1df2906dd6ae97a4b596c882`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c10aea7994a00039782ab1d341b65ebe73b39575affb94b42bbe6e4506316`  
		Last Modified: Mon, 07 Aug 2023 20:21:02 GMT  
		Size: 118.2 MB (118180315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576020c9a944e2b24ebca2b851d9be7a8ffe41364d07e2b018bfece41d50793`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:38edd994ce8e3a3dd37e72ad2964b3b48b320e1a7ba43a9c3ab3c48a09146fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178736193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6edf34148d1e29255cc39b92fe59f1e14f5142c1d45a81aa688f91990b752b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:56 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 21:02:58 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:02:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:03:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:03:03 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:03:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:03:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:03:21 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:03:22 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:03:23 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:03:25 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:03:26 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:03:28 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:03:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:03:30 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:03:34 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:03:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:03:36 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:03:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:03:37 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:03:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:03:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbf00b32a5ffbc82c2e22e3eae113f97e07a98a6f28a66ee8cc7426c086340e`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d2b99ce483dbb61d5638c55230f5081c6b912fd021846ce90f998fe4b00bf`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 3.0 KB (3047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04193e5ce6c7bfb73f99854d069a17eec4ca0ab8bd967de019f89c2fd0363e`  
		Last Modified: Mon, 07 Aug 2023 21:05:43 GMT  
		Size: 118.2 MB (118180324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7d34d1c6a44476bc5350e7b944a27644c90115e582a0d889f6b12c3ff2393`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2023.1-u0`

```console
$ docker pull bonita@sha256:d4d00069b4011987600893478398014bd45712ef4ba803efc52ca139572bbbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2023.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:0cec6e4c2cf0db75e2f8fbd10b65bd66d338483915505bb5732b8c7fac8b53ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182573608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:661e975084498f43ab55e0e7942291cd493ba0fcfc7a4b734658b3404291fd28`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:07:03 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:04 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:07:04 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:07:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:07:11 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:12 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:12 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:12 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f09bfbc4303e7ca9221650d6108ef24c989fe3234712ceb4cc438aafed6631`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b4856b17cf945155623a8ba6fa0fc4d34d716bff12a76aa69a0aa9fc800647`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f03e393c6062c5f5230b28ad2b86b79c2bca72b74a37c319143daaecf3e17`  
		Last Modified: Mon, 07 Aug 2023 20:08:52 GMT  
		Size: 118.2 MB (118180289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b30e288dc8d22588e6e14b31cf608e4165dd5cc5ed02a6ba74f05b705e9f`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7bdb78322790eaed16dfe674441022acda2f1a3449b7e9dbfa88c00d3a27b60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181715072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca4844028b13e1e0f43430ee74c0956374cd15a9b96022cc698f3039f92669`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:42 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:48 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:49 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:49 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:49 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cddfa8ba0254f1108ae328eae229c7adc124e1d77558c9fb4d7d89b6b91f38`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60b6d238d22066f45902030974fce87391e836e1df2906dd6ae97a4b596c882`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c10aea7994a00039782ab1d341b65ebe73b39575affb94b42bbe6e4506316`  
		Last Modified: Mon, 07 Aug 2023 20:21:02 GMT  
		Size: 118.2 MB (118180315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576020c9a944e2b24ebca2b851d9be7a8ffe41364d07e2b018bfece41d50793`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2023.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:38edd994ce8e3a3dd37e72ad2964b3b48b320e1a7ba43a9c3ab3c48a09146fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178736193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6edf34148d1e29255cc39b92fe59f1e14f5142c1d45a81aa688f91990b752b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:56 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 21:02:58 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:02:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:03:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:03:03 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:03:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:03:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:03:21 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:03:22 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:03:23 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:03:25 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:03:26 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:03:28 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:03:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:03:30 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:03:34 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:03:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:03:36 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:03:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:03:37 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:03:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:03:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbf00b32a5ffbc82c2e22e3eae113f97e07a98a6f28a66ee8cc7426c086340e`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d2b99ce483dbb61d5638c55230f5081c6b912fd021846ce90f998fe4b00bf`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 3.0 KB (3047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04193e5ce6c7bfb73f99854d069a17eec4ca0ab8bd967de019f89c2fd0363e`  
		Last Modified: Mon, 07 Aug 2023 21:05:43 GMT  
		Size: 118.2 MB (118180324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7d34d1c6a44476bc5350e7b944a27644c90115e582a0d889f6b12c3ff2393`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:ce650e5acc90966d76ebb0c0968f5d2fe9d1b62d69cae93bdd808bce9f52f6b9
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
$ docker pull bonita@sha256:ee1f85da1a0601a58c08f5b38954b807e58e77f1c15f856c6e65c6d7069d9f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232986008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f8cedb264ee64d6eea033731ad0d9e827931e355389b1670d4603868da35a`
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
# Sat, 16 Sep 2023 02:35:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 16 Sep 2023 02:38:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:38:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 16 Sep 2023 02:38:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 16 Sep 2023 02:38:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BONITA_VERSION
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BRANDING_VERSION
# Sat, 16 Sep 2023 02:38:36 GMT
ARG BONITA_SHA256
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BASE_URL
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BONITA_URL
# Sat, 16 Sep 2023 02:38:38 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 16 Sep 2023 02:38:40 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 16 Sep 2023 02:38:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:42 GMT
RUN mkdir /opt/files
# Sat, 16 Sep 2023 02:38:42 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 16 Sep 2023 02:38:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 16 Sep 2023 02:38:57 GMT
ENV HTTP_API=false
# Sat, 16 Sep 2023 02:39:00 GMT
VOLUME [/opt/bonita]
# Sat, 16 Sep 2023 02:39:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 16 Sep 2023 02:39:03 GMT
EXPOSE 8080
# Sat, 16 Sep 2023 02:39:06 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ceefc23d77069ec288df034168091e2b853c1486fed391d1dae80c8dd41319`  
		Last Modified: Sat, 16 Sep 2023 02:39:59 GMT  
		Size: 88.0 MB (87975233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05285767062ecf2a4dbeac7e3b295a6f16b85aaed73b43d053de02361fd4ee9`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85527ce4335f69446508c3a5ec215a176f774bb26f0e289f01f869b03a3f000`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b04b643d05b9d28651f17e0200b452ec28cb6c1a34562fb14ea01d4bf6563e`  
		Last Modified: Sat, 16 Sep 2023 02:39:38 GMT  
		Size: 831.6 KB (831580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58368109f9a398b225bcf828cfe5e4e1872efadae44c7f24b8ea71a490296db6`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba19de21f79dddd4b1496ced7970f008404bb0a6a0207e5d46a86964b546b2f`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65d3fdfff12c9f01cbb893d222cf4ffa59d774f4d34d06769fd273dcfb5d25d`  
		Last Modified: Sat, 16 Sep 2023 02:39:47 GMT  
		Size: 113.7 MB (113727900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86765eaed4922054440ad8df162f88c7bb68e20fe40dc037bf19ac523b0f1c`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:ce650e5acc90966d76ebb0c0968f5d2fe9d1b62d69cae93bdd808bce9f52f6b9
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
$ docker pull bonita@sha256:ee1f85da1a0601a58c08f5b38954b807e58e77f1c15f856c6e65c6d7069d9f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232986008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f8cedb264ee64d6eea033731ad0d9e827931e355389b1670d4603868da35a`
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
# Sat, 16 Sep 2023 02:35:53 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 16 Sep 2023 02:38:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:38:26 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 16 Sep 2023 02:38:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 16 Sep 2023 02:38:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BONITA_VERSION
# Sat, 16 Sep 2023 02:38:35 GMT
ARG BRANDING_VERSION
# Sat, 16 Sep 2023 02:38:36 GMT
ARG BONITA_SHA256
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BASE_URL
# Sat, 16 Sep 2023 02:38:37 GMT
ARG BONITA_URL
# Sat, 16 Sep 2023 02:38:38 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 16 Sep 2023 02:38:39 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 16 Sep 2023 02:38:40 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 16 Sep 2023 02:38:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 16 Sep 2023 02:38:42 GMT
RUN mkdir /opt/files
# Sat, 16 Sep 2023 02:38:42 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 16 Sep 2023 02:38:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 16 Sep 2023 02:38:57 GMT
ENV HTTP_API=false
# Sat, 16 Sep 2023 02:39:00 GMT
VOLUME [/opt/bonita]
# Sat, 16 Sep 2023 02:39:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 16 Sep 2023 02:39:03 GMT
EXPOSE 8080
# Sat, 16 Sep 2023 02:39:06 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2be4fb4963c9ca350d079e0a4f8a6af6e5c340f41d8021b993e78df7f93ad064`  
		Last Modified: Fri, 02 Jun 2023 00:21:59 GMT  
		Size: 30.4 MB (30444090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ceefc23d77069ec288df034168091e2b853c1486fed391d1dae80c8dd41319`  
		Last Modified: Sat, 16 Sep 2023 02:39:59 GMT  
		Size: 88.0 MB (87975233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05285767062ecf2a4dbeac7e3b295a6f16b85aaed73b43d053de02361fd4ee9`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85527ce4335f69446508c3a5ec215a176f774bb26f0e289f01f869b03a3f000`  
		Last Modified: Sat, 16 Sep 2023 02:39:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b04b643d05b9d28651f17e0200b452ec28cb6c1a34562fb14ea01d4bf6563e`  
		Last Modified: Sat, 16 Sep 2023 02:39:38 GMT  
		Size: 831.6 KB (831580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58368109f9a398b225bcf828cfe5e4e1872efadae44c7f24b8ea71a490296db6`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba19de21f79dddd4b1496ced7970f008404bb0a6a0207e5d46a86964b546b2f`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65d3fdfff12c9f01cbb893d222cf4ffa59d774f4d34d06769fd273dcfb5d25d`  
		Last Modified: Sat, 16 Sep 2023 02:39:47 GMT  
		Size: 113.7 MB (113727900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86765eaed4922054440ad8df162f88c7bb68e20fe40dc037bf19ac523b0f1c`  
		Last Modified: Sat, 16 Sep 2023 02:39:37 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:0d6f649407ee9b40f24f9a8bbac431843e22863a123b153ca8afa7964c9b4bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:6e37d19ba7a73cc342791e067ad974cfc70347a321f616a19b3ec8c971ffbe16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (177040226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa8920bdd5ea7b71a112b5142807009cdab7c52af6d9d21f67b12bb90278874`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:32 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:06:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:35 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:35 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:06:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:06:42 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:06:42 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:06:42 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:06:42 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:06:42 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:06:42 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491d5be99740a01bcf6d3effb2b65d751b17d2ce36f155ba6e3c0521ede5e1d`  
		Last Modified: Mon, 07 Aug 2023 20:07:39 GMT  
		Size: 57.5 MB (57513412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30944d8a02f5aa5b2df9f55d0e0e82cfbd301c2057b67968bdd9e6278834bdb3`  
		Last Modified: Mon, 07 Aug 2023 20:07:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b00d5cad62077e567e605de19de03ce072b5efcf28764a5b999dfc683edd1d9`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a201e4e46d2a7ee3d82944df44fbf4e83d69c84681f4b24420fb2d30618160`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd73cf062c66955f65d4d88518b2a9cc3ba90796d1b207b072790673baf6c75`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d182af21cdc26f2b23380091129b2e067e23a9ca9b9bfb47f1391db7df30931`  
		Last Modified: Mon, 07 Aug 2023 20:07:38 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c246e558fc4337d3476fd12619e376e64fbcb7767ca1e4f6a3bc04aa0aeb84b6`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:6768275ab183968bc57c60d1210dbd69047ea3151b2c74b0538c2d977a50801a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176262304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77da72567897e840c32222400f0c37efe6d8f91b53cdd65829232793d4df59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:11 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:19:12 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:13 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:19:13 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:14 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:20 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:21 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:21 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:21 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:21 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:21 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6299790359d70e22ca5255c4872a38bd76e660ac1965ec8839f329be49d6e0`  
		Last Modified: Mon, 07 Aug 2023 20:20:16 GMT  
		Size: 56.8 MB (56840636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde2f410764c8dd4d5aa4a1e1caaff936f4898b469567d3dce09cc2300c5fde9`  
		Last Modified: Mon, 07 Aug 2023 20:20:10 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a183615725bfd5df3507cc028f03a5d86895505fc81290d7fb5f25bdcd4a1c42`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4165241bb0894ac4336af593255778a69aad074d322b204628ed70d99670e49a`  
		Last Modified: Mon, 07 Aug 2023 20:20:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199352acfce239654f25a59c26d9d05f3a93e427bbf47f698e39aacbc25217f2`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878b92dc2b304cf31e868ad0c75f587f5e24a694694d1514ce7b6c81928e6fb`  
		Last Modified: Mon, 07 Aug 2023 20:20:15 GMT  
		Size: 116.7 MB (116690782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d442b6da1ed8b4b083b9748e14406f2f2c13c101acf077c2d11f07881dc6978`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:1d5b0c9579dad3f66b7d124ce485847e1a2254ed409e507512406f07b55f895f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172856836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf46b64638d0900b2bbf92002ef0548c4c9c55a7bc36c6cba38c15677c946fe2`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:00:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:00:55 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 21:00:59 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:01:01 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:01:04 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 21:01:06 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 21:01:06 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:09 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:01:10 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 21:01:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:01:27 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:01:27 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:01:28 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:01:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:01:30 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:01:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:01:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:01:34 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:01:35 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:01:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:01:36 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:01:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:01:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe564fb084b8a137bdb596c1b68b8890678cdac546872bf82d294938eb3057`  
		Last Modified: Mon, 07 Aug 2023 21:04:27 GMT  
		Size: 53.3 MB (53343673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83921fa265cc0f40ea202268c6acb0eff121e5dc980a79df9985247720c770ed`  
		Last Modified: Mon, 07 Aug 2023 21:04:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21a83293f73c86467ff15f689ee8e4ce09d1c66a4c582eba1ee5cb8f7299140`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab32330ed110ba514fb91cd76b73cc1efc3877a2fa29184d20693c4154236c1a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ca03c355c306ff1792fa6e7de3965c4ba98c28ba98c7d5e12dc86a618229a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 3.0 KB (3035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d77c5027597e89c08f48e2afd57b1ca00aa142c5bd4390158f609879841fda`  
		Last Modified: Mon, 07 Aug 2023 21:04:23 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798423f69137bef5850ea909ff5c3665124e306aa787d5278d2bd1a01f25438`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:0d6f649407ee9b40f24f9a8bbac431843e22863a123b153ca8afa7964c9b4bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:6e37d19ba7a73cc342791e067ad974cfc70347a321f616a19b3ec8c971ffbe16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (177040226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa8920bdd5ea7b71a112b5142807009cdab7c52af6d9d21f67b12bb90278874`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:32 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:33 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:33 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:06:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:34 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:06:35 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:35 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:06:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:41 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:41 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:06:41 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:06:42 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:06:42 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:06:42 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:06:42 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:06:42 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:06:42 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6491d5be99740a01bcf6d3effb2b65d751b17d2ce36f155ba6e3c0521ede5e1d`  
		Last Modified: Mon, 07 Aug 2023 20:07:39 GMT  
		Size: 57.5 MB (57513412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30944d8a02f5aa5b2df9f55d0e0e82cfbd301c2057b67968bdd9e6278834bdb3`  
		Last Modified: Mon, 07 Aug 2023 20:07:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b00d5cad62077e567e605de19de03ce072b5efcf28764a5b999dfc683edd1d9`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a201e4e46d2a7ee3d82944df44fbf4e83d69c84681f4b24420fb2d30618160`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd73cf062c66955f65d4d88518b2a9cc3ba90796d1b207b072790673baf6c75`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d182af21cdc26f2b23380091129b2e067e23a9ca9b9bfb47f1391db7df30931`  
		Last Modified: Mon, 07 Aug 2023 20:07:38 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c246e558fc4337d3476fd12619e376e64fbcb7767ca1e4f6a3bc04aa0aeb84b6`  
		Last Modified: Mon, 07 Aug 2023 20:07:30 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:6768275ab183968bc57c60d1210dbd69047ea3151b2c74b0538c2d977a50801a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176262304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77da72567897e840c32222400f0c37efe6d8f91b53cdd65829232793d4df59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:11 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 20:19:12 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:13 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 20:19:13 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 20:19:13 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 20:19:14 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:14 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 20:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:20 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:20 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:21 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:21 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:21 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:21 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:21 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:21 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6299790359d70e22ca5255c4872a38bd76e660ac1965ec8839f329be49d6e0`  
		Last Modified: Mon, 07 Aug 2023 20:20:16 GMT  
		Size: 56.8 MB (56840636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde2f410764c8dd4d5aa4a1e1caaff936f4898b469567d3dce09cc2300c5fde9`  
		Last Modified: Mon, 07 Aug 2023 20:20:10 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a183615725bfd5df3507cc028f03a5d86895505fc81290d7fb5f25bdcd4a1c42`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4165241bb0894ac4336af593255778a69aad074d322b204628ed70d99670e49a`  
		Last Modified: Mon, 07 Aug 2023 20:20:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199352acfce239654f25a59c26d9d05f3a93e427bbf47f698e39aacbc25217f2`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878b92dc2b304cf31e868ad0c75f587f5e24a694694d1514ce7b6c81928e6fb`  
		Last Modified: Mon, 07 Aug 2023 20:20:15 GMT  
		Size: 116.7 MB (116690782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d442b6da1ed8b4b083b9748e14406f2f2c13c101acf077c2d11f07881dc6978`  
		Last Modified: Mon, 07 Aug 2023 20:20:08 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1d5b0c9579dad3f66b7d124ce485847e1a2254ed409e507512406f07b55f895f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172856836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf46b64638d0900b2bbf92002ef0548c4c9c55a7bc36c6cba38c15677c946fe2`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:00:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:00:55 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Mon, 07 Aug 2023 21:00:59 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:01:01 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:01:02 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:01:03 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:01:04 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BONITA_VERSION=7.14.0
# Mon, 07 Aug 2023 21:01:05 GMT
ENV BRANDING_VERSION=2022.1-u0
# Mon, 07 Aug 2023 21:01:06 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Mon, 07 Aug 2023 21:01:06 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:01:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Mon, 07 Aug 2023 21:01:09 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:01:10 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Mon, 07 Aug 2023 21:01:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:01:26 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:01:27 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:01:27 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:01:28 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:01:29 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:01:30 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:01:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:01:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:01:33 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:01:34 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:01:35 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:01:35 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:01:36 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:01:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:01:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe564fb084b8a137bdb596c1b68b8890678cdac546872bf82d294938eb3057`  
		Last Modified: Mon, 07 Aug 2023 21:04:27 GMT  
		Size: 53.3 MB (53343673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83921fa265cc0f40ea202268c6acb0eff121e5dc980a79df9985247720c770ed`  
		Last Modified: Mon, 07 Aug 2023 21:04:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21a83293f73c86467ff15f689ee8e4ce09d1c66a4c582eba1ee5cb8f7299140`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab32330ed110ba514fb91cd76b73cc1efc3877a2fa29184d20693c4154236c1a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ca03c355c306ff1792fa6e7de3965c4ba98c28ba98c7d5e12dc86a618229a`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 3.0 KB (3035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d77c5027597e89c08f48e2afd57b1ca00aa142c5bd4390158f609879841fda`  
		Last Modified: Mon, 07 Aug 2023 21:04:23 GMT  
		Size: 116.7 MB (116690784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798423f69137bef5850ea909ff5c3665124e306aa787d5278d2bd1a01f25438`  
		Last Modified: Mon, 07 Aug 2023 21:04:13 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:ce3955d69f0b929db8c250e08929e906516ab3a7e7c5f36f8c7e0dda070c55e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15` - linux; amd64

```console
$ docker pull bonita@sha256:f1fbe76950249c5337b55456fc18828247e4a3692974573200a791465a73ef74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b7611f8a0d2511c02c992106aae05a369cd0bff59d23996d7a7558ac1ad75e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:06:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:59 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:00 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:00 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:00 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f54b3848aa87b54f37b2617641a73c10f3216e0fd40148ed17133629e3049`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c71bc0606a895255d2eb2c361edcc8a23c8108927ff33ee46595e7c8d5f6ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a5f962946fe88df7bd30bb6c59e5e4c0986f279dd0919f181b549ac4918309`  
		Last Modified: Mon, 07 Aug 2023 20:08:02 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb216d93fdd6e9836d94e5386c614c769d8e9f57264691f41052669dcc92ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e57219ac1417379d5585406bd938c05e051cd9ae1166b38507c56e1e0457c164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182727752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4afdbd8f51abd988fbcf83c66924ed89d1b4ddbb900c4f66f7aaf6dc3fadb89`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:19:30 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:31 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:31 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:39 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174d3ec451ae1e32a30c269130a1218cdbb11e6a864747d61a3a52a56806a77`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40c3379221adff40aef931c8d365089db87f2f45f8d0d0111922f4a13ddd3e6`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b405b04cb2b38e739e5e0121716cb3d2da0c624fcc3b50eab483a08b181fad8`  
		Last Modified: Mon, 07 Aug 2023 20:20:38 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda41b68ecdc2c2773ec69bf2348cacc451459ec7d4c503314b17c596a1bceb`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:f5a933c88fdf02b581885836758b76cada3a4493a67ac9798d37db2e2d58fc55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179748862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4428669dd49dc614e811672b9ec19c5a4d218916cc0e4df36523ede15bfc02a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 21:02:12 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:02:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:15 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:02:16 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:02:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:02:32 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:02:33 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:02:34 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:02:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:02:39 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:02:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:02:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:02:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:02:44 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:02:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:02:46 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:02:46 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:02:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04243d83b1b02f7bc4fd9e6b0cbc675f11b14dbdbb7834577d916797351f5f`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333e5557ff1ac5c9d56f0d8515beb1f0d32804d48d6ef2cf6c1c27212226d057`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3078da64cb0ef825f9ac8dee1aac789092494816150c5004496220679590742`  
		Last Modified: Mon, 07 Aug 2023 21:05:01 GMT  
		Size: 119.2 MB (119192982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eb3d4f22b8bb78ac888e934545fb42cae178f993793cdcf14323f38d82a8c9`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:ce3955d69f0b929db8c250e08929e906516ab3a7e7c5f36f8c7e0dda070c55e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15.0` - linux; amd64

```console
$ docker pull bonita@sha256:f1fbe76950249c5337b55456fc18828247e4a3692974573200a791465a73ef74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b7611f8a0d2511c02c992106aae05a369cd0bff59d23996d7a7558ac1ad75e`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:06:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:06:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:06:52 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:06:52 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:06:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:06:59 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:06:59 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:06:59 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:06:59 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:00 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:00 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:00 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:00 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:00 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:00 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f54b3848aa87b54f37b2617641a73c10f3216e0fd40148ed17133629e3049`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c71bc0606a895255d2eb2c361edcc8a23c8108927ff33ee46595e7c8d5f6ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a5f962946fe88df7bd30bb6c59e5e4c0986f279dd0919f181b549ac4918309`  
		Last Modified: Mon, 07 Aug 2023 20:08:02 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb216d93fdd6e9836d94e5386c614c769d8e9f57264691f41052669dcc92ab`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e57219ac1417379d5585406bd938c05e051cd9ae1166b38507c56e1e0457c164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182727752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4afdbd8f51abd988fbcf83c66924ed89d1b4ddbb900c4f66f7aaf6dc3fadb89`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 20:19:30 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 20:19:31 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:31 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:38 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:38 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:38 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:39 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:39 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:39 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:39 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174d3ec451ae1e32a30c269130a1218cdbb11e6a864747d61a3a52a56806a77`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40c3379221adff40aef931c8d365089db87f2f45f8d0d0111922f4a13ddd3e6`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b405b04cb2b38e739e5e0121716cb3d2da0c624fcc3b50eab483a08b181fad8`  
		Last Modified: Mon, 07 Aug 2023 20:20:38 GMT  
		Size: 119.2 MB (119192989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda41b68ecdc2c2773ec69bf2348cacc451459ec7d4c503314b17c596a1bceb`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:f5a933c88fdf02b581885836758b76cada3a4493a67ac9798d37db2e2d58fc55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179748862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4428669dd49dc614e811672b9ec19c5a4d218916cc0e4df36523ede15bfc02a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ENV BONITA_VERSION=7.15.0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BRANDING_VERSION=2022.2-u0
# Mon, 07 Aug 2023 21:02:12 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Mon, 07 Aug 2023 21:02:12 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:02:14 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Mon, 07 Aug 2023 21:02:15 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:02:16 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:02:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:02:32 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:02:33 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:02:34 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:02:35 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:02:38 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:02:39 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:02:40 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:02:41 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:02:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:02:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:02:44 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:02:45 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:02:46 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:02:46 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:02:47 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04243d83b1b02f7bc4fd9e6b0cbc675f11b14dbdbb7834577d916797351f5f`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333e5557ff1ac5c9d56f0d8515beb1f0d32804d48d6ef2cf6c1c27212226d057`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3078da64cb0ef825f9ac8dee1aac789092494816150c5004496220679590742`  
		Last Modified: Mon, 07 Aug 2023 21:05:01 GMT  
		Size: 119.2 MB (119192982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eb3d4f22b8bb78ac888e934545fb42cae178f993793cdcf14323f38d82a8c9`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 5.4 KB (5425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0`

```console
$ docker pull bonita@sha256:d4d00069b4011987600893478398014bd45712ef4ba803efc52ca139572bbbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:8.0` - linux; amd64

```console
$ docker pull bonita@sha256:0cec6e4c2cf0db75e2f8fbd10b65bd66d338483915505bb5732b8c7fac8b53ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182573608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:661e975084498f43ab55e0e7942291cd493ba0fcfc7a4b734658b3404291fd28`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:07:03 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:04 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:07:04 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:07:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:07:11 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:12 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:12 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:12 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f09bfbc4303e7ca9221650d6108ef24c989fe3234712ceb4cc438aafed6631`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b4856b17cf945155623a8ba6fa0fc4d34d716bff12a76aa69a0aa9fc800647`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f03e393c6062c5f5230b28ad2b86b79c2bca72b74a37c319143daaecf3e17`  
		Last Modified: Mon, 07 Aug 2023 20:08:52 GMT  
		Size: 118.2 MB (118180289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b30e288dc8d22588e6e14b31cf608e4165dd5cc5ed02a6ba74f05b705e9f`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7bdb78322790eaed16dfe674441022acda2f1a3449b7e9dbfa88c00d3a27b60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181715072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca4844028b13e1e0f43430ee74c0956374cd15a9b96022cc698f3039f92669`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:42 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:48 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:49 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:49 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:49 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cddfa8ba0254f1108ae328eae229c7adc124e1d77558c9fb4d7d89b6b91f38`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60b6d238d22066f45902030974fce87391e836e1df2906dd6ae97a4b596c882`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c10aea7994a00039782ab1d341b65ebe73b39575affb94b42bbe6e4506316`  
		Last Modified: Mon, 07 Aug 2023 20:21:02 GMT  
		Size: 118.2 MB (118180315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576020c9a944e2b24ebca2b851d9be7a8ffe41364d07e2b018bfece41d50793`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:38edd994ce8e3a3dd37e72ad2964b3b48b320e1a7ba43a9c3ab3c48a09146fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178736193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6edf34148d1e29255cc39b92fe59f1e14f5142c1d45a81aa688f91990b752b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:56 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 21:02:58 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:02:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:03:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:03:03 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:03:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:03:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:03:21 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:03:22 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:03:23 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:03:25 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:03:26 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:03:28 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:03:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:03:30 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:03:34 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:03:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:03:36 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:03:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:03:37 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:03:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:03:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbf00b32a5ffbc82c2e22e3eae113f97e07a98a6f28a66ee8cc7426c086340e`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d2b99ce483dbb61d5638c55230f5081c6b912fd021846ce90f998fe4b00bf`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 3.0 KB (3047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04193e5ce6c7bfb73f99854d069a17eec4ca0ab8bd967de019f89c2fd0363e`  
		Last Modified: Mon, 07 Aug 2023 21:05:43 GMT  
		Size: 118.2 MB (118180324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7d34d1c6a44476bc5350e7b944a27644c90115e582a0d889f6b12c3ff2393`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:8.0.0`

```console
$ docker pull bonita@sha256:d4d00069b4011987600893478398014bd45712ef4ba803efc52ca139572bbbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:8.0.0` - linux; amd64

```console
$ docker pull bonita@sha256:0cec6e4c2cf0db75e2f8fbd10b65bd66d338483915505bb5732b8c7fac8b53ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182573608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:661e975084498f43ab55e0e7942291cd493ba0fcfc7a4b734658b3404291fd28`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:07:03 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:04 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:07:04 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:07:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:07:11 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:12 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:12 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:12 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f09bfbc4303e7ca9221650d6108ef24c989fe3234712ceb4cc438aafed6631`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b4856b17cf945155623a8ba6fa0fc4d34d716bff12a76aa69a0aa9fc800647`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f03e393c6062c5f5230b28ad2b86b79c2bca72b74a37c319143daaecf3e17`  
		Last Modified: Mon, 07 Aug 2023 20:08:52 GMT  
		Size: 118.2 MB (118180289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b30e288dc8d22588e6e14b31cf608e4165dd5cc5ed02a6ba74f05b705e9f`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7bdb78322790eaed16dfe674441022acda2f1a3449b7e9dbfa88c00d3a27b60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181715072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca4844028b13e1e0f43430ee74c0956374cd15a9b96022cc698f3039f92669`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:42 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:48 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:49 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:49 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:49 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cddfa8ba0254f1108ae328eae229c7adc124e1d77558c9fb4d7d89b6b91f38`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60b6d238d22066f45902030974fce87391e836e1df2906dd6ae97a4b596c882`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c10aea7994a00039782ab1d341b65ebe73b39575affb94b42bbe6e4506316`  
		Last Modified: Mon, 07 Aug 2023 20:21:02 GMT  
		Size: 118.2 MB (118180315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576020c9a944e2b24ebca2b851d9be7a8ffe41364d07e2b018bfece41d50793`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:8.0.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:38edd994ce8e3a3dd37e72ad2964b3b48b320e1a7ba43a9c3ab3c48a09146fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178736193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6edf34148d1e29255cc39b92fe59f1e14f5142c1d45a81aa688f91990b752b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:56 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 21:02:58 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:02:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:03:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:03:03 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:03:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:03:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:03:21 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:03:22 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:03:23 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:03:25 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:03:26 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:03:28 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:03:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:03:30 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:03:34 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:03:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:03:36 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:03:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:03:37 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:03:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:03:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbf00b32a5ffbc82c2e22e3eae113f97e07a98a6f28a66ee8cc7426c086340e`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d2b99ce483dbb61d5638c55230f5081c6b912fd021846ce90f998fe4b00bf`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 3.0 KB (3047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04193e5ce6c7bfb73f99854d069a17eec4ca0ab8bd967de019f89c2fd0363e`  
		Last Modified: Mon, 07 Aug 2023 21:05:43 GMT  
		Size: 118.2 MB (118180324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7d34d1c6a44476bc5350e7b944a27644c90115e582a0d889f6b12c3ff2393`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:d4d00069b4011987600893478398014bd45712ef4ba803efc52ca139572bbbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:0cec6e4c2cf0db75e2f8fbd10b65bd66d338483915505bb5732b8c7fac8b53ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182573608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:661e975084498f43ab55e0e7942291cd493ba0fcfc7a4b734658b3404291fd28`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:06:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:06:49 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:06:50 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:06:51 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:06:51 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:07:03 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:07:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:07:04 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:07:04 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:07:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:07:10 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:07:11 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:07:11 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:07:11 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:07:11 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:07:12 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:07:12 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:07:12 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:07:12 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed80d93f75002d7425bc558a2d3dab12df173ef2d866c2bd4d62c1486b5caa`  
		Last Modified: Mon, 07 Aug 2023 20:08:09 GMT  
		Size: 61.6 MB (61575610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63659d2097230a4d818d5a8e1dea4e542f09a682c561ec678dceee5b74f514b4`  
		Last Modified: Mon, 07 Aug 2023 20:07:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80177c4ce23eb19289089ce6b4655b1d14a208ed0fcce46c940eb03d1871878`  
		Last Modified: Mon, 07 Aug 2023 20:07:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f09bfbc4303e7ca9221650d6108ef24c989fe3234712ceb4cc438aafed6631`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b4856b17cf945155623a8ba6fa0fc4d34d716bff12a76aa69a0aa9fc800647`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 3.0 KB (3045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f03e393c6062c5f5230b28ad2b86b79c2bca72b74a37c319143daaecf3e17`  
		Last Modified: Mon, 07 Aug 2023 20:08:52 GMT  
		Size: 118.2 MB (118180289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b30e288dc8d22588e6e14b31cf608e4165dd5cc5ed02a6ba74f05b705e9f`  
		Last Modified: Mon, 07 Aug 2023 20:08:42 GMT  
		Size: 5.4 KB (5420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7bdb78322790eaed16dfe674441022acda2f1a3449b7e9dbfa88c00d3a27b60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181715072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca4844028b13e1e0f43430ee74c0956374cd15a9b96022cc698f3039f92669`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:25 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 20:19:28 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 20:19:29 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 20:19:30 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 20:19:30 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 20:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 20:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 20:19:42 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 20:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 20:19:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 20:19:48 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 20:19:48 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 20:19:48 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 20:19:48 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 20:19:49 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 20:19:49 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 20:19:49 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 20:19:49 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 20:19:49 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 20:19:49 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6311611eec0d75cfc5a5b0550bcbe8277654c45760311d4c68cbf6bc07f3410`  
		Last Modified: Mon, 07 Aug 2023 20:20:40 GMT  
		Size: 60.8 MB (60816708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869efc37bdad525fcac6b7ac7d2f50926265be71714790af4c7bf72c2324fa3`  
		Last Modified: Mon, 07 Aug 2023 20:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294770ff9ee9544938a348b196c180dffcb2d054e5acf89eb7bffe3532e19e1`  
		Last Modified: Mon, 07 Aug 2023 20:20:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cddfa8ba0254f1108ae328eae229c7adc124e1d77558c9fb4d7d89b6b91f38`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60b6d238d22066f45902030974fce87391e836e1df2906dd6ae97a4b596c882`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c10aea7994a00039782ab1d341b65ebe73b39575affb94b42bbe6e4506316`  
		Last Modified: Mon, 07 Aug 2023 20:21:02 GMT  
		Size: 118.2 MB (118180315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576020c9a944e2b24ebca2b851d9be7a8ffe41364d07e2b018bfece41d50793`  
		Last Modified: Mon, 07 Aug 2023 20:20:54 GMT  
		Size: 5.4 KB (5417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:38edd994ce8e3a3dd37e72ad2964b3b48b320e1a7ba43a9c3ab3c48a09146fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178736193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6edf34148d1e29255cc39b92fe59f1e14f5142c1d45a81aa688f91990b752b`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
# Mon, 07 Aug 2023 20:16:44 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:01:45 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Mon, 07 Aug 2023 21:02:01 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Mon, 07 Aug 2023 21:02:06 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 07 Aug 2023 21:02:07 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Mon, 07 Aug 2023 21:02:08 GMT
ARG BONITA_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BRANDING_VERSION
# Mon, 07 Aug 2023 21:02:09 GMT
ARG BONITA_SHA256
# Mon, 07 Aug 2023 21:02:10 GMT
ARG BASE_URL
# Mon, 07 Aug 2023 21:02:11 GMT
ARG BONITA_URL
# Mon, 07 Aug 2023 21:02:56 GMT
ENV BONITA_VERSION=8.0.0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BRANDING_VERSION=2023.1-u0
# Mon, 07 Aug 2023 21:02:57 GMT
ENV BONITA_SHA256=2141b33d5835a0205e6da06580f75f44fd79c798552d4d1c3b304e6fa1b69a60
# Mon, 07 Aug 2023 21:02:58 GMT
ENV ZIP_FILE=BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:02:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 07 Aug 2023 21:03:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2023.1-u0/BonitaCommunity-2023.1-u0.zip
# Mon, 07 Aug 2023 21:03:03 GMT
RUN mkdir /opt/files
# Mon, 07 Aug 2023 21:03:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Mon, 07 Aug 2023 21:03:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Mon, 07 Aug 2023 21:03:21 GMT
ENV HTTP_API=false
# Mon, 07 Aug 2023 21:03:22 GMT
ENV HTTP_API_USERNAME=http-api
# Mon, 07 Aug 2023 21:03:23 GMT
ENV HTTP_API_PASSWORD=
# Mon, 07 Aug 2023 21:03:25 GMT
ENV MONITORING_USERNAME=monitoring
# Mon, 07 Aug 2023 21:03:26 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Mon, 07 Aug 2023 21:03:28 GMT
ENV JMX_REMOTE_ACCESS=false
# Mon, 07 Aug 2023 21:03:29 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Mon, 07 Aug 2023 21:03:30 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Mon, 07 Aug 2023 21:03:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Mon, 07 Aug 2023 21:03:34 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Mon, 07 Aug 2023 21:03:35 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Mon, 07 Aug 2023 21:03:36 GMT
ENV HTTP_MAX_THREADS=20
# Mon, 07 Aug 2023 21:03:36 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Mon, 07 Aug 2023 21:03:37 GMT
EXPOSE 8080 9000
# Mon, 07 Aug 2023 21:03:37 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Mon, 07 Aug 2023 21:03:37 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52e39089587119c893e8db183ebde539a650deb955194ce0600fbebad5aecd`  
		Last Modified: Mon, 07 Aug 2023 21:05:05 GMT  
		Size: 57.7 MB (57743515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87965a328a2c22d3308e03735bfc2684ea2ced2293ef2e866da9c04359480f26`  
		Last Modified: Mon, 07 Aug 2023 21:04:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e767b2a6ab7991182df5d0ca92d155ab8f64d78a5e2cb874ba49c346e9336`  
		Last Modified: Mon, 07 Aug 2023 21:04:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbf00b32a5ffbc82c2e22e3eae113f97e07a98a6f28a66ee8cc7426c086340e`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d2b99ce483dbb61d5638c55230f5081c6b912fd021846ce90f998fe4b00bf`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 3.0 KB (3047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04193e5ce6c7bfb73f99854d069a17eec4ca0ab8bd967de019f89c2fd0363e`  
		Last Modified: Mon, 07 Aug 2023 21:05:43 GMT  
		Size: 118.2 MB (118180324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7d34d1c6a44476bc5350e7b944a27644c90115e582a0d889f6b12c3ff2393`  
		Last Modified: Mon, 07 Aug 2023 21:05:26 GMT  
		Size: 5.4 KB (5418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
