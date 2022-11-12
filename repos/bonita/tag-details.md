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
$ docker pull bonita@sha256:46ad987086548e5839651d5041f90636d38fc4a66e30bf5bb4295c0e0eee9e77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:7736099b5a0fbd690c9282ed0c65668f24379cd2b0aea81d64022a05fcc291fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235177846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5f4822d7f3a158aa5057883e28e3984b534eb8143176acf341878421824333`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:52:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:52:31 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:52:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:52:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:52:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:52:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:36 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:52:37 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:52:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:52:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:52:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:52:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:52:46 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:52:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:52:47 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:52:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce567665295479c898d7f9293183d345a196c03c51919bb8178a41a48b5189`  
		Last Modified: Tue, 25 Oct 2022 15:54:21 GMT  
		Size: 91.5 MB (91532751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24296c370e3d7d1bc9d7959bc4eb56acc21e565d5b0d18e5eaa0563694b0c3e0`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253985ca492d1beb31f18def10e14718cd7bd77d860f29d633a6fcba03bafd32`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79f052367f73c0fd44c535e0ed2e6de71c184b3fcbb8564ec76e29933ebae8`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 506.3 KB (506347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb3a632b1c91989f258db6dbc1a4fe32ce5500d0230cc8bc0ba1a5149e2ea9`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f373f10e42c90e6c198dc86af4f21cf553ee7625859da5df64ff6613a35c8fc`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d343a7f8a2f5c8e34eca93be022cd5cb2930c854d104aa8259aedc6a96a42`  
		Last Modified: Tue, 25 Oct 2022 15:54:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba0dba1bbc5b46c45ac45acba4b59eb44e633a1a3cba46ee17fdce628172a1`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:88388c1b022ed85f5376df978d4862b89fa75e91cf81b9da500af1d2e3908e0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226655649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fb01229803e98578deb5ae9e8f594f81885ca2794decbedec7dcea2a13183`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 00:59:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:59:42 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 00:59:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 00:59:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 00:59:46 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 26 Oct 2022 00:59:47 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 26 Oct 2022 00:59:48 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 00:59:48 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 26 Oct 2022 00:59:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 26 Oct 2022 00:59:54 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 26 Oct 2022 00:59:54 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 26 Oct 2022 00:59:55 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 00:59:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 00:59:55 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 00:59:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dffde860fbbd42392ff77e38759245966a7182f0139841187bb163042988818`  
		Last Modified: Wed, 26 Oct 2022 01:02:00 GMT  
		Size: 86.0 MB (86017735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e318176d0c45cf1a2a2350640427c957ec3776a87f5f73267ed9a8a07275d283`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d931702069558109778cb8b5766604f7bba0d5751648b05fcdb67392e95e74b`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43476e7c830ff308b935f68f7641882a5c0e2a6ba2dcd9a02f0a96ed239fd455`  
		Last Modified: Wed, 26 Oct 2022 01:01:50 GMT  
		Size: 475.8 KB (475799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece0e86607bb253229446bef9695d91765c4a5091daf19d6266a3de11ed34e11`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de99403106573ed9e00c47b1923fe08b08cbfa879b95785b828796cc470c1481`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10b77d72296b42c9faa55435320dc1823f9702b30ed6b21dadf93f18f99958f`  
		Last Modified: Wed, 26 Oct 2022 01:01:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf370bf521d66fa39c549a560e25bea7556bdc6537541ca1afe64590a472febb`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:5ef4e3a6c96b32ec231f530e059dfe1b71baaa78cf750ab37b77ce2a360a13fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234160943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0875be850095eb8c2e1a31ee88f765296c9b98bf35f7e4c74819045b70cab1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:00:32 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:00:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:00:39 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:00:41 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:43 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:00:45 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:00:45 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:00:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:00:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:00:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:00:57 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:00:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:00:58 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:00:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bf908b740a06082b8cd17325b6597a3ef1380e9b186700b0fd995d958f16e`  
		Last Modified: Tue, 25 Oct 2022 15:03:47 GMT  
		Size: 86.8 MB (86816119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33059b8fceb675324742914a9bee1d0d76a22aa07638a8de985fe581d01f8703`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dcaef92716cfc0a27df29c6b4400bfbb5c016b38b0b198c9bc23afd1f95a`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e4dbce9799a10ec7fb02699ab08e330dce68115b62afc5a8608a8789c870d9`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 475.3 KB (475349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfd48608a926fc9739c766d7212ad37c4e1b10431297e5804efbf57cb6fd41c`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d248f05ade088bc58ecb87d89fd543bc55a5c0e5f50b5b6a4672193188708ea`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e377df32a41bd395185b6a33edd822a7cd31e8bc9f43c65ac8cc97048ed381c7`  
		Last Modified: Tue, 25 Oct 2022 15:03:29 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ace1f942b1e9c2a34bcae77510d4ab73f379b2a3ba7f59d733c2d9be57e7a0e`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:b418388fca7b8c968ebb732007d68c154109f4586bb377b6db7f3b21cd3652f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:89428640a9e65a669dd2d80432a83d4f14fc3ea52f147fb79b9d166ac600834c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232910837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57327096a0152d53428bf600651aa3d02cdb3694163cd8ef3a135b17e15c58e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:53:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:53:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:53:18 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:53:22 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:53:23 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:24 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:53:24 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:53:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:53:40 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:53:40 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:53:41 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:53:41 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:53:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4d444062fb1490dc40701d8201083260f32115730e595fc7eb0533d308187`  
		Last Modified: Tue, 25 Oct 2022 15:55:24 GMT  
		Size: 91.5 MB (91532740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64575146ef008f8318b475f9ac6437b9e84f4f45a626a1c0a2ac042c0a55e5a7`  
		Last Modified: Tue, 25 Oct 2022 15:55:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc81f1ca4a9fa69f8ce85c888642403bc5357e6aa8e5c27303bf9f7c8ffddac9`  
		Last Modified: Tue, 25 Oct 2022 15:55:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb0c1f6517e5d16e967d48e5794a1c1058b6ca4d6306d8a88335b084159337a`  
		Last Modified: Tue, 25 Oct 2022 15:55:09 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2975d5c35bbdd01161a6f82800341af5759c8b1a323e3271cca4eab7723855e0`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab9e4a959c92acae9c3bcbc05fedc30218b0663e3a7f5ceb04467e0d66306ad`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243de80728f9d53ff507070746cf4c92c712b4d44f2ab894390fef71342fcc8`  
		Last Modified: Tue, 25 Oct 2022 15:55:15 GMT  
		Size: 113.7 MB (113727915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94a522f5fdfb28c2e883baf8366e0d084e337ed88db718eabb1ceb650712119`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:539215409c088cfcb37d88ddcd646c8b25c1236ad91f6a20b33faf6640c6e984
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224348182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93cb0763d302538b7abaa14fc82139b687f3ad29338619d420d897a8baabde22`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 01:00:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:00:25 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 01:00:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 01:00:28 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 26 Oct 2022 01:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:30 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 01:00:30 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 26 Oct 2022 01:00:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 26 Oct 2022 01:00:44 GMT
ENV HTTP_API=false
# Wed, 26 Oct 2022 01:00:45 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 01:00:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 01:00:46 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 01:00:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87e4b48be33c3874175426beae7bef698137d1ddd60124338a3ac84767adc60`  
		Last Modified: Wed, 26 Oct 2022 01:02:25 GMT  
		Size: 86.0 MB (86017619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b313f79a8a118790254b764e04d46bc0f62323e99e23fcbba7906fe08bc02`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d958fd260eec0c33924b9c62e4012d7d8e78b0a92b492aeb1ecd4b11264756`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38331e2fea86cd0d9001a29fe93170874e7860b09fea765b59a8e344739bb05c`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 859.6 KB (859577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbd70b5e8b6ae25fa5f4fdd0a87337386aa2a2254122d7edb8fa4cd90a17054`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d0d8b93e75ddc6c93f9ac045e05de138ce023e3b356ef0a44d36ebaffd360`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25031c28db0d261ab6c0772562e3e34d4529292ba5831e0c135ca64ad05d463a`  
		Last Modified: Wed, 26 Oct 2022 01:02:19 GMT  
		Size: 113.7 MB (113727925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea76a40bc6b6863b7451791e765deb70ae5631422a94b24c1a69839b7567a8`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:1c8d0507483f67a146cd92ee71a9932bb7c6d4322c75f804df880c2f03c5dfd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231826002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e64debf4d35b95287c13910032120f63ecd6d1528cd9cb6023e7abc7a6e2da`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:01:50 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:01:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:01:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:01:58 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:01:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:02:00 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:02:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:02:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:02:16 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:02:18 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:02:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:02:20 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:02:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0bd46ad19567c08c1713a7725bc00aed8394fd8f3ed9bec7ce4479c7b86c69`  
		Last Modified: Tue, 25 Oct 2022 15:04:25 GMT  
		Size: 86.8 MB (86816051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee497a65fbc1669cf497d7ff89f1db3a0bced0347b40783fe209d3d89a3b81`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca0ee0d23f6a8f675abb762ed413d8dd07e65f10b9bff344fd67aa25e41b97f`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f272d29db7fb9f929358e96e47a2bf8e985f250fb1f95263cc65ceda4a739`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 831.6 KB (831579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2593595c89246ea872f1210053f7de8f27b8acedefb4457a7555967dfa6c21b`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b956766cd724dc4b950cbc195f0ec3d47ba2afcfac99a559d3768331b07c7`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a965377d658a6e91c602615fed50e102395e8d0f341e60b676cb62f27c69d`  
		Last Modified: Tue, 25 Oct 2022 15:04:19 GMT  
		Size: 113.7 MB (113727947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f50859dcba4b5885bbf6f5f1b214871dfe8ab0be5c20d65e8e4cee31a75d4e`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:b418388fca7b8c968ebb732007d68c154109f4586bb377b6db7f3b21cd3652f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:89428640a9e65a669dd2d80432a83d4f14fc3ea52f147fb79b9d166ac600834c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232910837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57327096a0152d53428bf600651aa3d02cdb3694163cd8ef3a135b17e15c58e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:53:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:53:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:53:18 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:53:22 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:53:23 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:24 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:53:24 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:53:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:53:40 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:53:40 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:53:41 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:53:41 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:53:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4d444062fb1490dc40701d8201083260f32115730e595fc7eb0533d308187`  
		Last Modified: Tue, 25 Oct 2022 15:55:24 GMT  
		Size: 91.5 MB (91532740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64575146ef008f8318b475f9ac6437b9e84f4f45a626a1c0a2ac042c0a55e5a7`  
		Last Modified: Tue, 25 Oct 2022 15:55:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc81f1ca4a9fa69f8ce85c888642403bc5357e6aa8e5c27303bf9f7c8ffddac9`  
		Last Modified: Tue, 25 Oct 2022 15:55:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb0c1f6517e5d16e967d48e5794a1c1058b6ca4d6306d8a88335b084159337a`  
		Last Modified: Tue, 25 Oct 2022 15:55:09 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2975d5c35bbdd01161a6f82800341af5759c8b1a323e3271cca4eab7723855e0`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab9e4a959c92acae9c3bcbc05fedc30218b0663e3a7f5ceb04467e0d66306ad`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243de80728f9d53ff507070746cf4c92c712b4d44f2ab894390fef71342fcc8`  
		Last Modified: Tue, 25 Oct 2022 15:55:15 GMT  
		Size: 113.7 MB (113727915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94a522f5fdfb28c2e883baf8366e0d084e337ed88db718eabb1ceb650712119`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:539215409c088cfcb37d88ddcd646c8b25c1236ad91f6a20b33faf6640c6e984
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224348182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93cb0763d302538b7abaa14fc82139b687f3ad29338619d420d897a8baabde22`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 01:00:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:00:25 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 01:00:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 01:00:28 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 26 Oct 2022 01:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:30 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 01:00:30 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 26 Oct 2022 01:00:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 26 Oct 2022 01:00:44 GMT
ENV HTTP_API=false
# Wed, 26 Oct 2022 01:00:45 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 01:00:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 01:00:46 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 01:00:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87e4b48be33c3874175426beae7bef698137d1ddd60124338a3ac84767adc60`  
		Last Modified: Wed, 26 Oct 2022 01:02:25 GMT  
		Size: 86.0 MB (86017619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b313f79a8a118790254b764e04d46bc0f62323e99e23fcbba7906fe08bc02`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d958fd260eec0c33924b9c62e4012d7d8e78b0a92b492aeb1ecd4b11264756`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38331e2fea86cd0d9001a29fe93170874e7860b09fea765b59a8e344739bb05c`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 859.6 KB (859577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbd70b5e8b6ae25fa5f4fdd0a87337386aa2a2254122d7edb8fa4cd90a17054`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d0d8b93e75ddc6c93f9ac045e05de138ce023e3b356ef0a44d36ebaffd360`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25031c28db0d261ab6c0772562e3e34d4529292ba5831e0c135ca64ad05d463a`  
		Last Modified: Wed, 26 Oct 2022 01:02:19 GMT  
		Size: 113.7 MB (113727925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea76a40bc6b6863b7451791e765deb70ae5631422a94b24c1a69839b7567a8`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1c8d0507483f67a146cd92ee71a9932bb7c6d4322c75f804df880c2f03c5dfd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231826002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e64debf4d35b95287c13910032120f63ecd6d1528cd9cb6023e7abc7a6e2da`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:01:50 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:01:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:01:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:01:58 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:01:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:02:00 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:02:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:02:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:02:16 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:02:18 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:02:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:02:20 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:02:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0bd46ad19567c08c1713a7725bc00aed8394fd8f3ed9bec7ce4479c7b86c69`  
		Last Modified: Tue, 25 Oct 2022 15:04:25 GMT  
		Size: 86.8 MB (86816051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee497a65fbc1669cf497d7ff89f1db3a0bced0347b40783fe209d3d89a3b81`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca0ee0d23f6a8f675abb762ed413d8dd07e65f10b9bff344fd67aa25e41b97f`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f272d29db7fb9f929358e96e47a2bf8e985f250fb1f95263cc65ceda4a739`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 831.6 KB (831579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2593595c89246ea872f1210053f7de8f27b8acedefb4457a7555967dfa6c21b`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b956766cd724dc4b950cbc195f0ec3d47ba2afcfac99a559d3768331b07c7`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a965377d658a6e91c602615fed50e102395e8d0f341e60b676cb62f27c69d`  
		Last Modified: Tue, 25 Oct 2022 15:04:19 GMT  
		Size: 113.7 MB (113727947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f50859dcba4b5885bbf6f5f1b214871dfe8ab0be5c20d65e8e4cee31a75d4e`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:0f038ccdde32fa4b90a855ec5bb41db8434cfbe432cecbcde8abd01c88b0ad8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:92b3b92dc468cfc22704a83368c85d4758c878808548637ad8401f6ba78e5282
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176177804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a01742b56399308f70d74c2477c82b5f0562160950db295a6adb0b48e8dadf`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:31:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 10 Nov 2022 21:31:12 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 10 Nov 2022 21:31:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 10 Nov 2022 21:31:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BRANDING_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_SHA256
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BASE_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BONITA_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 10 Nov 2022 21:31:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:16 GMT
RUN mkdir /opt/files
# Thu, 10 Nov 2022 21:31:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 10 Nov 2022 21:31:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_PASSWORD=
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 10 Nov 2022 21:31:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 10 Nov 2022 21:31:26 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 10 Nov 2022 21:31:26 GMT
EXPOSE 8080 9000
# Thu, 10 Nov 2022 21:31:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 10 Nov 2022 21:31:26 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3ecf9c0764240ea4a002e97a93756470158670ab2d476271c5dff63411aba`  
		Last Modified: Thu, 10 Nov 2022 21:32:24 GMT  
		Size: 56.8 MB (56758527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a3561b22a1c5d6d0052ed6e609a9b4f439038a3c9316e4a18d113bccb1cbb`  
		Last Modified: Thu, 10 Nov 2022 21:32:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3521a1d72476ad9583383dfcada876476cbebf359be2854f3719b473260f64`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ecdb4041b3ae0840a5435e5c6d2ae2cf6a480e838b043cd029bc990ebfbbb2`  
		Last Modified: Thu, 10 Nov 2022 21:32:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2977a32ef333556aa544c36b6595d83f2cf92d76f429a58780b327eac6de9aca`  
		Last Modified: Thu, 10 Nov 2022 21:32:12 GMT  
		Size: 3.0 KB (3036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc41606a6fed8126df1e7a47259412bf23cca1aad6619f8bde287a1e2a81`  
		Last Modified: Thu, 10 Nov 2022 21:32:16 GMT  
		Size: 116.7 MB (116690815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2c6540a466d20ce7e64cbabe62163e54d535f2a5f75f8b7dfaae489c50e8e`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:0f038ccdde32fa4b90a855ec5bb41db8434cfbe432cecbcde8abd01c88b0ad8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:92b3b92dc468cfc22704a83368c85d4758c878808548637ad8401f6ba78e5282
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176177804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a01742b56399308f70d74c2477c82b5f0562160950db295a6adb0b48e8dadf`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:31:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 10 Nov 2022 21:31:12 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 10 Nov 2022 21:31:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 10 Nov 2022 21:31:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BRANDING_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_SHA256
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BASE_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BONITA_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 10 Nov 2022 21:31:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:16 GMT
RUN mkdir /opt/files
# Thu, 10 Nov 2022 21:31:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 10 Nov 2022 21:31:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_PASSWORD=
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 10 Nov 2022 21:31:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 10 Nov 2022 21:31:26 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 10 Nov 2022 21:31:26 GMT
EXPOSE 8080 9000
# Thu, 10 Nov 2022 21:31:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 10 Nov 2022 21:31:26 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3ecf9c0764240ea4a002e97a93756470158670ab2d476271c5dff63411aba`  
		Last Modified: Thu, 10 Nov 2022 21:32:24 GMT  
		Size: 56.8 MB (56758527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a3561b22a1c5d6d0052ed6e609a9b4f439038a3c9316e4a18d113bccb1cbb`  
		Last Modified: Thu, 10 Nov 2022 21:32:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3521a1d72476ad9583383dfcada876476cbebf359be2854f3719b473260f64`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ecdb4041b3ae0840a5435e5c6d2ae2cf6a480e838b043cd029bc990ebfbbb2`  
		Last Modified: Thu, 10 Nov 2022 21:32:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2977a32ef333556aa544c36b6595d83f2cf92d76f429a58780b327eac6de9aca`  
		Last Modified: Thu, 10 Nov 2022 21:32:12 GMT  
		Size: 3.0 KB (3036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc41606a6fed8126df1e7a47259412bf23cca1aad6619f8bde287a1e2a81`  
		Last Modified: Thu, 10 Nov 2022 21:32:16 GMT  
		Size: 116.7 MB (116690815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2c6540a466d20ce7e64cbabe62163e54d535f2a5f75f8b7dfaae489c50e8e`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:ab6c74c8f8157a5fca98141a6137586c41362da4a2e35a1a7b8e27aeb3d59a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2` - linux; amd64

```console
$ docker pull bonita@sha256:af0b3309cef222dc7bb8eea0171365ce7c1f04c653ce1fcb88946269cbdaa1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183358999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9109ad12339446e49ea0fe59899c0fbc099861b68ba6dfff446717483f9db272`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:10:33 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 05:10:37 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 05:10:38 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 05:10:39 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 05:10:40 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 05:10:41 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 05:10:49 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 05:10:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 05:10:51 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 05:10:51 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 05:10:51 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 05:10:51 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 05:10:51 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f44ece23391fa62ec0b54a5223b0e83bf3afdf487aac2e8bcf40fceafe3c7f9`  
		Last Modified: Sat, 12 Nov 2022 05:11:27 GMT  
		Size: 61.3 MB (61349663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f737142fcee545435fb87aad8ba19c0c5161b2123af22ed53f23cbbe74a40`  
		Last Modified: Sat, 12 Nov 2022 05:11:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03e552725b71e9a3c2d21554036dbc8c8f37d789460fb85a83a2caf824e0a8`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381b9f3f89adb3f9b9d686274b546978dcc1f8be9c09645ca12db9a3c0fa144`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e828375313adaa2ecd577320401dd912202ef128213370630fa123ddf458322`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbec32dd5245f88019c4158f869ef58fdc51e7151d35b1adbcbb4d987469d0`  
		Last Modified: Sat, 12 Nov 2022 05:11:23 GMT  
		Size: 119.2 MB (119193030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ac6aa1740a5547ebbd19730284cda96651ea618939ce1a72b2db0103764307`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:bde00eff2d5e13f1c0f5a0f252e7c53e25c810d4451913d76329abfd16f89f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182510902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afb8eb0b9144f3d0cdcba7e22c5cad653298929ff2c0800dee8831210724443`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:12:26 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:12:30 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:12:31 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:12:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:12:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:33 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:12:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:12:41 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:12:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:12:43 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:12:43 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:12:43 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:12:43 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:12:43 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce4c0a72e6d1f312d742245a673d03cf1c1a40071986286029e0a00a67480f`  
		Last Modified: Sat, 12 Nov 2022 04:13:20 GMT  
		Size: 60.6 MB (60600121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf2b4f26366c9aae2cf0ff0f36b0ac4bf366208f938eeeab3b21f32657639c`  
		Last Modified: Sat, 12 Nov 2022 04:13:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835deb94e6aaa2b983a18fb02dd0f8170a3e79b46ce9d67fe76b9390ccf1a12`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c66d5ecba2c4fc8f635b2b2e3954ef6e3f2a3c9e881e00c59b35ed8f0e7c7b3`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dab80d34b1704dded6340f627700423b28bf8257b13c50a5812a341a71de0c`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab7f4c30d1b1e3a2e766637f44f630946117f6aa4b404086c57031afef18d2`  
		Last Modified: Sat, 12 Nov 2022 04:13:15 GMT  
		Size: 119.2 MB (119192997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60912611891a306ce975f3597861cc95698c4f4831b69483b30193d2fbfe64d4`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:bc646851cea3a34aaeab8a829e05dec0b922b6c5e8f164f1a5388a6c04c5efa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179512965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097c6f360acaa7279b69d25d1ad4db629ebbbcbc5e6745a637f19029edd7bf16`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:33:24 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:33:27 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:33:28 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:33:28 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:33:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:34 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:33:34 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:33:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:33:54 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:33:55 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:33:55 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:33:58 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:33:58 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:33:58 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:33:58 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59594f530089b9a64ebc37b50c12ff83c1569c34d1d31a8d9f8eafd01bc0d8`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 57.5 MB (57508396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfbbf9fbe77af1267d6ef466813e355c78a4b827f69744a76a1178c1165a9c`  
		Last Modified: Sat, 12 Nov 2022 04:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba451e84465bdf445877d0098a73aa0811961f2d4d03eb32f40162e5aeeba26f`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b20935842b33aa0fadf0982a1cc1a4522a21dcc3d7d0062187c68adece9fd`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540c740bc35002c6104e6212b741283455567c9395bbb50870b249cec397295`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717fd7aec4ecaedcffa16c8c06fcfc48e41141994da313ea21f63164fa3d8692`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7709ea2302b6abbd61cdf354155d561cec710e2f3db1efb45fe3bb7803466be8`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:ab6c74c8f8157a5fca98141a6137586c41362da4a2e35a1a7b8e27aeb3d59a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:af0b3309cef222dc7bb8eea0171365ce7c1f04c653ce1fcb88946269cbdaa1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183358999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9109ad12339446e49ea0fe59899c0fbc099861b68ba6dfff446717483f9db272`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:10:33 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 05:10:37 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 05:10:38 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 05:10:39 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 05:10:40 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 05:10:41 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 05:10:49 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 05:10:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 05:10:51 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 05:10:51 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 05:10:51 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 05:10:51 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 05:10:51 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f44ece23391fa62ec0b54a5223b0e83bf3afdf487aac2e8bcf40fceafe3c7f9`  
		Last Modified: Sat, 12 Nov 2022 05:11:27 GMT  
		Size: 61.3 MB (61349663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f737142fcee545435fb87aad8ba19c0c5161b2123af22ed53f23cbbe74a40`  
		Last Modified: Sat, 12 Nov 2022 05:11:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03e552725b71e9a3c2d21554036dbc8c8f37d789460fb85a83a2caf824e0a8`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381b9f3f89adb3f9b9d686274b546978dcc1f8be9c09645ca12db9a3c0fa144`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e828375313adaa2ecd577320401dd912202ef128213370630fa123ddf458322`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbec32dd5245f88019c4158f869ef58fdc51e7151d35b1adbcbb4d987469d0`  
		Last Modified: Sat, 12 Nov 2022 05:11:23 GMT  
		Size: 119.2 MB (119193030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ac6aa1740a5547ebbd19730284cda96651ea618939ce1a72b2db0103764307`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:bde00eff2d5e13f1c0f5a0f252e7c53e25c810d4451913d76329abfd16f89f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182510902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afb8eb0b9144f3d0cdcba7e22c5cad653298929ff2c0800dee8831210724443`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:12:26 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:12:30 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:12:31 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:12:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:12:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:33 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:12:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:12:41 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:12:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:12:43 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:12:43 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:12:43 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:12:43 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:12:43 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce4c0a72e6d1f312d742245a673d03cf1c1a40071986286029e0a00a67480f`  
		Last Modified: Sat, 12 Nov 2022 04:13:20 GMT  
		Size: 60.6 MB (60600121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf2b4f26366c9aae2cf0ff0f36b0ac4bf366208f938eeeab3b21f32657639c`  
		Last Modified: Sat, 12 Nov 2022 04:13:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835deb94e6aaa2b983a18fb02dd0f8170a3e79b46ce9d67fe76b9390ccf1a12`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c66d5ecba2c4fc8f635b2b2e3954ef6e3f2a3c9e881e00c59b35ed8f0e7c7b3`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dab80d34b1704dded6340f627700423b28bf8257b13c50a5812a341a71de0c`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab7f4c30d1b1e3a2e766637f44f630946117f6aa4b404086c57031afef18d2`  
		Last Modified: Sat, 12 Nov 2022 04:13:15 GMT  
		Size: 119.2 MB (119192997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60912611891a306ce975f3597861cc95698c4f4831b69483b30193d2fbfe64d4`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:bc646851cea3a34aaeab8a829e05dec0b922b6c5e8f164f1a5388a6c04c5efa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179512965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097c6f360acaa7279b69d25d1ad4db629ebbbcbc5e6745a637f19029edd7bf16`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:33:24 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:33:27 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:33:28 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:33:28 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:33:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:34 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:33:34 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:33:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:33:54 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:33:55 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:33:55 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:33:58 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:33:58 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:33:58 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:33:58 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59594f530089b9a64ebc37b50c12ff83c1569c34d1d31a8d9f8eafd01bc0d8`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 57.5 MB (57508396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfbbf9fbe77af1267d6ef466813e355c78a4b827f69744a76a1178c1165a9c`  
		Last Modified: Sat, 12 Nov 2022 04:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba451e84465bdf445877d0098a73aa0811961f2d4d03eb32f40162e5aeeba26f`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b20935842b33aa0fadf0982a1cc1a4522a21dcc3d7d0062187c68adece9fd`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540c740bc35002c6104e6212b741283455567c9395bbb50870b249cec397295`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717fd7aec4ecaedcffa16c8c06fcfc48e41141994da313ea21f63164fa3d8692`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7709ea2302b6abbd61cdf354155d561cec710e2f3db1efb45fe3bb7803466be8`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:46ad987086548e5839651d5041f90636d38fc4a66e30bf5bb4295c0e0eee9e77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:7736099b5a0fbd690c9282ed0c65668f24379cd2b0aea81d64022a05fcc291fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235177846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5f4822d7f3a158aa5057883e28e3984b534eb8143176acf341878421824333`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:52:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:52:31 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:52:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:52:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:52:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:52:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:36 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:52:37 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:52:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:52:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:52:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:52:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:52:46 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:52:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:52:47 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:52:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce567665295479c898d7f9293183d345a196c03c51919bb8178a41a48b5189`  
		Last Modified: Tue, 25 Oct 2022 15:54:21 GMT  
		Size: 91.5 MB (91532751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24296c370e3d7d1bc9d7959bc4eb56acc21e565d5b0d18e5eaa0563694b0c3e0`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253985ca492d1beb31f18def10e14718cd7bd77d860f29d633a6fcba03bafd32`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79f052367f73c0fd44c535e0ed2e6de71c184b3fcbb8564ec76e29933ebae8`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 506.3 KB (506347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb3a632b1c91989f258db6dbc1a4fe32ce5500d0230cc8bc0ba1a5149e2ea9`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f373f10e42c90e6c198dc86af4f21cf553ee7625859da5df64ff6613a35c8fc`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d343a7f8a2f5c8e34eca93be022cd5cb2930c854d104aa8259aedc6a96a42`  
		Last Modified: Tue, 25 Oct 2022 15:54:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba0dba1bbc5b46c45ac45acba4b59eb44e633a1a3cba46ee17fdce628172a1`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:88388c1b022ed85f5376df978d4862b89fa75e91cf81b9da500af1d2e3908e0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226655649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fb01229803e98578deb5ae9e8f594f81885ca2794decbedec7dcea2a13183`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 00:59:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:59:42 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 00:59:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 00:59:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 00:59:46 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 26 Oct 2022 00:59:47 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 26 Oct 2022 00:59:48 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 00:59:48 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 26 Oct 2022 00:59:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 26 Oct 2022 00:59:54 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 26 Oct 2022 00:59:54 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 26 Oct 2022 00:59:55 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 00:59:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 00:59:55 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 00:59:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dffde860fbbd42392ff77e38759245966a7182f0139841187bb163042988818`  
		Last Modified: Wed, 26 Oct 2022 01:02:00 GMT  
		Size: 86.0 MB (86017735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e318176d0c45cf1a2a2350640427c957ec3776a87f5f73267ed9a8a07275d283`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d931702069558109778cb8b5766604f7bba0d5751648b05fcdb67392e95e74b`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43476e7c830ff308b935f68f7641882a5c0e2a6ba2dcd9a02f0a96ed239fd455`  
		Last Modified: Wed, 26 Oct 2022 01:01:50 GMT  
		Size: 475.8 KB (475799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece0e86607bb253229446bef9695d91765c4a5091daf19d6266a3de11ed34e11`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de99403106573ed9e00c47b1923fe08b08cbfa879b95785b828796cc470c1481`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10b77d72296b42c9faa55435320dc1823f9702b30ed6b21dadf93f18f99958f`  
		Last Modified: Wed, 26 Oct 2022 01:01:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf370bf521d66fa39c549a560e25bea7556bdc6537541ca1afe64590a472febb`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:5ef4e3a6c96b32ec231f530e059dfe1b71baaa78cf750ab37b77ce2a360a13fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234160943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0875be850095eb8c2e1a31ee88f765296c9b98bf35f7e4c74819045b70cab1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:00:32 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:00:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:00:39 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:00:41 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:43 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:00:45 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:00:45 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:00:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:00:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:00:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:00:57 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:00:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:00:58 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:00:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bf908b740a06082b8cd17325b6597a3ef1380e9b186700b0fd995d958f16e`  
		Last Modified: Tue, 25 Oct 2022 15:03:47 GMT  
		Size: 86.8 MB (86816119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33059b8fceb675324742914a9bee1d0d76a22aa07638a8de985fe581d01f8703`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dcaef92716cfc0a27df29c6b4400bfbb5c016b38b0b198c9bc23afd1f95a`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e4dbce9799a10ec7fb02699ab08e330dce68115b62afc5a8608a8789c870d9`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 475.3 KB (475349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfd48608a926fc9739c766d7212ad37c4e1b10431297e5804efbf57cb6fd41c`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d248f05ade088bc58ecb87d89fd543bc55a5c0e5f50b5b6a4672193188708ea`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e377df32a41bd395185b6a33edd822a7cd31e8bc9f43c65ac8cc97048ed381c7`  
		Last Modified: Tue, 25 Oct 2022 15:03:29 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ace1f942b1e9c2a34bcae77510d4ab73f379b2a3ba7f59d733c2d9be57e7a0e`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:46ad987086548e5839651d5041f90636d38fc4a66e30bf5bb4295c0e0eee9e77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:7736099b5a0fbd690c9282ed0c65668f24379cd2b0aea81d64022a05fcc291fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235177846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5f4822d7f3a158aa5057883e28e3984b534eb8143176acf341878421824333`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:52:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:52:31 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:52:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:52:34 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:52:35 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:35 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:52:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:52:36 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:52:37 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:52:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:52:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:52:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:52:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:52:46 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:52:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:52:47 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:52:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce567665295479c898d7f9293183d345a196c03c51919bb8178a41a48b5189`  
		Last Modified: Tue, 25 Oct 2022 15:54:21 GMT  
		Size: 91.5 MB (91532751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24296c370e3d7d1bc9d7959bc4eb56acc21e565d5b0d18e5eaa0563694b0c3e0`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253985ca492d1beb31f18def10e14718cd7bd77d860f29d633a6fcba03bafd32`  
		Last Modified: Tue, 25 Oct 2022 15:54:09 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79f052367f73c0fd44c535e0ed2e6de71c184b3fcbb8564ec76e29933ebae8`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 506.3 KB (506347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb3a632b1c91989f258db6dbc1a4fe32ce5500d0230cc8bc0ba1a5149e2ea9`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f373f10e42c90e6c198dc86af4f21cf553ee7625859da5df64ff6613a35c8fc`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d343a7f8a2f5c8e34eca93be022cd5cb2930c854d104aa8259aedc6a96a42`  
		Last Modified: Tue, 25 Oct 2022 15:54:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba0dba1bbc5b46c45ac45acba4b59eb44e633a1a3cba46ee17fdce628172a1`  
		Last Modified: Tue, 25 Oct 2022 15:54:07 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:88388c1b022ed85f5376df978d4862b89fa75e91cf81b9da500af1d2e3908e0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226655649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fb01229803e98578deb5ae9e8f594f81885ca2794decbedec7dcea2a13183`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 00:59:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:59:42 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 00:59:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 00:59:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 00:59:46 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 26 Oct 2022 00:59:47 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 00:59:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 26 Oct 2022 00:59:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 26 Oct 2022 00:59:48 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 00:59:48 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 26 Oct 2022 00:59:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 26 Oct 2022 00:59:54 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 26 Oct 2022 00:59:54 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 26 Oct 2022 00:59:55 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 00:59:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 00:59:55 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 00:59:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dffde860fbbd42392ff77e38759245966a7182f0139841187bb163042988818`  
		Last Modified: Wed, 26 Oct 2022 01:02:00 GMT  
		Size: 86.0 MB (86017735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e318176d0c45cf1a2a2350640427c957ec3776a87f5f73267ed9a8a07275d283`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d931702069558109778cb8b5766604f7bba0d5751648b05fcdb67392e95e74b`  
		Last Modified: Wed, 26 Oct 2022 01:01:51 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43476e7c830ff308b935f68f7641882a5c0e2a6ba2dcd9a02f0a96ed239fd455`  
		Last Modified: Wed, 26 Oct 2022 01:01:50 GMT  
		Size: 475.8 KB (475799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece0e86607bb253229446bef9695d91765c4a5091daf19d6266a3de11ed34e11`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de99403106573ed9e00c47b1923fe08b08cbfa879b95785b828796cc470c1481`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10b77d72296b42c9faa55435320dc1823f9702b30ed6b21dadf93f18f99958f`  
		Last Modified: Wed, 26 Oct 2022 01:01:54 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf370bf521d66fa39c549a560e25bea7556bdc6537541ca1afe64590a472febb`  
		Last Modified: Wed, 26 Oct 2022 01:01:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:5ef4e3a6c96b32ec231f530e059dfe1b71baaa78cf750ab37b77ce2a360a13fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234160943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0875be850095eb8c2e1a31ee88f765296c9b98bf35f7e4c74819045b70cab1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:00:32 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:00:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:00:39 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:00:39 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:00:40 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 25 Oct 2022 15:00:41 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 25 Oct 2022 15:00:41 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:00:42 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 25 Oct 2022 15:00:43 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 25 Oct 2022 15:00:45 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:00:45 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 25 Oct 2022 15:00:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 25 Oct 2022 15:00:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 25 Oct 2022 15:00:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 25 Oct 2022 15:00:57 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:00:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:00:58 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:00:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bf908b740a06082b8cd17325b6597a3ef1380e9b186700b0fd995d958f16e`  
		Last Modified: Tue, 25 Oct 2022 15:03:47 GMT  
		Size: 86.8 MB (86816119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33059b8fceb675324742914a9bee1d0d76a22aa07638a8de985fe581d01f8703`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dcaef92716cfc0a27df29c6b4400bfbb5c016b38b0b198c9bc23afd1f95a`  
		Last Modified: Tue, 25 Oct 2022 15:03:24 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e4dbce9799a10ec7fb02699ab08e330dce68115b62afc5a8608a8789c870d9`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 475.3 KB (475349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfd48608a926fc9739c766d7212ad37c4e1b10431297e5804efbf57cb6fd41c`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d248f05ade088bc58ecb87d89fd543bc55a5c0e5f50b5b6a4672193188708ea`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e377df32a41bd395185b6a33edd822a7cd31e8bc9f43c65ac8cc97048ed381c7`  
		Last Modified: Tue, 25 Oct 2022 15:03:29 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ace1f942b1e9c2a34bcae77510d4ab73f379b2a3ba7f59d733c2d9be57e7a0e`  
		Last Modified: Tue, 25 Oct 2022 15:03:21 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:b418388fca7b8c968ebb732007d68c154109f4586bb377b6db7f3b21cd3652f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:89428640a9e65a669dd2d80432a83d4f14fc3ea52f147fb79b9d166ac600834c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232910837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57327096a0152d53428bf600651aa3d02cdb3694163cd8ef3a135b17e15c58e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:53:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:53:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:53:18 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:53:22 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:53:23 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:24 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:53:24 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:53:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:53:40 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:53:40 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:53:41 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:53:41 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:53:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4d444062fb1490dc40701d8201083260f32115730e595fc7eb0533d308187`  
		Last Modified: Tue, 25 Oct 2022 15:55:24 GMT  
		Size: 91.5 MB (91532740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64575146ef008f8318b475f9ac6437b9e84f4f45a626a1c0a2ac042c0a55e5a7`  
		Last Modified: Tue, 25 Oct 2022 15:55:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc81f1ca4a9fa69f8ce85c888642403bc5357e6aa8e5c27303bf9f7c8ffddac9`  
		Last Modified: Tue, 25 Oct 2022 15:55:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb0c1f6517e5d16e967d48e5794a1c1058b6ca4d6306d8a88335b084159337a`  
		Last Modified: Tue, 25 Oct 2022 15:55:09 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2975d5c35bbdd01161a6f82800341af5759c8b1a323e3271cca4eab7723855e0`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab9e4a959c92acae9c3bcbc05fedc30218b0663e3a7f5ceb04467e0d66306ad`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243de80728f9d53ff507070746cf4c92c712b4d44f2ab894390fef71342fcc8`  
		Last Modified: Tue, 25 Oct 2022 15:55:15 GMT  
		Size: 113.7 MB (113727915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94a522f5fdfb28c2e883baf8366e0d084e337ed88db718eabb1ceb650712119`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:539215409c088cfcb37d88ddcd646c8b25c1236ad91f6a20b33faf6640c6e984
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224348182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93cb0763d302538b7abaa14fc82139b687f3ad29338619d420d897a8baabde22`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 01:00:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:00:25 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 01:00:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 01:00:28 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 26 Oct 2022 01:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:30 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 01:00:30 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 26 Oct 2022 01:00:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 26 Oct 2022 01:00:44 GMT
ENV HTTP_API=false
# Wed, 26 Oct 2022 01:00:45 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 01:00:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 01:00:46 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 01:00:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87e4b48be33c3874175426beae7bef698137d1ddd60124338a3ac84767adc60`  
		Last Modified: Wed, 26 Oct 2022 01:02:25 GMT  
		Size: 86.0 MB (86017619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b313f79a8a118790254b764e04d46bc0f62323e99e23fcbba7906fe08bc02`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d958fd260eec0c33924b9c62e4012d7d8e78b0a92b492aeb1ecd4b11264756`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38331e2fea86cd0d9001a29fe93170874e7860b09fea765b59a8e344739bb05c`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 859.6 KB (859577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbd70b5e8b6ae25fa5f4fdd0a87337386aa2a2254122d7edb8fa4cd90a17054`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d0d8b93e75ddc6c93f9ac045e05de138ce023e3b356ef0a44d36ebaffd360`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25031c28db0d261ab6c0772562e3e34d4529292ba5831e0c135ca64ad05d463a`  
		Last Modified: Wed, 26 Oct 2022 01:02:19 GMT  
		Size: 113.7 MB (113727925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea76a40bc6b6863b7451791e765deb70ae5631422a94b24c1a69839b7567a8`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:1c8d0507483f67a146cd92ee71a9932bb7c6d4322c75f804df880c2f03c5dfd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231826002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e64debf4d35b95287c13910032120f63ecd6d1528cd9cb6023e7abc7a6e2da`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:01:50 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:01:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:01:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:01:58 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:01:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:02:00 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:02:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:02:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:02:16 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:02:18 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:02:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:02:20 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:02:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0bd46ad19567c08c1713a7725bc00aed8394fd8f3ed9bec7ce4479c7b86c69`  
		Last Modified: Tue, 25 Oct 2022 15:04:25 GMT  
		Size: 86.8 MB (86816051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee497a65fbc1669cf497d7ff89f1db3a0bced0347b40783fe209d3d89a3b81`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca0ee0d23f6a8f675abb762ed413d8dd07e65f10b9bff344fd67aa25e41b97f`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f272d29db7fb9f929358e96e47a2bf8e985f250fb1f95263cc65ceda4a739`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 831.6 KB (831579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2593595c89246ea872f1210053f7de8f27b8acedefb4457a7555967dfa6c21b`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b956766cd724dc4b950cbc195f0ec3d47ba2afcfac99a559d3768331b07c7`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a965377d658a6e91c602615fed50e102395e8d0f341e60b676cb62f27c69d`  
		Last Modified: Tue, 25 Oct 2022 15:04:19 GMT  
		Size: 113.7 MB (113727947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f50859dcba4b5885bbf6f5f1b214871dfe8ab0be5c20d65e8e4cee31a75d4e`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:b418388fca7b8c968ebb732007d68c154109f4586bb377b6db7f3b21cd3652f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:89428640a9e65a669dd2d80432a83d4f14fc3ea52f147fb79b9d166ac600834c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232910837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57327096a0152d53428bf600651aa3d02cdb3694163cd8ef3a135b17e15c58e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 15:51:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:53:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:53:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:53:18 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:53:22 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:53:22 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:53:23 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:53:23 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:53:24 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:53:24 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:53:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:53:40 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:53:40 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:53:41 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:53:41 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:53:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4d444062fb1490dc40701d8201083260f32115730e595fc7eb0533d308187`  
		Last Modified: Tue, 25 Oct 2022 15:55:24 GMT  
		Size: 91.5 MB (91532740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64575146ef008f8318b475f9ac6437b9e84f4f45a626a1c0a2ac042c0a55e5a7`  
		Last Modified: Tue, 25 Oct 2022 15:55:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc81f1ca4a9fa69f8ce85c888642403bc5357e6aa8e5c27303bf9f7c8ffddac9`  
		Last Modified: Tue, 25 Oct 2022 15:55:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb0c1f6517e5d16e967d48e5794a1c1058b6ca4d6306d8a88335b084159337a`  
		Last Modified: Tue, 25 Oct 2022 15:55:09 GMT  
		Size: 930.5 KB (930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2975d5c35bbdd01161a6f82800341af5759c8b1a323e3271cca4eab7723855e0`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab9e4a959c92acae9c3bcbc05fedc30218b0663e3a7f5ceb04467e0d66306ad`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243de80728f9d53ff507070746cf4c92c712b4d44f2ab894390fef71342fcc8`  
		Last Modified: Tue, 25 Oct 2022 15:55:15 GMT  
		Size: 113.7 MB (113727915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94a522f5fdfb28c2e883baf8366e0d084e337ed88db718eabb1ceb650712119`  
		Last Modified: Tue, 25 Oct 2022 15:55:08 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:539215409c088cfcb37d88ddcd646c8b25c1236ad91f6a20b33faf6640c6e984
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224348182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93cb0763d302538b7abaa14fc82139b687f3ad29338619d420d897a8baabde22`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:58:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 26 Oct 2022 01:00:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:00:25 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 26 Oct 2022 01:00:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 26 Oct 2022 01:00:28 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BONITA_VERSION
# Wed, 26 Oct 2022 01:00:28 GMT
ARG BRANDING_VERSION
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_SHA256
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BASE_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ARG BONITA_URL
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 26 Oct 2022 01:00:29 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 26 Oct 2022 01:00:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 26 Oct 2022 01:00:30 GMT
RUN mkdir /opt/files
# Wed, 26 Oct 2022 01:00:30 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 26 Oct 2022 01:00:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 26 Oct 2022 01:00:44 GMT
ENV HTTP_API=false
# Wed, 26 Oct 2022 01:00:45 GMT
VOLUME [/opt/bonita]
# Wed, 26 Oct 2022 01:00:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 26 Oct 2022 01:00:46 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 01:00:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87e4b48be33c3874175426beae7bef698137d1ddd60124338a3ac84767adc60`  
		Last Modified: Wed, 26 Oct 2022 01:02:25 GMT  
		Size: 86.0 MB (86017619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b313f79a8a118790254b764e04d46bc0f62323e99e23fcbba7906fe08bc02`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d958fd260eec0c33924b9c62e4012d7d8e78b0a92b492aeb1ecd4b11264756`  
		Last Modified: Wed, 26 Oct 2022 01:02:15 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38331e2fea86cd0d9001a29fe93170874e7860b09fea765b59a8e344739bb05c`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 859.6 KB (859577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbd70b5e8b6ae25fa5f4fdd0a87337386aa2a2254122d7edb8fa4cd90a17054`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d0d8b93e75ddc6c93f9ac045e05de138ce023e3b356ef0a44d36ebaffd360`  
		Last Modified: Wed, 26 Oct 2022 01:02:13 GMT  
		Size: 3.3 KB (3304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25031c28db0d261ab6c0772562e3e34d4529292ba5831e0c135ca64ad05d463a`  
		Last Modified: Wed, 26 Oct 2022 01:02:19 GMT  
		Size: 113.7 MB (113727925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea76a40bc6b6863b7451791e765deb70ae5631422a94b24c1a69839b7567a8`  
		Last Modified: Wed, 26 Oct 2022 01:02:14 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1c8d0507483f67a146cd92ee71a9932bb7c6d4322c75f804df880c2f03c5dfd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231826002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e64debf4d35b95287c13910032120f63ecd6d1528cd9cb6023e7abc7a6e2da`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:58:59 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 25 Oct 2022 15:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 15:01:50 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 25 Oct 2022 15:01:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 25 Oct 2022 15:01:56 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BRANDING_VERSION
# Tue, 25 Oct 2022 15:01:56 GMT
ARG BONITA_SHA256
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BASE_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ARG BONITA_URL
# Tue, 25 Oct 2022 15:01:57 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 25 Oct 2022 15:01:58 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:01:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 25 Oct 2022 15:01:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 25 Oct 2022 15:02:00 GMT
RUN mkdir /opt/files
# Tue, 25 Oct 2022 15:02:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 25 Oct 2022 15:02:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 25 Oct 2022 15:02:16 GMT
ENV HTTP_API=false
# Tue, 25 Oct 2022 15:02:18 GMT
VOLUME [/opt/bonita]
# Tue, 25 Oct 2022 15:02:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 25 Oct 2022 15:02:20 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 15:02:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0bd46ad19567c08c1713a7725bc00aed8394fd8f3ed9bec7ce4479c7b86c69`  
		Last Modified: Tue, 25 Oct 2022 15:04:25 GMT  
		Size: 86.8 MB (86816051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee497a65fbc1669cf497d7ff89f1db3a0bced0347b40783fe209d3d89a3b81`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca0ee0d23f6a8f675abb762ed413d8dd07e65f10b9bff344fd67aa25e41b97f`  
		Last Modified: Tue, 25 Oct 2022 15:04:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f272d29db7fb9f929358e96e47a2bf8e985f250fb1f95263cc65ceda4a739`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 831.6 KB (831579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2593595c89246ea872f1210053f7de8f27b8acedefb4457a7555967dfa6c21b`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b956766cd724dc4b950cbc195f0ec3d47ba2afcfac99a559d3768331b07c7`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a965377d658a6e91c602615fed50e102395e8d0f341e60b676cb62f27c69d`  
		Last Modified: Tue, 25 Oct 2022 15:04:19 GMT  
		Size: 113.7 MB (113727947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f50859dcba4b5885bbf6f5f1b214871dfe8ab0be5c20d65e8e4cee31a75d4e`  
		Last Modified: Tue, 25 Oct 2022 15:04:04 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:0f038ccdde32fa4b90a855ec5bb41db8434cfbe432cecbcde8abd01c88b0ad8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:92b3b92dc468cfc22704a83368c85d4758c878808548637ad8401f6ba78e5282
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176177804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a01742b56399308f70d74c2477c82b5f0562160950db295a6adb0b48e8dadf`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:31:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 10 Nov 2022 21:31:12 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 10 Nov 2022 21:31:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 10 Nov 2022 21:31:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BRANDING_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_SHA256
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BASE_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BONITA_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 10 Nov 2022 21:31:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:16 GMT
RUN mkdir /opt/files
# Thu, 10 Nov 2022 21:31:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 10 Nov 2022 21:31:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_PASSWORD=
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 10 Nov 2022 21:31:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 10 Nov 2022 21:31:26 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 10 Nov 2022 21:31:26 GMT
EXPOSE 8080 9000
# Thu, 10 Nov 2022 21:31:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 10 Nov 2022 21:31:26 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3ecf9c0764240ea4a002e97a93756470158670ab2d476271c5dff63411aba`  
		Last Modified: Thu, 10 Nov 2022 21:32:24 GMT  
		Size: 56.8 MB (56758527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a3561b22a1c5d6d0052ed6e609a9b4f439038a3c9316e4a18d113bccb1cbb`  
		Last Modified: Thu, 10 Nov 2022 21:32:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3521a1d72476ad9583383dfcada876476cbebf359be2854f3719b473260f64`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ecdb4041b3ae0840a5435e5c6d2ae2cf6a480e838b043cd029bc990ebfbbb2`  
		Last Modified: Thu, 10 Nov 2022 21:32:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2977a32ef333556aa544c36b6595d83f2cf92d76f429a58780b327eac6de9aca`  
		Last Modified: Thu, 10 Nov 2022 21:32:12 GMT  
		Size: 3.0 KB (3036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc41606a6fed8126df1e7a47259412bf23cca1aad6619f8bde287a1e2a81`  
		Last Modified: Thu, 10 Nov 2022 21:32:16 GMT  
		Size: 116.7 MB (116690815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2c6540a466d20ce7e64cbabe62163e54d535f2a5f75f8b7dfaae489c50e8e`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:0f038ccdde32fa4b90a855ec5bb41db8434cfbe432cecbcde8abd01c88b0ad8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:92b3b92dc468cfc22704a83368c85d4758c878808548637ad8401f6ba78e5282
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176177804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a01742b56399308f70d74c2477c82b5f0562160950db295a6adb0b48e8dadf`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:31:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 10 Nov 2022 21:31:12 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 10 Nov 2022 21:31:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 10 Nov 2022 21:31:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BRANDING_VERSION
# Thu, 10 Nov 2022 21:31:14 GMT
ARG BONITA_SHA256
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BASE_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ARG BONITA_URL
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 10 Nov 2022 21:31:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 10 Nov 2022 21:31:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 10 Nov 2022 21:31:16 GMT
RUN mkdir /opt/files
# Thu, 10 Nov 2022 21:31:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 10 Nov 2022 21:31:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_API_PASSWORD=
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 10 Nov 2022 21:31:25 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 10 Nov 2022 21:31:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 10 Nov 2022 21:31:25 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 10 Nov 2022 21:31:25 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 10 Nov 2022 21:31:26 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 10 Nov 2022 21:31:26 GMT
EXPOSE 8080 9000
# Thu, 10 Nov 2022 21:31:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 10 Nov 2022 21:31:26 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3ecf9c0764240ea4a002e97a93756470158670ab2d476271c5dff63411aba`  
		Last Modified: Thu, 10 Nov 2022 21:32:24 GMT  
		Size: 56.8 MB (56758527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a3561b22a1c5d6d0052ed6e609a9b4f439038a3c9316e4a18d113bccb1cbb`  
		Last Modified: Thu, 10 Nov 2022 21:32:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3521a1d72476ad9583383dfcada876476cbebf359be2854f3719b473260f64`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ecdb4041b3ae0840a5435e5c6d2ae2cf6a480e838b043cd029bc990ebfbbb2`  
		Last Modified: Thu, 10 Nov 2022 21:32:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2977a32ef333556aa544c36b6595d83f2cf92d76f429a58780b327eac6de9aca`  
		Last Modified: Thu, 10 Nov 2022 21:32:12 GMT  
		Size: 3.0 KB (3036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc41606a6fed8126df1e7a47259412bf23cca1aad6619f8bde287a1e2a81`  
		Last Modified: Thu, 10 Nov 2022 21:32:16 GMT  
		Size: 116.7 MB (116690815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2c6540a466d20ce7e64cbabe62163e54d535f2a5f75f8b7dfaae489c50e8e`  
		Last Modified: Thu, 10 Nov 2022 21:32:11 GMT  
		Size: 5.4 KB (5424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:ab6c74c8f8157a5fca98141a6137586c41362da4a2e35a1a7b8e27aeb3d59a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15` - linux; amd64

```console
$ docker pull bonita@sha256:af0b3309cef222dc7bb8eea0171365ce7c1f04c653ce1fcb88946269cbdaa1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183358999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9109ad12339446e49ea0fe59899c0fbc099861b68ba6dfff446717483f9db272`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:10:33 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 05:10:37 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 05:10:38 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 05:10:39 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 05:10:40 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 05:10:41 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 05:10:49 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 05:10:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 05:10:51 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 05:10:51 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 05:10:51 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 05:10:51 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 05:10:51 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f44ece23391fa62ec0b54a5223b0e83bf3afdf487aac2e8bcf40fceafe3c7f9`  
		Last Modified: Sat, 12 Nov 2022 05:11:27 GMT  
		Size: 61.3 MB (61349663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f737142fcee545435fb87aad8ba19c0c5161b2123af22ed53f23cbbe74a40`  
		Last Modified: Sat, 12 Nov 2022 05:11:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03e552725b71e9a3c2d21554036dbc8c8f37d789460fb85a83a2caf824e0a8`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381b9f3f89adb3f9b9d686274b546978dcc1f8be9c09645ca12db9a3c0fa144`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e828375313adaa2ecd577320401dd912202ef128213370630fa123ddf458322`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbec32dd5245f88019c4158f869ef58fdc51e7151d35b1adbcbb4d987469d0`  
		Last Modified: Sat, 12 Nov 2022 05:11:23 GMT  
		Size: 119.2 MB (119193030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ac6aa1740a5547ebbd19730284cda96651ea618939ce1a72b2db0103764307`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:bde00eff2d5e13f1c0f5a0f252e7c53e25c810d4451913d76329abfd16f89f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182510902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afb8eb0b9144f3d0cdcba7e22c5cad653298929ff2c0800dee8831210724443`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:12:26 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:12:30 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:12:31 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:12:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:12:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:33 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:12:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:12:41 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:12:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:12:43 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:12:43 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:12:43 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:12:43 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:12:43 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce4c0a72e6d1f312d742245a673d03cf1c1a40071986286029e0a00a67480f`  
		Last Modified: Sat, 12 Nov 2022 04:13:20 GMT  
		Size: 60.6 MB (60600121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf2b4f26366c9aae2cf0ff0f36b0ac4bf366208f938eeeab3b21f32657639c`  
		Last Modified: Sat, 12 Nov 2022 04:13:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835deb94e6aaa2b983a18fb02dd0f8170a3e79b46ce9d67fe76b9390ccf1a12`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c66d5ecba2c4fc8f635b2b2e3954ef6e3f2a3c9e881e00c59b35ed8f0e7c7b3`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dab80d34b1704dded6340f627700423b28bf8257b13c50a5812a341a71de0c`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab7f4c30d1b1e3a2e766637f44f630946117f6aa4b404086c57031afef18d2`  
		Last Modified: Sat, 12 Nov 2022 04:13:15 GMT  
		Size: 119.2 MB (119192997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60912611891a306ce975f3597861cc95698c4f4831b69483b30193d2fbfe64d4`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:bc646851cea3a34aaeab8a829e05dec0b922b6c5e8f164f1a5388a6c04c5efa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179512965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097c6f360acaa7279b69d25d1ad4db629ebbbcbc5e6745a637f19029edd7bf16`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:33:24 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:33:27 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:33:28 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:33:28 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:33:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:34 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:33:34 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:33:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:33:54 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:33:55 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:33:55 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:33:58 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:33:58 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:33:58 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:33:58 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59594f530089b9a64ebc37b50c12ff83c1569c34d1d31a8d9f8eafd01bc0d8`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 57.5 MB (57508396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfbbf9fbe77af1267d6ef466813e355c78a4b827f69744a76a1178c1165a9c`  
		Last Modified: Sat, 12 Nov 2022 04:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba451e84465bdf445877d0098a73aa0811961f2d4d03eb32f40162e5aeeba26f`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b20935842b33aa0fadf0982a1cc1a4522a21dcc3d7d0062187c68adece9fd`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540c740bc35002c6104e6212b741283455567c9395bbb50870b249cec397295`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717fd7aec4ecaedcffa16c8c06fcfc48e41141994da313ea21f63164fa3d8692`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7709ea2302b6abbd61cdf354155d561cec710e2f3db1efb45fe3bb7803466be8`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:ab6c74c8f8157a5fca98141a6137586c41362da4a2e35a1a7b8e27aeb3d59a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15.0` - linux; amd64

```console
$ docker pull bonita@sha256:af0b3309cef222dc7bb8eea0171365ce7c1f04c653ce1fcb88946269cbdaa1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183358999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9109ad12339446e49ea0fe59899c0fbc099861b68ba6dfff446717483f9db272`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:10:33 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 05:10:37 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 05:10:38 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 05:10:39 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 05:10:40 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 05:10:41 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 05:10:49 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 05:10:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 05:10:51 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 05:10:51 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 05:10:51 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 05:10:51 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 05:10:51 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f44ece23391fa62ec0b54a5223b0e83bf3afdf487aac2e8bcf40fceafe3c7f9`  
		Last Modified: Sat, 12 Nov 2022 05:11:27 GMT  
		Size: 61.3 MB (61349663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f737142fcee545435fb87aad8ba19c0c5161b2123af22ed53f23cbbe74a40`  
		Last Modified: Sat, 12 Nov 2022 05:11:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03e552725b71e9a3c2d21554036dbc8c8f37d789460fb85a83a2caf824e0a8`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381b9f3f89adb3f9b9d686274b546978dcc1f8be9c09645ca12db9a3c0fa144`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e828375313adaa2ecd577320401dd912202ef128213370630fa123ddf458322`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbec32dd5245f88019c4158f869ef58fdc51e7151d35b1adbcbb4d987469d0`  
		Last Modified: Sat, 12 Nov 2022 05:11:23 GMT  
		Size: 119.2 MB (119193030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ac6aa1740a5547ebbd19730284cda96651ea618939ce1a72b2db0103764307`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:bde00eff2d5e13f1c0f5a0f252e7c53e25c810d4451913d76329abfd16f89f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182510902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afb8eb0b9144f3d0cdcba7e22c5cad653298929ff2c0800dee8831210724443`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:12:26 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:12:30 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:12:31 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:12:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:12:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:33 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:12:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:12:41 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:12:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:12:43 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:12:43 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:12:43 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:12:43 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:12:43 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce4c0a72e6d1f312d742245a673d03cf1c1a40071986286029e0a00a67480f`  
		Last Modified: Sat, 12 Nov 2022 04:13:20 GMT  
		Size: 60.6 MB (60600121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf2b4f26366c9aae2cf0ff0f36b0ac4bf366208f938eeeab3b21f32657639c`  
		Last Modified: Sat, 12 Nov 2022 04:13:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835deb94e6aaa2b983a18fb02dd0f8170a3e79b46ce9d67fe76b9390ccf1a12`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c66d5ecba2c4fc8f635b2b2e3954ef6e3f2a3c9e881e00c59b35ed8f0e7c7b3`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dab80d34b1704dded6340f627700423b28bf8257b13c50a5812a341a71de0c`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab7f4c30d1b1e3a2e766637f44f630946117f6aa4b404086c57031afef18d2`  
		Last Modified: Sat, 12 Nov 2022 04:13:15 GMT  
		Size: 119.2 MB (119192997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60912611891a306ce975f3597861cc95698c4f4831b69483b30193d2fbfe64d4`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:bc646851cea3a34aaeab8a829e05dec0b922b6c5e8f164f1a5388a6c04c5efa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179512965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097c6f360acaa7279b69d25d1ad4db629ebbbcbc5e6745a637f19029edd7bf16`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:33:24 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:33:27 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:33:28 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:33:28 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:33:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:34 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:33:34 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:33:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:33:54 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:33:55 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:33:55 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:33:58 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:33:58 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:33:58 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:33:58 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59594f530089b9a64ebc37b50c12ff83c1569c34d1d31a8d9f8eafd01bc0d8`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 57.5 MB (57508396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfbbf9fbe77af1267d6ef466813e355c78a4b827f69744a76a1178c1165a9c`  
		Last Modified: Sat, 12 Nov 2022 04:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba451e84465bdf445877d0098a73aa0811961f2d4d03eb32f40162e5aeeba26f`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b20935842b33aa0fadf0982a1cc1a4522a21dcc3d7d0062187c68adece9fd`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540c740bc35002c6104e6212b741283455567c9395bbb50870b249cec397295`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717fd7aec4ecaedcffa16c8c06fcfc48e41141994da313ea21f63164fa3d8692`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7709ea2302b6abbd61cdf354155d561cec710e2f3db1efb45fe3bb7803466be8`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:ab6c74c8f8157a5fca98141a6137586c41362da4a2e35a1a7b8e27aeb3d59a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:af0b3309cef222dc7bb8eea0171365ce7c1f04c653ce1fcb88946269cbdaa1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183358999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9109ad12339446e49ea0fe59899c0fbc099861b68ba6dfff446717483f9db272`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:10:33 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 05:10:37 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 05:10:38 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 05:10:39 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 05:10:39 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 05:10:40 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 05:10:40 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 05:10:40 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 05:10:41 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 05:10:49 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 05:10:50 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 05:10:50 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 05:10:50 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 05:10:50 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 05:10:51 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 05:10:51 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 05:10:51 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 05:10:51 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 05:10:51 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 05:10:51 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f44ece23391fa62ec0b54a5223b0e83bf3afdf487aac2e8bcf40fceafe3c7f9`  
		Last Modified: Sat, 12 Nov 2022 05:11:27 GMT  
		Size: 61.3 MB (61349663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f737142fcee545435fb87aad8ba19c0c5161b2123af22ed53f23cbbe74a40`  
		Last Modified: Sat, 12 Nov 2022 05:11:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03e552725b71e9a3c2d21554036dbc8c8f37d789460fb85a83a2caf824e0a8`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381b9f3f89adb3f9b9d686274b546978dcc1f8be9c09645ca12db9a3c0fa144`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e828375313adaa2ecd577320401dd912202ef128213370630fa123ddf458322`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbec32dd5245f88019c4158f869ef58fdc51e7151d35b1adbcbb4d987469d0`  
		Last Modified: Sat, 12 Nov 2022 05:11:23 GMT  
		Size: 119.2 MB (119193030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ac6aa1740a5547ebbd19730284cda96651ea618939ce1a72b2db0103764307`  
		Last Modified: Sat, 12 Nov 2022 05:11:16 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:bde00eff2d5e13f1c0f5a0f252e7c53e25c810d4451913d76329abfd16f89f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182510902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afb8eb0b9144f3d0cdcba7e22c5cad653298929ff2c0800dee8831210724443`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:12:26 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:12:30 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:12:31 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:12:32 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:12:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:12:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:12:33 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:12:33 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:12:41 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:12:42 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:12:42 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:12:43 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:12:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:12:43 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:12:43 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:12:43 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:12:43 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:12:43 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce4c0a72e6d1f312d742245a673d03cf1c1a40071986286029e0a00a67480f`  
		Last Modified: Sat, 12 Nov 2022 04:13:20 GMT  
		Size: 60.6 MB (60600121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf2b4f26366c9aae2cf0ff0f36b0ac4bf366208f938eeeab3b21f32657639c`  
		Last Modified: Sat, 12 Nov 2022 04:13:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835deb94e6aaa2b983a18fb02dd0f8170a3e79b46ce9d67fe76b9390ccf1a12`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c66d5ecba2c4fc8f635b2b2e3954ef6e3f2a3c9e881e00c59b35ed8f0e7c7b3`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dab80d34b1704dded6340f627700423b28bf8257b13c50a5812a341a71de0c`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 3.0 KB (3044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab7f4c30d1b1e3a2e766637f44f630946117f6aa4b404086c57031afef18d2`  
		Last Modified: Sat, 12 Nov 2022 04:13:15 GMT  
		Size: 119.2 MB (119192997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60912611891a306ce975f3597861cc95698c4f4831b69483b30193d2fbfe64d4`  
		Last Modified: Sat, 12 Nov 2022 04:13:10 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:bc646851cea3a34aaeab8a829e05dec0b922b6c5e8f164f1a5388a6c04c5efa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179512965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097c6f360acaa7279b69d25d1ad4db629ebbbcbc5e6745a637f19029edd7bf16`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:08 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 12 Nov 2022 04:33:24 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Sat, 12 Nov 2022 04:33:27 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 12 Nov 2022 04:33:28 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Sat, 12 Nov 2022 04:33:28 GMT
ARG BONITA_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BRANDING_VERSION
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BONITA_SHA256
# Sat, 12 Nov 2022 04:33:29 GMT
ARG BASE_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ARG BONITA_URL
# Sat, 12 Nov 2022 04:33:30 GMT
ENV BONITA_VERSION=7.15.0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BRANDING_VERSION=2022.2-u0
# Sat, 12 Nov 2022 04:33:31 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Sat, 12 Nov 2022 04:33:32 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 12 Nov 2022 04:33:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Sat, 12 Nov 2022 04:33:34 GMT
RUN mkdir /opt/files
# Sat, 12 Nov 2022 04:33:34 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Sat, 12 Nov 2022 04:33:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API=false
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_USERNAME=http-api
# Sat, 12 Nov 2022 04:33:54 GMT
ENV HTTP_API_PASSWORD=
# Sat, 12 Nov 2022 04:33:54 GMT
ENV MONITORING_USERNAME=monitoring
# Sat, 12 Nov 2022 04:33:55 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Sat, 12 Nov 2022 04:33:55 GMT
ENV JMX_REMOTE_ACCESS=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Sat, 12 Nov 2022 04:33:56 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Sat, 12 Nov 2022 04:33:57 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Sat, 12 Nov 2022 04:33:58 GMT
ENV HTTP_MAX_THREADS=20
# Sat, 12 Nov 2022 04:33:58 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Sat, 12 Nov 2022 04:33:58 GMT
EXPOSE 8080 9000
# Sat, 12 Nov 2022 04:33:58 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59594f530089b9a64ebc37b50c12ff83c1569c34d1d31a8d9f8eafd01bc0d8`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 57.5 MB (57508396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfbbf9fbe77af1267d6ef466813e355c78a4b827f69744a76a1178c1165a9c`  
		Last Modified: Sat, 12 Nov 2022 04:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba451e84465bdf445877d0098a73aa0811961f2d4d03eb32f40162e5aeeba26f`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b20935842b33aa0fadf0982a1cc1a4522a21dcc3d7d0062187c68adece9fd`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540c740bc35002c6104e6212b741283455567c9395bbb50870b249cec397295`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717fd7aec4ecaedcffa16c8c06fcfc48e41141994da313ea21f63164fa3d8692`  
		Last Modified: Sat, 12 Nov 2022 04:35:11 GMT  
		Size: 119.2 MB (119192984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7709ea2302b6abbd61cdf354155d561cec710e2f3db1efb45fe3bb7803466be8`  
		Last Modified: Sat, 12 Nov 2022 04:34:55 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
