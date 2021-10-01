<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.6`](#bonita7106)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.4`](#bonita7114)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:4540a66faca5eddb09c489f1502da84c0a8e4cb53b3b33154af0493842a666e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:cf985e502beeda7bd213e4dc3693b5cfd446649e79cf2c0ee2a42300216dd863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237233028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8faf747c59cd928e06fcf2203462737f87491ecd4c493d9f675a5f9c033cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:23:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:23:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:23:09 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:23:10 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:23:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:23:15 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:23:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:23:17 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:23:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:23:17 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:23:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed2f0a34ec7142b310f91d2f7ff94491fe271f681d1c0291b69c435abeba8f6`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730994432f980a3f07c8221390194452b08adaed9fa66daa66bfc1b3a8de5e36`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f5d7b809750eafcb136c948b160bcb2ea131f98cd825ad396179dd403dcdf`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef3a2fb4265fb966417cfe461e5d74bab49a20525b8cda63cb71e690843252`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dbde33b8607bcd5550cf36354dc50a802a53eac3ffcc3304477599273ba28e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226334004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1aa0819625c2f2587cedf8b8c4991d872594b067ebb98e96c65080d71af486`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:12:09 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:12:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:12 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:12:12 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:12:13 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:12:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:12:17 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:19 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:19 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96344b1ed8fdc3a7e4c6982958db4e3db69e1c243b99a310d69c2a647186d799`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a80275c26cbf501b20ec3280ac760bc2d08edfd02c4bfbc5883f9203f0aa8d`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 6.9 KB (6938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2236e483c06abc6f1a2ad6cc261ce0ef609048f07ba63ff4f6809d6a9fdc49`  
		Last Modified: Fri, 01 Oct 2021 03:13:47 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ed7af5efb5ad02a38247d168986cfbd102e6db255f183e4a2f19bbd5c430a8`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:2a6e551a5bd891abe055c5d3d9cdeaf51fd8d396f78c85cfb15615a6ea13d4e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233852199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6637b1b076c10f7d06f93e4de13692ebd64c32e3798b8e5cd4279f111bd2e367`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:18:05 GMT
ARG BRANDING_VERSION
# Tue, 31 Aug 2021 03:18:09 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:18:12 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:18:20 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:18:23 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 31 Aug 2021 03:18:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 31 Aug 2021 03:18:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 31 Aug 2021 03:18:34 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:18:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:19:02 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:19:03 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 31 Aug 2021 03:19:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:19:26 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:19:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:19:46 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:19:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:19:57 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:20:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a6dcceeb84150e152f7d2042a19418478b89434c18c29f816842761aebb84`  
		Last Modified: Tue, 31 Aug 2021 03:21:46 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709568a28e21e633e7c8714f0d7c15f5da8998019a55ab816fb0b6801fbfd65e`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba285a6b98fd908e3b4653f4ad1e188d38918991721f88d13cdfc321aebca4f8`  
		Last Modified: Tue, 31 Aug 2021 03:21:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ef0f91abdc722f016ef5cf11495031666b723bca3aec839d977e7340f489dd`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:6a49dd868f4b92a17db6187993c1d7b1cbd04cf4c69e4e2e3e8c464588dbf74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:c9aef5e0f249b8c478dbe9a1627b236dc937d902ebfb4047972853b6e82ca764
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242322192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1b98e8f2c1c14f5006826970981dabb2d5d85f91b4bf1e1251a48151cb2f8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:21:03 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 01 Oct 2021 03:21:49 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:51 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:21:52 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:21:55 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:21:56 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 01 Oct 2021 03:21:57 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 01 Oct 2021 03:22:00 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:22:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:22:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 01 Oct 2021 03:22:03 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:22:03 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 01 Oct 2021 03:22:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 01 Oct 2021 03:22:04 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:22:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd754908e13c860de1e431f70f3d9911b7d1c7e023412775d096f89b56dd37`  
		Last Modified: Fri, 01 Oct 2021 03:23:51 GMT  
		Size: 117.1 MB (117054878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb213b07d9b2a84bdbecfceb625729e774b059941020b31a9a6743c1682337c3`  
		Last Modified: Fri, 01 Oct 2021 03:23:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b83748ca3f856836892ae78c3e1d3198eb96716d5a3931c3cae26e6be0aacb6`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 1.9 KB (1906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce23d74d9b2942c8c752815bf2b7bb4aa8d92726fa1b45edab39ecab4159b91`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 576.9 KB (576930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6936bcc70fcfbc86bbe353e8fcfaaf57048d37d3b2f0865fa6b35b1514a0111`  
		Last Modified: Fri, 01 Oct 2021 03:23:38 GMT  
		Size: 98.0 MB (97973946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8c04f8db8a4878427df717de46207063b08c016933d3eb17c573f2760eb78f`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 7.7 KB (7650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5ffd1240a3edca88a0c1b20a470131282f5d5293a39f8ac8e1054f891245a9`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dc46426e4d55fe55256ae2fe9a281cb814548030ef2b0ea2f85374115bdad9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231031822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ef88c0147288c24bb2bee595ad44e0487b34719912984c41d50a8d77185f81`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:10:16 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 01 Oct 2021 03:10:45 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:10:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:10:47 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:10:58 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:10:59 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 01 Oct 2021 03:10:59 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 01 Oct 2021 03:11:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:11:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 01 Oct 2021 03:11:01 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 01 Oct 2021 03:11:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:11:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:11:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 01 Oct 2021 03:11:07 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:11:08 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 01 Oct 2021 03:11:08 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 01 Oct 2021 03:11:08 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:11:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dc030b9450ab01b9922083623e4d43e9afdc3212e2b885d2bae34399252c62`  
		Last Modified: Fri, 01 Oct 2021 03:13:03 GMT  
		Size: 108.8 MB (108772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f97372dc9489cc7eac8b6532fbd4e2eea78da6b6f9924bc8b041b8ad7b36ee`  
		Last Modified: Fri, 01 Oct 2021 03:12:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cddb0731a712a5ac532d8f2e61719f8e6a671d476517f59973565c77ae138be`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf42254624fe6008cc111e3b4363e58b61bc45e76a21f27389d8b5226dddb6a`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 547.0 KB (546957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc91ee64a161e65d5f2b6bc3fa214edd5d4ad4a53222f00e39b19c3ef66f96a`  
		Last Modified: Fri, 01 Oct 2021 03:12:50 GMT  
		Size: 98.0 MB (97973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863c6bdf65b203d8548ce47497f7c32567b56603627d8c61dff78893a32184e`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 7.7 KB (7651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d340d45cee37f0300c95ed270b11ad637208efdb7f4af42ebfd0084813f6121b`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:0ae6c6450c051c25e61270b1a58b8acdae9c5c0abd9f0bcb5d05b795864300b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240327540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b74e981f8d30d34825dd3ce487e3d65a484c148b34f83c95cf71f7c9a5ecd7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:03:49 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 31 Aug 2021 03:09:22 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:09:44 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:09:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:10:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:10:20 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:10:23 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:10:27 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:10:31 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:10:33 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 31 Aug 2021 03:10:38 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 31 Aug 2021 03:10:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:10:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 31 Aug 2021 03:10:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 31 Aug 2021 03:11:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 31 Aug 2021 03:11:22 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 31 Aug 2021 03:11:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 31 Aug 2021 03:11:39 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:11:41 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 31 Aug 2021 03:11:42 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 31 Aug 2021 03:11:48 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:11:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add44339faca2d4e791ed66e2cc50a15e7bda3647d29de7ae9628db9a1493fc`  
		Last Modified: Tue, 31 Aug 2021 03:21:03 GMT  
		Size: 111.4 MB (111357716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b827ba8115e75901e84e8190622e4d47dca42d7cdf1b1fe977bcb323235f9b`  
		Last Modified: Tue, 31 Aug 2021 03:20:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffd233d9be9777560e7dd5ad2a212327772e2cc680c97b23a38e50f6efeb5f4`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4db659952a332fe2eadf615eaaa663b32956a03131296c855ab00d086a49f9`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 546.7 KB (546736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23195d1ede89cb6aa100ddfbc20aae90b9a811f215921fbf7bb9767d0f8d866c`  
		Last Modified: Tue, 31 Aug 2021 03:20:49 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80c5bdf7ebccef54348c023d7cd195c4bb6c3dbe599a831c0d8cf4bada53f2`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c942391fbaeac4398aa5af8f95bd135bc3f10263ed371efe463398c200793261`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 1.6 KB (1647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:6a49dd868f4b92a17db6187993c1d7b1cbd04cf4c69e4e2e3e8c464588dbf74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:c9aef5e0f249b8c478dbe9a1627b236dc937d902ebfb4047972853b6e82ca764
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242322192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1b98e8f2c1c14f5006826970981dabb2d5d85f91b4bf1e1251a48151cb2f8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:21:03 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 01 Oct 2021 03:21:49 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:51 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:21:52 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:21:55 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:21:55 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:21:56 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:21:56 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 01 Oct 2021 03:21:57 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 01 Oct 2021 03:22:00 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:22:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:22:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 01 Oct 2021 03:22:03 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:22:03 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 01 Oct 2021 03:22:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 01 Oct 2021 03:22:04 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:22:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd754908e13c860de1e431f70f3d9911b7d1c7e023412775d096f89b56dd37`  
		Last Modified: Fri, 01 Oct 2021 03:23:51 GMT  
		Size: 117.1 MB (117054878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb213b07d9b2a84bdbecfceb625729e774b059941020b31a9a6743c1682337c3`  
		Last Modified: Fri, 01 Oct 2021 03:23:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b83748ca3f856836892ae78c3e1d3198eb96716d5a3931c3cae26e6be0aacb6`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 1.9 KB (1906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce23d74d9b2942c8c752815bf2b7bb4aa8d92726fa1b45edab39ecab4159b91`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 576.9 KB (576930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6936bcc70fcfbc86bbe353e8fcfaaf57048d37d3b2f0865fa6b35b1514a0111`  
		Last Modified: Fri, 01 Oct 2021 03:23:38 GMT  
		Size: 98.0 MB (97973946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8c04f8db8a4878427df717de46207063b08c016933d3eb17c573f2760eb78f`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 7.7 KB (7650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5ffd1240a3edca88a0c1b20a470131282f5d5293a39f8ac8e1054f891245a9`  
		Last Modified: Fri, 01 Oct 2021 03:23:33 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dc46426e4d55fe55256ae2fe9a281cb814548030ef2b0ea2f85374115bdad9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231031822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ef88c0147288c24bb2bee595ad44e0487b34719912984c41d50a8d77185f81`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:10:16 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 01 Oct 2021 03:10:45 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:10:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:10:47 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:10:58 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:10:59 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:10:59 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 01 Oct 2021 03:10:59 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 01 Oct 2021 03:11:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:11:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 01 Oct 2021 03:11:01 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 01 Oct 2021 03:11:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:11:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 01 Oct 2021 03:11:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 01 Oct 2021 03:11:07 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:11:08 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 01 Oct 2021 03:11:08 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 01 Oct 2021 03:11:08 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:11:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dc030b9450ab01b9922083623e4d43e9afdc3212e2b885d2bae34399252c62`  
		Last Modified: Fri, 01 Oct 2021 03:13:03 GMT  
		Size: 108.8 MB (108772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f97372dc9489cc7eac8b6532fbd4e2eea78da6b6f9924bc8b041b8ad7b36ee`  
		Last Modified: Fri, 01 Oct 2021 03:12:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cddb0731a712a5ac532d8f2e61719f8e6a671d476517f59973565c77ae138be`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf42254624fe6008cc111e3b4363e58b61bc45e76a21f27389d8b5226dddb6a`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 547.0 KB (546957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc91ee64a161e65d5f2b6bc3fa214edd5d4ad4a53222f00e39b19c3ef66f96a`  
		Last Modified: Fri, 01 Oct 2021 03:12:50 GMT  
		Size: 98.0 MB (97973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863c6bdf65b203d8548ce47497f7c32567b56603627d8c61dff78893a32184e`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 7.7 KB (7651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d340d45cee37f0300c95ed270b11ad637208efdb7f4af42ebfd0084813f6121b`  
		Last Modified: Fri, 01 Oct 2021 03:12:45 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:0ae6c6450c051c25e61270b1a58b8acdae9c5c0abd9f0bcb5d05b795864300b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240327540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b74e981f8d30d34825dd3ce487e3d65a484c148b34f83c95cf71f7c9a5ecd7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:03:49 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 31 Aug 2021 03:09:22 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:09:44 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:09:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:10:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:10:20 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:10:23 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:10:27 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:10:31 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:10:33 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 31 Aug 2021 03:10:38 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 31 Aug 2021 03:10:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:10:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 31 Aug 2021 03:10:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 31 Aug 2021 03:11:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 31 Aug 2021 03:11:22 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 31 Aug 2021 03:11:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 31 Aug 2021 03:11:39 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:11:41 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 31 Aug 2021 03:11:42 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 31 Aug 2021 03:11:48 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:11:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add44339faca2d4e791ed66e2cc50a15e7bda3647d29de7ae9628db9a1493fc`  
		Last Modified: Tue, 31 Aug 2021 03:21:03 GMT  
		Size: 111.4 MB (111357716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b827ba8115e75901e84e8190622e4d47dca42d7cdf1b1fe977bcb323235f9b`  
		Last Modified: Tue, 31 Aug 2021 03:20:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffd233d9be9777560e7dd5ad2a212327772e2cc680c97b23a38e50f6efeb5f4`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4db659952a332fe2eadf615eaaa663b32956a03131296c855ab00d086a49f9`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 546.7 KB (546736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23195d1ede89cb6aa100ddfbc20aae90b9a811f215921fbf7bb9767d0f8d866c`  
		Last Modified: Tue, 31 Aug 2021 03:20:49 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80c5bdf7ebccef54348c023d7cd195c4bb6c3dbe599a831c0d8cf4bada53f2`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c942391fbaeac4398aa5af8f95bd135bc3f10263ed371efe463398c200793261`  
		Last Modified: Tue, 31 Aug 2021 03:20:41 GMT  
		Size: 1.6 KB (1647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:3a8866041d202cbaf62bd6a5a7cd70154df101cfe45901e6b4305d454671eace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:bbdaba7e3164c62b94ae8f9057594d6a32869b7386e015aad82ff81995d49e68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234165396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de9e07975fb21d8ce06a92bc4d429cf7b94e71b793303bf0ecc303cbaad83f9a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 01 Oct 2021 03:22:46 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:22:47 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:22:48 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:22:48 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 01 Oct 2021 03:22:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:22:53 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:22:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:22:55 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:22:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:22:55 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:22:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b295d7c5302141dd8bfd8a706f2a8b68a05a3efec81da0fd09d1d7716799329`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c605799b5599db9cd1d8ac88a61c687eef4a8b3957d75b2570f6fbe3bb1423c`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d504f928d3c01acc2fef88c30402c886cf56ffffb19bf64b2991f516f04640f9`  
		Last Modified: Fri, 01 Oct 2021 03:24:12 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803bfd0d48da39732d2e4d1275a3d8eed84e87d3c1cb7ff8c95cd467e39ec3c5`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c657a1aecdc28a3e93b2f4f6d0624dc993108e31ff49328f2aae5fbb95ce249e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223266380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c226b3fc88443bf1b34c3398dd3e4f39109172b081f8e9a5a7b712bd78777fd`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:11:51 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 01 Oct 2021 03:11:52 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:11:53 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:11:54 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:11:54 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 01 Oct 2021 03:11:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:11:59 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:00 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:00 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:00 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:01 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca2ea259c0c1a55ef58023b3d1039fec097033c710a252c5309753c04f7e6d8`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddd9a625363a97d90b9aa063e3a54554d8c765ea411b9e14684dfcee1e6790c`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf6207d95cc2dc46c9f92c0a94baf50d083e5d224baaad20225456e77ccd149`  
		Last Modified: Fri, 01 Oct 2021 03:13:20 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e46a4487eaf1e3e37bc05e4ed78a9257cc612bbb75eca7da0db08919e36bf`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:aba9c3174ce3d2f36951dba013b6d3af8f231e695e07659ed37fe8be538f8582
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230784560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f14dc7c890827eefb5f79f2d6153f6e19e26684f58e4212278aae56e2ae059b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:16:01 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:16:07 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:16:09 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:16:14 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 31 Aug 2021 03:16:17 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 31 Aug 2021 03:16:20 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 31 Aug 2021 03:16:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 31 Aug 2021 03:16:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:16:46 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:16:48 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 31 Aug 2021 03:17:03 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:17:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:17:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:17:23 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:17:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:17:30 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:17:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2455a524c6bc2143b839a7531d140e08fb9557b58b83bc39ab745f4f27b35ad4`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ffbec42c83b4a8072a5bdea66efb9e2835f9d5a967ec44332bbfbb1f043429`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6976cb44c5c1e4ca88a4f5e3d5e8fd1361b495050ed551041f0b8f0236553410`  
		Last Modified: Tue, 31 Aug 2021 03:21:25 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c74acd6e8d186eb6f6bc7ce65cfbae0348073dce3ad27e6ca6dde039f27bc7`  
		Last Modified: Tue, 31 Aug 2021 03:21:16 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:3a8866041d202cbaf62bd6a5a7cd70154df101cfe45901e6b4305d454671eace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:bbdaba7e3164c62b94ae8f9057594d6a32869b7386e015aad82ff81995d49e68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234165396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de9e07975fb21d8ce06a92bc4d429cf7b94e71b793303bf0ecc303cbaad83f9a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 01 Oct 2021 03:22:46 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:22:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:22:47 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:22:48 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:22:48 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 01 Oct 2021 03:22:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:22:53 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:22:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:22:55 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:22:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:22:55 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:22:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b295d7c5302141dd8bfd8a706f2a8b68a05a3efec81da0fd09d1d7716799329`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c605799b5599db9cd1d8ac88a61c687eef4a8b3957d75b2570f6fbe3bb1423c`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d504f928d3c01acc2fef88c30402c886cf56ffffb19bf64b2991f516f04640f9`  
		Last Modified: Fri, 01 Oct 2021 03:24:12 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803bfd0d48da39732d2e4d1275a3d8eed84e87d3c1cb7ff8c95cd467e39ec3c5`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c657a1aecdc28a3e93b2f4f6d0624dc993108e31ff49328f2aae5fbb95ce249e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223266380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c226b3fc88443bf1b34c3398dd3e4f39109172b081f8e9a5a7b712bd78777fd`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:11:51 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 01 Oct 2021 03:11:52 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:11:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 01 Oct 2021 03:11:53 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:11:54 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:11:54 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 01 Oct 2021 03:11:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:11:59 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:00 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:00 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:00 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:01 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca2ea259c0c1a55ef58023b3d1039fec097033c710a252c5309753c04f7e6d8`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddd9a625363a97d90b9aa063e3a54554d8c765ea411b9e14684dfcee1e6790c`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf6207d95cc2dc46c9f92c0a94baf50d083e5d224baaad20225456e77ccd149`  
		Last Modified: Fri, 01 Oct 2021 03:13:20 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e46a4487eaf1e3e37bc05e4ed78a9257cc612bbb75eca7da0db08919e36bf`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:aba9c3174ce3d2f36951dba013b6d3af8f231e695e07659ed37fe8be538f8582
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230784560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f14dc7c890827eefb5f79f2d6153f6e19e26684f58e4212278aae56e2ae059b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:16:01 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:16:07 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:16:09 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:16:14 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 31 Aug 2021 03:16:17 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 31 Aug 2021 03:16:20 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 31 Aug 2021 03:16:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:16:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 31 Aug 2021 03:16:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:16:46 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:16:48 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 31 Aug 2021 03:17:03 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:17:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:17:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:17:23 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:17:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:17:30 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:17:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2455a524c6bc2143b839a7531d140e08fb9557b58b83bc39ab745f4f27b35ad4`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ffbec42c83b4a8072a5bdea66efb9e2835f9d5a967ec44332bbfbb1f043429`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6976cb44c5c1e4ca88a4f5e3d5e8fd1361b495050ed551041f0b8f0236553410`  
		Last Modified: Tue, 31 Aug 2021 03:21:25 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c74acd6e8d186eb6f6bc7ce65cfbae0348073dce3ad27e6ca6dde039f27bc7`  
		Last Modified: Tue, 31 Aug 2021 03:21:16 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:4540a66faca5eddb09c489f1502da84c0a8e4cb53b3b33154af0493842a666e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:cf985e502beeda7bd213e4dc3693b5cfd446649e79cf2c0ee2a42300216dd863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237233028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8faf747c59cd928e06fcf2203462737f87491ecd4c493d9f675a5f9c033cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:23:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:23:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:23:09 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:23:10 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:23:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:23:15 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:23:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:23:17 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:23:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:23:17 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:23:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed2f0a34ec7142b310f91d2f7ff94491fe271f681d1c0291b69c435abeba8f6`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730994432f980a3f07c8221390194452b08adaed9fa66daa66bfc1b3a8de5e36`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f5d7b809750eafcb136c948b160bcb2ea131f98cd825ad396179dd403dcdf`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef3a2fb4265fb966417cfe461e5d74bab49a20525b8cda63cb71e690843252`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dbde33b8607bcd5550cf36354dc50a802a53eac3ffcc3304477599273ba28e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226334004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1aa0819625c2f2587cedf8b8c4991d872594b067ebb98e96c65080d71af486`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:12:09 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:12:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:12 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:12:12 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:12:13 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:12:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:12:17 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:19 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:19 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96344b1ed8fdc3a7e4c6982958db4e3db69e1c243b99a310d69c2a647186d799`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a80275c26cbf501b20ec3280ac760bc2d08edfd02c4bfbc5883f9203f0aa8d`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 6.9 KB (6938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2236e483c06abc6f1a2ad6cc261ce0ef609048f07ba63ff4f6809d6a9fdc49`  
		Last Modified: Fri, 01 Oct 2021 03:13:47 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ed7af5efb5ad02a38247d168986cfbd102e6db255f183e4a2f19bbd5c430a8`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:2a6e551a5bd891abe055c5d3d9cdeaf51fd8d396f78c85cfb15615a6ea13d4e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233852199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6637b1b076c10f7d06f93e4de13692ebd64c32e3798b8e5cd4279f111bd2e367`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:18:05 GMT
ARG BRANDING_VERSION
# Tue, 31 Aug 2021 03:18:09 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:18:12 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:18:20 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:18:23 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 31 Aug 2021 03:18:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 31 Aug 2021 03:18:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 31 Aug 2021 03:18:34 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:18:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:19:02 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:19:03 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 31 Aug 2021 03:19:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:19:26 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:19:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:19:46 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:19:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:19:57 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:20:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a6dcceeb84150e152f7d2042a19418478b89434c18c29f816842761aebb84`  
		Last Modified: Tue, 31 Aug 2021 03:21:46 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709568a28e21e633e7c8714f0d7c15f5da8998019a55ab816fb0b6801fbfd65e`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba285a6b98fd908e3b4653f4ad1e188d38918991721f88d13cdfc321aebca4f8`  
		Last Modified: Tue, 31 Aug 2021 03:21:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ef0f91abdc722f016ef5cf11495031666b723bca3aec839d977e7340f489dd`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:4540a66faca5eddb09c489f1502da84c0a8e4cb53b3b33154af0493842a666e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:cf985e502beeda7bd213e4dc3693b5cfd446649e79cf2c0ee2a42300216dd863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237233028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8faf747c59cd928e06fcf2203462737f87491ecd4c493d9f675a5f9c033cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:23:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:23:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:23:09 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:23:10 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:23:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:23:15 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:23:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:23:17 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:23:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:23:17 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:23:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed2f0a34ec7142b310f91d2f7ff94491fe271f681d1c0291b69c435abeba8f6`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730994432f980a3f07c8221390194452b08adaed9fa66daa66bfc1b3a8de5e36`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f5d7b809750eafcb136c948b160bcb2ea131f98cd825ad396179dd403dcdf`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef3a2fb4265fb966417cfe461e5d74bab49a20525b8cda63cb71e690843252`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dbde33b8607bcd5550cf36354dc50a802a53eac3ffcc3304477599273ba28e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226334004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1aa0819625c2f2587cedf8b8c4991d872594b067ebb98e96c65080d71af486`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:12:09 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:12:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:12 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:12:12 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:12:13 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:12:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:12:17 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:19 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:19 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96344b1ed8fdc3a7e4c6982958db4e3db69e1c243b99a310d69c2a647186d799`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a80275c26cbf501b20ec3280ac760bc2d08edfd02c4bfbc5883f9203f0aa8d`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 6.9 KB (6938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2236e483c06abc6f1a2ad6cc261ce0ef609048f07ba63ff4f6809d6a9fdc49`  
		Last Modified: Fri, 01 Oct 2021 03:13:47 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ed7af5efb5ad02a38247d168986cfbd102e6db255f183e4a2f19bbd5c430a8`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:2a6e551a5bd891abe055c5d3d9cdeaf51fd8d396f78c85cfb15615a6ea13d4e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233852199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6637b1b076c10f7d06f93e4de13692ebd64c32e3798b8e5cd4279f111bd2e367`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:18:05 GMT
ARG BRANDING_VERSION
# Tue, 31 Aug 2021 03:18:09 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:18:12 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:18:20 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:18:23 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 31 Aug 2021 03:18:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 31 Aug 2021 03:18:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 31 Aug 2021 03:18:34 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:18:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:19:02 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:19:03 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 31 Aug 2021 03:19:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:19:26 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:19:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:19:46 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:19:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:19:57 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:20:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a6dcceeb84150e152f7d2042a19418478b89434c18c29f816842761aebb84`  
		Last Modified: Tue, 31 Aug 2021 03:21:46 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709568a28e21e633e7c8714f0d7c15f5da8998019a55ab816fb0b6801fbfd65e`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba285a6b98fd908e3b4653f4ad1e188d38918991721f88d13cdfc321aebca4f8`  
		Last Modified: Tue, 31 Aug 2021 03:21:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ef0f91abdc722f016ef5cf11495031666b723bca3aec839d977e7340f489dd`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:4540a66faca5eddb09c489f1502da84c0a8e4cb53b3b33154af0493842a666e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:cf985e502beeda7bd213e4dc3693b5cfd446649e79cf2c0ee2a42300216dd863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237233028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8faf747c59cd928e06fcf2203462737f87491ecd4c493d9f675a5f9c033cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:22:38 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:22:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:22:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:22:45 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:23:06 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:23:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:07 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:23:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:23:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:23:09 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:23:10 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:23:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:23:15 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:23:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:23:17 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:23:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:23:17 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:23:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26e82d109872f0211374fbdd95c3c9f1799fe2afa49aee374740e411069a9`  
		Last Modified: Fri, 01 Oct 2021 03:24:22 GMT  
		Size: 93.5 MB (93524773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d98d32b0e20a905a110297e723006f1a0a3914d3c02eaa7ec1910002aca2d5b`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a615c2a472e58e3e3ca78ee9119db9aa6cbfba55f63e200cb23320af9a9b39af`  
		Last Modified: Fri, 01 Oct 2021 03:24:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bff023499a597e17c3b59e6fa979fc6e0c958f530d7aa8b6a5ad477d197b07`  
		Last Modified: Fri, 01 Oct 2021 03:24:06 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed2f0a34ec7142b310f91d2f7ff94491fe271f681d1c0291b69c435abeba8f6`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730994432f980a3f07c8221390194452b08adaed9fa66daa66bfc1b3a8de5e36`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f5d7b809750eafcb136c948b160bcb2ea131f98cd825ad396179dd403dcdf`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef3a2fb4265fb966417cfe461e5d74bab49a20525b8cda63cb71e690843252`  
		Last Modified: Fri, 01 Oct 2021 03:24:33 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dbde33b8607bcd5550cf36354dc50a802a53eac3ffcc3304477599273ba28e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226334004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1aa0819625c2f2587cedf8b8c4991d872594b067ebb98e96c65080d71af486`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 01 Oct 2021 03:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:11:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 01 Oct 2021 03:11:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 01 Oct 2021 03:11:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 01 Oct 2021 03:11:51 GMT
ARG BONITA_VERSION
# Fri, 01 Oct 2021 03:12:09 GMT
ARG BRANDING_VERSION
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_SHA256
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BASE_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ARG BONITA_URL
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 01 Oct 2021 03:12:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 01 Oct 2021 03:12:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 01 Oct 2021 03:12:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 01 Oct 2021 03:12:12 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 01 Oct 2021 03:12:12 GMT
RUN mkdir /opt/files
# Fri, 01 Oct 2021 03:12:13 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 01 Oct 2021 03:12:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 01 Oct 2021 03:12:17 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 01 Oct 2021 03:12:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 01 Oct 2021 03:12:19 GMT
VOLUME [/opt/bonita]
# Fri, 01 Oct 2021 03:12:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 01 Oct 2021 03:12:19 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:12:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2961f2a4bb67da5eacd8035656d46b0b9ce152f747e5a4866615a41912e77`  
		Last Modified: Fri, 01 Oct 2021 03:13:29 GMT  
		Size: 85.6 MB (85633335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbadb494c476cbc9027d808b5602ca944569d12f137a0d2ecdd29df277acd0e6`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f264659a1637719775ef2123464f83436ff5bb0548fc6dcfd79901ac8c637`  
		Last Modified: Fri, 01 Oct 2021 03:13:16 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d568262d6dd7434b5917a08133c89776d2f316d5fe0322f20f5c224daf1fd3`  
		Last Modified: Fri, 01 Oct 2021 03:13:14 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96344b1ed8fdc3a7e4c6982958db4e3db69e1c243b99a310d69c2a647186d799`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a80275c26cbf501b20ec3280ac760bc2d08edfd02c4bfbc5883f9203f0aa8d`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 6.9 KB (6938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2236e483c06abc6f1a2ad6cc261ce0ef609048f07ba63ff4f6809d6a9fdc49`  
		Last Modified: Fri, 01 Oct 2021 03:13:47 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ed7af5efb5ad02a38247d168986cfbd102e6db255f183e4a2f19bbd5c430a8`  
		Last Modified: Fri, 01 Oct 2021 03:13:40 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:2a6e551a5bd891abe055c5d3d9cdeaf51fd8d396f78c85cfb15615a6ea13d4e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233852199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6637b1b076c10f7d06f93e4de13692ebd64c32e3798b8e5cd4279f111bd2e367`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:12:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 31 Aug 2021 03:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 31 Aug 2021 03:15:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 31 Aug 2021 03:15:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 31 Aug 2021 03:15:55 GMT
ARG BONITA_VERSION
# Tue, 31 Aug 2021 03:18:05 GMT
ARG BRANDING_VERSION
# Tue, 31 Aug 2021 03:18:09 GMT
ARG BONITA_SHA256
# Tue, 31 Aug 2021 03:18:12 GMT
ARG BASE_URL
# Tue, 31 Aug 2021 03:18:20 GMT
ARG BONITA_URL
# Tue, 31 Aug 2021 03:18:23 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 31 Aug 2021 03:18:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 31 Aug 2021 03:18:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 31 Aug 2021 03:18:34 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 31 Aug 2021 03:18:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 31 Aug 2021 03:18:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 31 Aug 2021 03:19:02 GMT
RUN mkdir /opt/files
# Tue, 31 Aug 2021 03:19:03 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 31 Aug 2021 03:19:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 31 Aug 2021 03:19:26 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 31 Aug 2021 03:19:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 31 Aug 2021 03:19:46 GMT
VOLUME [/opt/bonita]
# Tue, 31 Aug 2021 03:19:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 31 Aug 2021 03:19:57 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 03:20:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54978ae656d40037cfaec12659d83d17df3f111e5c260f8b00c5dc48967862b`  
		Last Modified: Tue, 31 Aug 2021 03:21:33 GMT  
		Size: 86.4 MB (86441451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe73f6d51a2d50268e599e7d89ba63e3c7ecaeebb9d94462603eade0789a5`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0555b6890c27c06b847697527af8c80b7ab11e7c04f51b2d34afa768079ee3`  
		Last Modified: Tue, 31 Aug 2021 03:21:18 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2debdb88d2a487637f51a90eddc12512ef172a3f9b78ac28492b922aad94b55`  
		Last Modified: Tue, 31 Aug 2021 03:21:15 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a6dcceeb84150e152f7d2042a19418478b89434c18c29f816842761aebb84`  
		Last Modified: Tue, 31 Aug 2021 03:21:46 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709568a28e21e633e7c8714f0d7c15f5da8998019a55ab816fb0b6801fbfd65e`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba285a6b98fd908e3b4653f4ad1e188d38918991721f88d13cdfc321aebca4f8`  
		Last Modified: Tue, 31 Aug 2021 03:21:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ef0f91abdc722f016ef5cf11495031666b723bca3aec839d977e7340f489dd`  
		Last Modified: Tue, 31 Aug 2021 03:21:45 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
