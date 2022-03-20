<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.4`](#bonita7114)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:14c134aca33da365fb3afaa2ef0bfc9a216327f4af1ba5f84f718828b9d1d19e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:0a5df04fdf9e2518814eabb4c4bb3616638b216c6dc23173bd2b20cae8700085
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237364118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d18a4c0a52de08e58755248a78dc6005cbb66942c98f06af6a504fc23cf8ae`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:33:12 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:33:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:33:49 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 22:34:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 22:34:17 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:34:17 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 22:34:22 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 22:34:23 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 22:34:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 22:34:25 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:34:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:34:25 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:34:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243b914b9e4b6fb7ac97f6985856105df397ebe953a46a891d3fb61e19cd188`  
		Last Modified: Sat, 19 Mar 2022 22:35:54 GMT  
		Size: 93.7 MB (93652268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c137b851e3462a6945dd8eba41e1c5d25719ead032e2a0b5f2ec5246218e6d`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6bd5a2ca725536cdf2adb96200b6c1e2e06302b461f5697abbcde1daefa5b`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb82ac7fa955532c88d7a17213ea673acdde2093ec391b04a4e7d852920ea00`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 577.0 KB (576968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933e83e7c77c7103082d620ca9e2efe0613e49ab34b0a5a188f1b68fa9f7a569`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda0434e279fc7a6bed15623d6cffc6470f6dc6f2b2f6468b72605a8d594e344`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34a2a49687acf914d45f77967952dc9ef09d6835439713e5061edadabb451c`  
		Last Modified: Sat, 19 Mar 2022 22:36:09 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf6410c63fc3634c4a8ff616843c05cafe9e5b1cd1af15f2815cb537ea9a31f`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:f664c5ae3a0d1d0d6556109b5912e173dbdad1aae70f0c89aa76c403cfc79b16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226465717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37840f7b36e1ea8d3cc1eb484918408a0a7c80694e498a9624403ec6b2779da5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:06:55 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:06:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:07:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:07:39 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:08:11 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:08:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:08:13 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:08:14 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:08:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 15:08:16 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 15:08:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 15:08:18 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:19 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:08:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:21 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 15:08:22 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:08:24 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 15:08:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 15:08:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 15:08:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 15:08:32 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:08:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:08:34 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:08:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6aca795d67851a5bf64ff69de8a2c846040a785e02ab939c669ea1259dead`  
		Last Modified: Sat, 19 Mar 2022 15:11:16 GMT  
		Size: 85.8 MB (85763563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bdcf2d35ac4a0024417899c05e98131a4fff9dc84f1e8c8adc753bdce04155`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8ec78bd0d33bfd948482e9fddfc7b40d51477334e11b6fb2e7ef30e6edb77`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7bb9b39c93dd2e07a5372e3777c60cb0580fa34e0c509de2eff55931bdda02`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 546.9 KB (546945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6a905429eeab80d97e3d0628638e40ba16452b559eb12908873a93a91a3e19`  
		Last Modified: Sat, 19 Mar 2022 15:11:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4b9a3fc49d78b5e0b3831ecbceff18387baa0c173e82a7701578c1bd596185`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 6.9 KB (6918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c8577ef4db2696b862301023b268b85368ef6fcb21d3769c06a9a13fd5bcf`  
		Last Modified: Sat, 19 Mar 2022 15:11:39 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55f445dd268c9ca2b9a9d3fd0b8821f0a0fd2cfec6e249e708eeec06cdb2503`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:c833e7f91287c1f5278fae277f9e5c578f23343164d1e650008b3e410e16384d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233968471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d919663177257a141b27a779eee211f7bca2ffbc1f5dc8d79e150b12cfb0c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:49:46 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:49:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:50:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:50:32 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:52:31 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:52:34 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:52:36 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:52:38 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:52:41 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 20:52:42 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 20:52:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 20:52:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:52:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:53 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 20:52:59 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:52:59 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 20:53:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 20:53:18 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 20:53:22 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 20:53:24 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:53:26 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:53:27 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:53:28 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29745dd35ee1f69790cb70dafe2654f253a2638e23c28c77381c2a35be5ae34`  
		Last Modified: Sat, 19 Mar 2022 20:59:23 GMT  
		Size: 86.6 MB (86557393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81968045c994cb7690d1dc9d02c0dafbd65aa7250aa87e3ecb5a33d1f6873a`  
		Last Modified: Sat, 19 Mar 2022 20:59:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e298445fac0e7aca27b8ba8df16b18493ea21a96401f4545613ffd08bcc7c7a1`  
		Last Modified: Sat, 19 Mar 2022 20:59:08 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0bed89b849d63e13572d4bd1f077ac7051d8690ed5f7b2a7ee9f31235c407a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 546.8 KB (546771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6809331661c2785e9c54575fb950fb7978d450c5086c859db31604e5b79b58d1`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4731e00bf5db007aa911c27ad45121ec04a668928cd8a3e4ea8e7e8022f22f`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e63959ee9c0d9f76fdddb46152c725ee56be5cd78f916a1b217b72d8149f686`  
		Last Modified: Sat, 19 Mar 2022 20:59:43 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddec700f67833da011d3636ac47dd284f8ffe607f1ebe5f3f8baa77667774a78`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:1dc812cf6152a1dbd7dd664e0764032b903cc57c50cff56b29cd4aca4225acd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:b8b90f3f8aa8a5a5a0ec94c45447c20d7e2653088cd2f92fadc0fc1adbdfe9c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235101881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d1ac77f073ff34cd4af6e8870392ef73eb84279d0aeb4e35641c72b1ae3d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:34:48 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:34:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:35:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:35:07 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 22:35:08 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:09 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:35:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 22:35:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 22:35:18 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 22:35:19 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:35:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:35:19 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:35:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918014104c9ad49400ad5b9cc91d4bcbae82a73fa5abc7a409bf899c6c43f707`  
		Last Modified: Sat, 19 Mar 2022 22:36:36 GMT  
		Size: 93.7 MB (93654889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dbdd5fbdd128de63982a3bcd426031fd93f653efb545091ac58b78a211fe`  
		Last Modified: Sat, 19 Mar 2022 22:36:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b04accad0ea54945a94640fe15c4f18217ac339546430605562903bb6e198c`  
		Last Modified: Sat, 19 Mar 2022 22:36:23 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf332606cb830b506954d33ba501b217b0cf296e237e53ef52a6a9a64c442`  
		Last Modified: Sat, 19 Mar 2022 22:36:22 GMT  
		Size: 1.0 MB (1003224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212fc94ac887dd5a2399140898860c0a998fe2df050fc6e32930fee44eb331d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea58fb34b6055f277ccc1d770336f1a956999418f8c74dcac36d843e5b416d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24ddcab601ff797ff8b88340a09e3597f00209e58763e8cf7ed883c7c7dcb87`  
		Last Modified: Sat, 19 Mar 2022 22:36:28 GMT  
		Size: 113.7 MB (113727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c310e4514d6b20246d217eb5e9eb415ba672947ac5986dff90d60de6cee91c`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8145813d259caf6cd0bea5d1927b07af9b65099efde705c1b7dc4b12dc186c85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224156613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282818f0e70e12d2041d5851adc6e578279aaaed15d0a8744828bf7dc42eefed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:09:07 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:09:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:09:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:09:55 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:09:56 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:09:57 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:09:58 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:09:59 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:10:00 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 15:10:01 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 15:10:02 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 15:10:03 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:10:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:06 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:10:08 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 15:10:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 15:10:29 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 15:10:29 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:10:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:10:31 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:10:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3433408c5fc7f4ae638ee2b5297e626eccb6ef1eaa854483eaa88fe9452b9`  
		Last Modified: Sat, 19 Mar 2022 15:12:08 GMT  
		Size: 85.8 MB (85763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf766653b0804c4ca85b92cc0c0069fac5a3f16d050f228364daa9898cdddc`  
		Last Modified: Sat, 19 Mar 2022 15:11:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faef7cbb4cb2bf00d122900c6fc72a76a1c4ce7e507619ce147f81ef8541dd2`  
		Last Modified: Sat, 19 Mar 2022 15:11:57 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708c338db08b4e85061950c8cb417d1fdd8d11ab132c8869662712a9d49a856`  
		Last Modified: Sat, 19 Mar 2022 15:11:55 GMT  
		Size: 929.4 KB (929409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ab77260b346ebc4ffb2b67788f195a531157a6a926db586e202224550f95b5`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a15c093ce6465bc4b31ce2c94333e202d3a124194d56bb99438c8074746c3c`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0df29d03ead5b114014be21794a723b2a019942d32b8d108fe3f1f2de09ff`  
		Last Modified: Sat, 19 Mar 2022 15:12:12 GMT  
		Size: 113.7 MB (113727850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c4162cb8595bb82ce1922c26bc251eadd27b261925942c84f067f35057191`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:0c8c69d7af8f945591a5d089408490bf52d5bc01ddafc64b7143d5ec6676a8ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231634930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7996e14d3d401d9e6a086fdc28917a40774b46df8ec09f0dd2d332cf566df8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:56:02 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:56:12 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:57:00 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:57:03 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:57:07 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:57:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:57:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:57:17 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:57:19 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 20:57:21 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 20:57:22 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 20:57:25 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:57:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:36 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:57:37 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 20:57:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 20:58:01 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 20:58:07 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:58:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:58:14 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54998de650aec3ff8c87077551a8a8dedbac826f959645af516a214758030de1`  
		Last Modified: Sat, 19 Mar 2022 21:00:18 GMT  
		Size: 86.6 MB (86557500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80861eb3c1c18c4914806cea4a42cc6605837eb735445fe587096738b931ba`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3e83293caa8f19217184082aaf48f054162fd676b0bfe80c811db04b5fa07`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172e62718fccbad62107b4fe7fd7a9a97a92e26d79914dbc2cd2ce19c1ae3a3e`  
		Last Modified: Sat, 19 Mar 2022 21:00:01 GMT  
		Size: 904.2 KB (904217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ad91e85241ec6b752c76025976f23d679c8eda783616cb3d8830044dcb21a`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaebf6593ed9f193fbd8172caa14b34ddf91ceab1a3dc48c01ad9e695794966`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d1d821c92f5f66422e0625adaed7d15289260431916f065c873a51902db85`  
		Last Modified: Sat, 19 Mar 2022 21:00:10 GMT  
		Size: 113.7 MB (113727951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7730acde910ffb0b1920533e60561ebf0826b19c5d57baa84709e782722f8539`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:1dc812cf6152a1dbd7dd664e0764032b903cc57c50cff56b29cd4aca4225acd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:b8b90f3f8aa8a5a5a0ec94c45447c20d7e2653088cd2f92fadc0fc1adbdfe9c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235101881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d1ac77f073ff34cd4af6e8870392ef73eb84279d0aeb4e35641c72b1ae3d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:34:48 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:34:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:35:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:35:07 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 22:35:08 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:09 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:35:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 22:35:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 22:35:18 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 22:35:19 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:35:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:35:19 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:35:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918014104c9ad49400ad5b9cc91d4bcbae82a73fa5abc7a409bf899c6c43f707`  
		Last Modified: Sat, 19 Mar 2022 22:36:36 GMT  
		Size: 93.7 MB (93654889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dbdd5fbdd128de63982a3bcd426031fd93f653efb545091ac58b78a211fe`  
		Last Modified: Sat, 19 Mar 2022 22:36:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b04accad0ea54945a94640fe15c4f18217ac339546430605562903bb6e198c`  
		Last Modified: Sat, 19 Mar 2022 22:36:23 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf332606cb830b506954d33ba501b217b0cf296e237e53ef52a6a9a64c442`  
		Last Modified: Sat, 19 Mar 2022 22:36:22 GMT  
		Size: 1.0 MB (1003224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212fc94ac887dd5a2399140898860c0a998fe2df050fc6e32930fee44eb331d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea58fb34b6055f277ccc1d770336f1a956999418f8c74dcac36d843e5b416d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24ddcab601ff797ff8b88340a09e3597f00209e58763e8cf7ed883c7c7dcb87`  
		Last Modified: Sat, 19 Mar 2022 22:36:28 GMT  
		Size: 113.7 MB (113727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c310e4514d6b20246d217eb5e9eb415ba672947ac5986dff90d60de6cee91c`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8145813d259caf6cd0bea5d1927b07af9b65099efde705c1b7dc4b12dc186c85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224156613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282818f0e70e12d2041d5851adc6e578279aaaed15d0a8744828bf7dc42eefed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:09:07 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:09:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:09:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:09:55 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:09:56 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:09:57 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:09:58 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:09:59 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:10:00 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 15:10:01 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 15:10:02 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 15:10:03 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:10:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:06 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:10:08 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 15:10:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 15:10:29 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 15:10:29 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:10:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:10:31 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:10:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3433408c5fc7f4ae638ee2b5297e626eccb6ef1eaa854483eaa88fe9452b9`  
		Last Modified: Sat, 19 Mar 2022 15:12:08 GMT  
		Size: 85.8 MB (85763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf766653b0804c4ca85b92cc0c0069fac5a3f16d050f228364daa9898cdddc`  
		Last Modified: Sat, 19 Mar 2022 15:11:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faef7cbb4cb2bf00d122900c6fc72a76a1c4ce7e507619ce147f81ef8541dd2`  
		Last Modified: Sat, 19 Mar 2022 15:11:57 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708c338db08b4e85061950c8cb417d1fdd8d11ab132c8869662712a9d49a856`  
		Last Modified: Sat, 19 Mar 2022 15:11:55 GMT  
		Size: 929.4 KB (929409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ab77260b346ebc4ffb2b67788f195a531157a6a926db586e202224550f95b5`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a15c093ce6465bc4b31ce2c94333e202d3a124194d56bb99438c8074746c3c`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0df29d03ead5b114014be21794a723b2a019942d32b8d108fe3f1f2de09ff`  
		Last Modified: Sat, 19 Mar 2022 15:12:12 GMT  
		Size: 113.7 MB (113727850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c4162cb8595bb82ce1922c26bc251eadd27b261925942c84f067f35057191`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:0c8c69d7af8f945591a5d089408490bf52d5bc01ddafc64b7143d5ec6676a8ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231634930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7996e14d3d401d9e6a086fdc28917a40774b46df8ec09f0dd2d332cf566df8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:56:02 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:56:12 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:57:00 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:57:03 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:57:07 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:57:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:57:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:57:17 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:57:19 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 20:57:21 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 20:57:22 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 20:57:25 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:57:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:36 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:57:37 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 20:57:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 20:58:01 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 20:58:07 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:58:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:58:14 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54998de650aec3ff8c87077551a8a8dedbac826f959645af516a214758030de1`  
		Last Modified: Sat, 19 Mar 2022 21:00:18 GMT  
		Size: 86.6 MB (86557500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80861eb3c1c18c4914806cea4a42cc6605837eb735445fe587096738b931ba`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3e83293caa8f19217184082aaf48f054162fd676b0bfe80c811db04b5fa07`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172e62718fccbad62107b4fe7fd7a9a97a92e26d79914dbc2cd2ce19c1ae3a3e`  
		Last Modified: Sat, 19 Mar 2022 21:00:01 GMT  
		Size: 904.2 KB (904217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ad91e85241ec6b752c76025976f23d679c8eda783616cb3d8830044dcb21a`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaebf6593ed9f193fbd8172caa14b34ddf91ceab1a3dc48c01ad9e695794966`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d1d821c92f5f66422e0625adaed7d15289260431916f065c873a51902db85`  
		Last Modified: Sat, 19 Mar 2022 21:00:10 GMT  
		Size: 113.7 MB (113727951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7730acde910ffb0b1920533e60561ebf0826b19c5d57baa84709e782722f8539`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:b09aabe5e53eef543e04b1e620854908090a269a7e3dd8dd906d17ac58efd8a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:3d56dc5956fc937138f8b67bce7a718960256ba23dc047867b4851d49609f56a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234296488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e63835c77f553cd49f6fdad885df3e8efed4e7226e427de48648bb2ef8d606`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:33:12 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:33:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:33:49 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:33:49 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 22:33:50 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 22:33:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 22:33:51 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:33:51 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 22:33:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 22:33:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 22:33:58 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 22:33:58 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:33:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:33:59 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:33:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243b914b9e4b6fb7ac97f6985856105df397ebe953a46a891d3fb61e19cd188`  
		Last Modified: Sat, 19 Mar 2022 22:35:54 GMT  
		Size: 93.7 MB (93652268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c137b851e3462a6945dd8eba41e1c5d25719ead032e2a0b5f2ec5246218e6d`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6bd5a2ca725536cdf2adb96200b6c1e2e06302b461f5697abbcde1daefa5b`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb82ac7fa955532c88d7a17213ea673acdde2093ec391b04a4e7d852920ea00`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 577.0 KB (576968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f682cde06a7aa95480ac5dc7cc95fc8c9696db138d42db9fc09cd573f66389`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51084112012e02760c4ba1429a290ad3d4e152cd65923556149e9d01184e756a`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 6.9 KB (6892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd0f2bbec3d62ca540ba900370ff14e55c04d3a61644fef5081feaca3b64ff`  
		Last Modified: Sat, 19 Mar 2022 22:35:44 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de1b0587490a6bc1f260a6c6c2ed86c3bbce41e10b43398410d48aa0f1028d8`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b732258ad4d0545519476ef1838d564873f7bbc6303d48ba31860b15fa1c216d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223398092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5b18a2b27fc0537123084fcd1dd6be5b6b456db72101e1ddf4055b9870f193c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:06:55 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:06:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:07:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:07:39 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:07:40 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:07:41 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:07:42 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:07:43 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 15:07:44 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 15:07:45 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 15:07:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:07:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 15:07:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 15:07:49 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:07:51 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 15:07:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 15:07:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 15:07:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 15:07:59 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:08:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:08:01 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:08:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6aca795d67851a5bf64ff69de8a2c846040a785e02ab939c669ea1259dead`  
		Last Modified: Sat, 19 Mar 2022 15:11:16 GMT  
		Size: 85.8 MB (85763563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bdcf2d35ac4a0024417899c05e98131a4fff9dc84f1e8c8adc753bdce04155`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8ec78bd0d33bfd948482e9fddfc7b40d51477334e11b6fb2e7ef30e6edb77`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7bb9b39c93dd2e07a5372e3777c60cb0580fa34e0c509de2eff55931bdda02`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 546.9 KB (546945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8269e71ec2c56fcbeb374291ab3b6cbd9800ca42d5ce17bbb96b58ec87a784e`  
		Last Modified: Sat, 19 Mar 2022 15:11:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17061a1ecac089b349eef6f326687a930af6cc29437b84106fba66deb2ec1275`  
		Last Modified: Sat, 19 Mar 2022 15:11:02 GMT  
		Size: 6.9 KB (6868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d703a1843771d417512570ca8adaab6262cec33aa8b30a723924e76adf89c85a`  
		Last Modified: Sat, 19 Mar 2022 15:11:14 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526d4ff3aec4aafb383c962346282b8357e16cebe913ad0ec73c09e25ecf97e`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:d16ea974e04bd4f761f67994ccc5d5624979db582d507c2958d3f870fbab3f88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230900848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9ef5c8715617b7a80a200ac195558cb116f45f37925d8739f3603215b5021e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:49:46 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:49:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:50:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:50:32 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:50:35 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:50:40 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:50:43 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:50:45 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 20:50:51 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 20:51:03 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 20:51:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:51:24 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 20:51:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 20:51:39 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:51:40 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 20:51:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 20:51:58 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 20:52:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 20:52:05 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:52:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:52:09 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:52:12 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29745dd35ee1f69790cb70dafe2654f253a2638e23c28c77381c2a35be5ae34`  
		Last Modified: Sat, 19 Mar 2022 20:59:23 GMT  
		Size: 86.6 MB (86557393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81968045c994cb7690d1dc9d02c0dafbd65aa7250aa87e3ecb5a33d1f6873a`  
		Last Modified: Sat, 19 Mar 2022 20:59:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e298445fac0e7aca27b8ba8df16b18493ea21a96401f4545613ffd08bcc7c7a1`  
		Last Modified: Sat, 19 Mar 2022 20:59:08 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0bed89b849d63e13572d4bd1f077ac7051d8690ed5f7b2a7ee9f31235c407a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 546.8 KB (546771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc57ec54343963dbbc5c48b04500239581d1365e6db96cefe43e2e8ed21e8e`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af31894a70c1b8382c27ee2315c3dd303a7f07fd2d75cc4460cf168169eff9a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9689812f93fa2920862b8e121c3ce42e84f83176e16bc32c4a1d8b820eae6a3e`  
		Last Modified: Sat, 19 Mar 2022 20:59:13 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bee7cf5f74b0357e0a79f4f64270f610ef989226329b53084744dc5da4ae8a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:b09aabe5e53eef543e04b1e620854908090a269a7e3dd8dd906d17ac58efd8a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:3d56dc5956fc937138f8b67bce7a718960256ba23dc047867b4851d49609f56a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234296488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e63835c77f553cd49f6fdad885df3e8efed4e7226e427de48648bb2ef8d606`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:33:12 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:33:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:33:49 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:33:49 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 22:33:50 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:33:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 22:33:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 22:33:51 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:33:51 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 22:33:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 22:33:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 22:33:58 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 22:33:58 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:33:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:33:59 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:33:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243b914b9e4b6fb7ac97f6985856105df397ebe953a46a891d3fb61e19cd188`  
		Last Modified: Sat, 19 Mar 2022 22:35:54 GMT  
		Size: 93.7 MB (93652268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c137b851e3462a6945dd8eba41e1c5d25719ead032e2a0b5f2ec5246218e6d`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6bd5a2ca725536cdf2adb96200b6c1e2e06302b461f5697abbcde1daefa5b`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb82ac7fa955532c88d7a17213ea673acdde2093ec391b04a4e7d852920ea00`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 577.0 KB (576968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f682cde06a7aa95480ac5dc7cc95fc8c9696db138d42db9fc09cd573f66389`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51084112012e02760c4ba1429a290ad3d4e152cd65923556149e9d01184e756a`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 6.9 KB (6892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd0f2bbec3d62ca540ba900370ff14e55c04d3a61644fef5081feaca3b64ff`  
		Last Modified: Sat, 19 Mar 2022 22:35:44 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de1b0587490a6bc1f260a6c6c2ed86c3bbce41e10b43398410d48aa0f1028d8`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b732258ad4d0545519476ef1838d564873f7bbc6303d48ba31860b15fa1c216d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223398092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5b18a2b27fc0537123084fcd1dd6be5b6b456db72101e1ddf4055b9870f193c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:06:55 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:06:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:07:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:07:39 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:07:40 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:07:41 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:07:42 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:07:43 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 15:07:44 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 15:07:45 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 15:07:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:07:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 15:07:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 15:07:49 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:07:51 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 15:07:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 15:07:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 15:07:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 15:07:59 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:08:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:08:01 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:08:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6aca795d67851a5bf64ff69de8a2c846040a785e02ab939c669ea1259dead`  
		Last Modified: Sat, 19 Mar 2022 15:11:16 GMT  
		Size: 85.8 MB (85763563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bdcf2d35ac4a0024417899c05e98131a4fff9dc84f1e8c8adc753bdce04155`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8ec78bd0d33bfd948482e9fddfc7b40d51477334e11b6fb2e7ef30e6edb77`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7bb9b39c93dd2e07a5372e3777c60cb0580fa34e0c509de2eff55931bdda02`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 546.9 KB (546945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8269e71ec2c56fcbeb374291ab3b6cbd9800ca42d5ce17bbb96b58ec87a784e`  
		Last Modified: Sat, 19 Mar 2022 15:11:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17061a1ecac089b349eef6f326687a930af6cc29437b84106fba66deb2ec1275`  
		Last Modified: Sat, 19 Mar 2022 15:11:02 GMT  
		Size: 6.9 KB (6868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d703a1843771d417512570ca8adaab6262cec33aa8b30a723924e76adf89c85a`  
		Last Modified: Sat, 19 Mar 2022 15:11:14 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526d4ff3aec4aafb383c962346282b8357e16cebe913ad0ec73c09e25ecf97e`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:d16ea974e04bd4f761f67994ccc5d5624979db582d507c2958d3f870fbab3f88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230900848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9ef5c8715617b7a80a200ac195558cb116f45f37925d8739f3603215b5021e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:49:46 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:49:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:50:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:50:32 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:50:35 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:50:40 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:50:43 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:50:45 GMT
ENV BONITA_VERSION=7.11.4
# Sat, 19 Mar 2022 20:50:51 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Sat, 19 Mar 2022 20:51:03 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 20:51:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:51:24 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Sat, 19 Mar 2022 20:51:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 20:51:39 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:51:40 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Sat, 19 Mar 2022 20:51:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Sat, 19 Mar 2022 20:51:58 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 20:52:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 20:52:05 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:52:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:52:09 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:52:12 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29745dd35ee1f69790cb70dafe2654f253a2638e23c28c77381c2a35be5ae34`  
		Last Modified: Sat, 19 Mar 2022 20:59:23 GMT  
		Size: 86.6 MB (86557393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81968045c994cb7690d1dc9d02c0dafbd65aa7250aa87e3ecb5a33d1f6873a`  
		Last Modified: Sat, 19 Mar 2022 20:59:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e298445fac0e7aca27b8ba8df16b18493ea21a96401f4545613ffd08bcc7c7a1`  
		Last Modified: Sat, 19 Mar 2022 20:59:08 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0bed89b849d63e13572d4bd1f077ac7051d8690ed5f7b2a7ee9f31235c407a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 546.8 KB (546771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc57ec54343963dbbc5c48b04500239581d1365e6db96cefe43e2e8ed21e8e`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af31894a70c1b8382c27ee2315c3dd303a7f07fd2d75cc4460cf168169eff9a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9689812f93fa2920862b8e121c3ce42e84f83176e16bc32c4a1d8b820eae6a3e`  
		Last Modified: Sat, 19 Mar 2022 20:59:13 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bee7cf5f74b0357e0a79f4f64270f610ef989226329b53084744dc5da4ae8a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:14c134aca33da365fb3afaa2ef0bfc9a216327f4af1ba5f84f718828b9d1d19e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:0a5df04fdf9e2518814eabb4c4bb3616638b216c6dc23173bd2b20cae8700085
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237364118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d18a4c0a52de08e58755248a78dc6005cbb66942c98f06af6a504fc23cf8ae`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:33:12 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:33:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:33:49 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 22:34:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 22:34:17 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:34:17 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 22:34:22 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 22:34:23 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 22:34:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 22:34:25 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:34:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:34:25 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:34:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243b914b9e4b6fb7ac97f6985856105df397ebe953a46a891d3fb61e19cd188`  
		Last Modified: Sat, 19 Mar 2022 22:35:54 GMT  
		Size: 93.7 MB (93652268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c137b851e3462a6945dd8eba41e1c5d25719ead032e2a0b5f2ec5246218e6d`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6bd5a2ca725536cdf2adb96200b6c1e2e06302b461f5697abbcde1daefa5b`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb82ac7fa955532c88d7a17213ea673acdde2093ec391b04a4e7d852920ea00`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 577.0 KB (576968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933e83e7c77c7103082d620ca9e2efe0613e49ab34b0a5a188f1b68fa9f7a569`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda0434e279fc7a6bed15623d6cffc6470f6dc6f2b2f6468b72605a8d594e344`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34a2a49687acf914d45f77967952dc9ef09d6835439713e5061edadabb451c`  
		Last Modified: Sat, 19 Mar 2022 22:36:09 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf6410c63fc3634c4a8ff616843c05cafe9e5b1cd1af15f2815cb537ea9a31f`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:f664c5ae3a0d1d0d6556109b5912e173dbdad1aae70f0c89aa76c403cfc79b16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226465717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37840f7b36e1ea8d3cc1eb484918408a0a7c80694e498a9624403ec6b2779da5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:06:55 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:06:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:07:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:07:39 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:08:11 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:08:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:08:13 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:08:14 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:08:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 15:08:16 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 15:08:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 15:08:18 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:19 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:08:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:21 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 15:08:22 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:08:24 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 15:08:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 15:08:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 15:08:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 15:08:32 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:08:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:08:34 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:08:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6aca795d67851a5bf64ff69de8a2c846040a785e02ab939c669ea1259dead`  
		Last Modified: Sat, 19 Mar 2022 15:11:16 GMT  
		Size: 85.8 MB (85763563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bdcf2d35ac4a0024417899c05e98131a4fff9dc84f1e8c8adc753bdce04155`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8ec78bd0d33bfd948482e9fddfc7b40d51477334e11b6fb2e7ef30e6edb77`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7bb9b39c93dd2e07a5372e3777c60cb0580fa34e0c509de2eff55931bdda02`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 546.9 KB (546945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6a905429eeab80d97e3d0628638e40ba16452b559eb12908873a93a91a3e19`  
		Last Modified: Sat, 19 Mar 2022 15:11:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4b9a3fc49d78b5e0b3831ecbceff18387baa0c173e82a7701578c1bd596185`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 6.9 KB (6918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c8577ef4db2696b862301023b268b85368ef6fcb21d3769c06a9a13fd5bcf`  
		Last Modified: Sat, 19 Mar 2022 15:11:39 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55f445dd268c9ca2b9a9d3fd0b8821f0a0fd2cfec6e249e708eeec06cdb2503`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:c833e7f91287c1f5278fae277f9e5c578f23343164d1e650008b3e410e16384d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233968471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d919663177257a141b27a779eee211f7bca2ffbc1f5dc8d79e150b12cfb0c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:49:46 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:49:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:50:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:50:32 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:52:31 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:52:34 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:52:36 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:52:38 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:52:41 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 20:52:42 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 20:52:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 20:52:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:52:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:53 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 20:52:59 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:52:59 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 20:53:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 20:53:18 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 20:53:22 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 20:53:24 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:53:26 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:53:27 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:53:28 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29745dd35ee1f69790cb70dafe2654f253a2638e23c28c77381c2a35be5ae34`  
		Last Modified: Sat, 19 Mar 2022 20:59:23 GMT  
		Size: 86.6 MB (86557393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81968045c994cb7690d1dc9d02c0dafbd65aa7250aa87e3ecb5a33d1f6873a`  
		Last Modified: Sat, 19 Mar 2022 20:59:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e298445fac0e7aca27b8ba8df16b18493ea21a96401f4545613ffd08bcc7c7a1`  
		Last Modified: Sat, 19 Mar 2022 20:59:08 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0bed89b849d63e13572d4bd1f077ac7051d8690ed5f7b2a7ee9f31235c407a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 546.8 KB (546771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6809331661c2785e9c54575fb950fb7978d450c5086c859db31604e5b79b58d1`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4731e00bf5db007aa911c27ad45121ec04a668928cd8a3e4ea8e7e8022f22f`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e63959ee9c0d9f76fdddb46152c725ee56be5cd78f916a1b217b72d8149f686`  
		Last Modified: Sat, 19 Mar 2022 20:59:43 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddec700f67833da011d3636ac47dd284f8ffe607f1ebe5f3f8baa77667774a78`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:14c134aca33da365fb3afaa2ef0bfc9a216327f4af1ba5f84f718828b9d1d19e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:0a5df04fdf9e2518814eabb4c4bb3616638b216c6dc23173bd2b20cae8700085
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237364118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d18a4c0a52de08e58755248a78dc6005cbb66942c98f06af6a504fc23cf8ae`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:33:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:33:12 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:33:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:33:49 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:33:49 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 22:34:15 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 22:34:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:34:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 22:34:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 22:34:17 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:34:17 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 22:34:22 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 22:34:23 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 22:34:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 22:34:25 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:34:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:34:25 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:34:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243b914b9e4b6fb7ac97f6985856105df397ebe953a46a891d3fb61e19cd188`  
		Last Modified: Sat, 19 Mar 2022 22:35:54 GMT  
		Size: 93.7 MB (93652268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c137b851e3462a6945dd8eba41e1c5d25719ead032e2a0b5f2ec5246218e6d`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6bd5a2ca725536cdf2adb96200b6c1e2e06302b461f5697abbcde1daefa5b`  
		Last Modified: Sat, 19 Mar 2022 22:35:41 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb82ac7fa955532c88d7a17213ea673acdde2093ec391b04a4e7d852920ea00`  
		Last Modified: Sat, 19 Mar 2022 22:35:39 GMT  
		Size: 577.0 KB (576968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933e83e7c77c7103082d620ca9e2efe0613e49ab34b0a5a188f1b68fa9f7a569`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda0434e279fc7a6bed15623d6cffc6470f6dc6f2b2f6468b72605a8d594e344`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34a2a49687acf914d45f77967952dc9ef09d6835439713e5061edadabb451c`  
		Last Modified: Sat, 19 Mar 2022 22:36:09 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf6410c63fc3634c4a8ff616843c05cafe9e5b1cd1af15f2815cb537ea9a31f`  
		Last Modified: Sat, 19 Mar 2022 22:36:04 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:f664c5ae3a0d1d0d6556109b5912e173dbdad1aae70f0c89aa76c403cfc79b16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226465717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37840f7b36e1ea8d3cc1eb484918408a0a7c80694e498a9624403ec6b2779da5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:06:55 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:06:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:07:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:07:39 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:08:11 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:08:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:08:13 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:08:14 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:08:15 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 15:08:16 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 15:08:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 15:08:18 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:19 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:08:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 15:08:21 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 15:08:22 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:08:24 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 15:08:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 15:08:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 15:08:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 15:08:32 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:08:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:08:34 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:08:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6aca795d67851a5bf64ff69de8a2c846040a785e02ab939c669ea1259dead`  
		Last Modified: Sat, 19 Mar 2022 15:11:16 GMT  
		Size: 85.8 MB (85763563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bdcf2d35ac4a0024417899c05e98131a4fff9dc84f1e8c8adc753bdce04155`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8ec78bd0d33bfd948482e9fddfc7b40d51477334e11b6fb2e7ef30e6edb77`  
		Last Modified: Sat, 19 Mar 2022 15:11:05 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7bb9b39c93dd2e07a5372e3777c60cb0580fa34e0c509de2eff55931bdda02`  
		Last Modified: Sat, 19 Mar 2022 15:11:03 GMT  
		Size: 546.9 KB (546945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6a905429eeab80d97e3d0628638e40ba16452b559eb12908873a93a91a3e19`  
		Last Modified: Sat, 19 Mar 2022 15:11:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4b9a3fc49d78b5e0b3831ecbceff18387baa0c173e82a7701578c1bd596185`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 6.9 KB (6918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c8577ef4db2696b862301023b268b85368ef6fcb21d3769c06a9a13fd5bcf`  
		Last Modified: Sat, 19 Mar 2022 15:11:39 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55f445dd268c9ca2b9a9d3fd0b8821f0a0fd2cfec6e249e708eeec06cdb2503`  
		Last Modified: Sat, 19 Mar 2022 15:11:28 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:c833e7f91287c1f5278fae277f9e5c578f23343164d1e650008b3e410e16384d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233968471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d919663177257a141b27a779eee211f7bca2ffbc1f5dc8d79e150b12cfb0c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:49:46 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:49:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:50:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:50:32 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:52:31 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:52:34 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:52:36 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:52:38 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:52:41 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 19 Mar 2022 20:52:42 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 19 Mar 2022 20:52:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 19 Mar 2022 20:52:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:52:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 19 Mar 2022 20:52:53 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 19 Mar 2022 20:52:59 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:52:59 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 19 Mar 2022 20:53:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 19 Mar 2022 20:53:18 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 19 Mar 2022 20:53:22 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 19 Mar 2022 20:53:24 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:53:26 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:53:27 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:53:28 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29745dd35ee1f69790cb70dafe2654f253a2638e23c28c77381c2a35be5ae34`  
		Last Modified: Sat, 19 Mar 2022 20:59:23 GMT  
		Size: 86.6 MB (86557393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81968045c994cb7690d1dc9d02c0dafbd65aa7250aa87e3ecb5a33d1f6873a`  
		Last Modified: Sat, 19 Mar 2022 20:59:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e298445fac0e7aca27b8ba8df16b18493ea21a96401f4545613ffd08bcc7c7a1`  
		Last Modified: Sat, 19 Mar 2022 20:59:08 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0bed89b849d63e13572d4bd1f077ac7051d8690ed5f7b2a7ee9f31235c407a`  
		Last Modified: Sat, 19 Mar 2022 20:59:05 GMT  
		Size: 546.8 KB (546771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6809331661c2785e9c54575fb950fb7978d450c5086c859db31604e5b79b58d1`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4731e00bf5db007aa911c27ad45121ec04a668928cd8a3e4ea8e7e8022f22f`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e63959ee9c0d9f76fdddb46152c725ee56be5cd78f916a1b217b72d8149f686`  
		Last Modified: Sat, 19 Mar 2022 20:59:43 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddec700f67833da011d3636ac47dd284f8ffe607f1ebe5f3f8baa77667774a78`  
		Last Modified: Sat, 19 Mar 2022 20:59:35 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:1dc812cf6152a1dbd7dd664e0764032b903cc57c50cff56b29cd4aca4225acd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:b8b90f3f8aa8a5a5a0ec94c45447c20d7e2653088cd2f92fadc0fc1adbdfe9c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235101881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d1ac77f073ff34cd4af6e8870392ef73eb84279d0aeb4e35641c72b1ae3d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:34:48 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:34:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:35:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:35:07 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 22:35:08 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:09 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:35:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 22:35:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 22:35:18 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 22:35:19 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:35:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:35:19 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:35:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918014104c9ad49400ad5b9cc91d4bcbae82a73fa5abc7a409bf899c6c43f707`  
		Last Modified: Sat, 19 Mar 2022 22:36:36 GMT  
		Size: 93.7 MB (93654889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dbdd5fbdd128de63982a3bcd426031fd93f653efb545091ac58b78a211fe`  
		Last Modified: Sat, 19 Mar 2022 22:36:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b04accad0ea54945a94640fe15c4f18217ac339546430605562903bb6e198c`  
		Last Modified: Sat, 19 Mar 2022 22:36:23 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf332606cb830b506954d33ba501b217b0cf296e237e53ef52a6a9a64c442`  
		Last Modified: Sat, 19 Mar 2022 22:36:22 GMT  
		Size: 1.0 MB (1003224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212fc94ac887dd5a2399140898860c0a998fe2df050fc6e32930fee44eb331d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea58fb34b6055f277ccc1d770336f1a956999418f8c74dcac36d843e5b416d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24ddcab601ff797ff8b88340a09e3597f00209e58763e8cf7ed883c7c7dcb87`  
		Last Modified: Sat, 19 Mar 2022 22:36:28 GMT  
		Size: 113.7 MB (113727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c310e4514d6b20246d217eb5e9eb415ba672947ac5986dff90d60de6cee91c`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8145813d259caf6cd0bea5d1927b07af9b65099efde705c1b7dc4b12dc186c85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224156613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282818f0e70e12d2041d5851adc6e578279aaaed15d0a8744828bf7dc42eefed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:09:07 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:09:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:09:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:09:55 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:09:56 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:09:57 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:09:58 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:09:59 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:10:00 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 15:10:01 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 15:10:02 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 15:10:03 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:10:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:06 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:10:08 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 15:10:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 15:10:29 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 15:10:29 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:10:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:10:31 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:10:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3433408c5fc7f4ae638ee2b5297e626eccb6ef1eaa854483eaa88fe9452b9`  
		Last Modified: Sat, 19 Mar 2022 15:12:08 GMT  
		Size: 85.8 MB (85763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf766653b0804c4ca85b92cc0c0069fac5a3f16d050f228364daa9898cdddc`  
		Last Modified: Sat, 19 Mar 2022 15:11:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faef7cbb4cb2bf00d122900c6fc72a76a1c4ce7e507619ce147f81ef8541dd2`  
		Last Modified: Sat, 19 Mar 2022 15:11:57 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708c338db08b4e85061950c8cb417d1fdd8d11ab132c8869662712a9d49a856`  
		Last Modified: Sat, 19 Mar 2022 15:11:55 GMT  
		Size: 929.4 KB (929409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ab77260b346ebc4ffb2b67788f195a531157a6a926db586e202224550f95b5`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a15c093ce6465bc4b31ce2c94333e202d3a124194d56bb99438c8074746c3c`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0df29d03ead5b114014be21794a723b2a019942d32b8d108fe3f1f2de09ff`  
		Last Modified: Sat, 19 Mar 2022 15:12:12 GMT  
		Size: 113.7 MB (113727850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c4162cb8595bb82ce1922c26bc251eadd27b261925942c84f067f35057191`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:0c8c69d7af8f945591a5d089408490bf52d5bc01ddafc64b7143d5ec6676a8ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231634930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7996e14d3d401d9e6a086fdc28917a40774b46df8ec09f0dd2d332cf566df8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:56:02 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:56:12 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:57:00 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:57:03 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:57:07 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:57:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:57:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:57:17 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:57:19 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 20:57:21 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 20:57:22 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 20:57:25 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:57:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:36 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:57:37 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 20:57:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 20:58:01 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 20:58:07 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:58:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:58:14 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54998de650aec3ff8c87077551a8a8dedbac826f959645af516a214758030de1`  
		Last Modified: Sat, 19 Mar 2022 21:00:18 GMT  
		Size: 86.6 MB (86557500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80861eb3c1c18c4914806cea4a42cc6605837eb735445fe587096738b931ba`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3e83293caa8f19217184082aaf48f054162fd676b0bfe80c811db04b5fa07`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172e62718fccbad62107b4fe7fd7a9a97a92e26d79914dbc2cd2ce19c1ae3a3e`  
		Last Modified: Sat, 19 Mar 2022 21:00:01 GMT  
		Size: 904.2 KB (904217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ad91e85241ec6b752c76025976f23d679c8eda783616cb3d8830044dcb21a`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaebf6593ed9f193fbd8172caa14b34ddf91ceab1a3dc48c01ad9e695794966`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d1d821c92f5f66422e0625adaed7d15289260431916f065c873a51902db85`  
		Last Modified: Sat, 19 Mar 2022 21:00:10 GMT  
		Size: 113.7 MB (113727951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7730acde910ffb0b1920533e60561ebf0826b19c5d57baa84709e782722f8539`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:1dc812cf6152a1dbd7dd664e0764032b903cc57c50cff56b29cd4aca4225acd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:b8b90f3f8aa8a5a5a0ec94c45447c20d7e2653088cd2f92fadc0fc1adbdfe9c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235101881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d1ac77f073ff34cd4af6e8870392ef73eb84279d0aeb4e35641c72b1ae3d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:34:48 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:34:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:35:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:35:07 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 22:35:08 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:09 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:35:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 22:35:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 22:35:18 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 22:35:19 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:35:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:35:19 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:35:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918014104c9ad49400ad5b9cc91d4bcbae82a73fa5abc7a409bf899c6c43f707`  
		Last Modified: Sat, 19 Mar 2022 22:36:36 GMT  
		Size: 93.7 MB (93654889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dbdd5fbdd128de63982a3bcd426031fd93f653efb545091ac58b78a211fe`  
		Last Modified: Sat, 19 Mar 2022 22:36:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b04accad0ea54945a94640fe15c4f18217ac339546430605562903bb6e198c`  
		Last Modified: Sat, 19 Mar 2022 22:36:23 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf332606cb830b506954d33ba501b217b0cf296e237e53ef52a6a9a64c442`  
		Last Modified: Sat, 19 Mar 2022 22:36:22 GMT  
		Size: 1.0 MB (1003224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212fc94ac887dd5a2399140898860c0a998fe2df050fc6e32930fee44eb331d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea58fb34b6055f277ccc1d770336f1a956999418f8c74dcac36d843e5b416d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24ddcab601ff797ff8b88340a09e3597f00209e58763e8cf7ed883c7c7dcb87`  
		Last Modified: Sat, 19 Mar 2022 22:36:28 GMT  
		Size: 113.7 MB (113727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c310e4514d6b20246d217eb5e9eb415ba672947ac5986dff90d60de6cee91c`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8145813d259caf6cd0bea5d1927b07af9b65099efde705c1b7dc4b12dc186c85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224156613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282818f0e70e12d2041d5851adc6e578279aaaed15d0a8744828bf7dc42eefed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:09:07 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:09:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:09:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:09:55 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:09:56 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:09:57 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:09:58 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:09:59 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:10:00 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 15:10:01 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 15:10:02 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 15:10:03 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:10:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:06 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:10:08 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 15:10:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 15:10:29 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 15:10:29 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:10:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:10:31 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:10:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3433408c5fc7f4ae638ee2b5297e626eccb6ef1eaa854483eaa88fe9452b9`  
		Last Modified: Sat, 19 Mar 2022 15:12:08 GMT  
		Size: 85.8 MB (85763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf766653b0804c4ca85b92cc0c0069fac5a3f16d050f228364daa9898cdddc`  
		Last Modified: Sat, 19 Mar 2022 15:11:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faef7cbb4cb2bf00d122900c6fc72a76a1c4ce7e507619ce147f81ef8541dd2`  
		Last Modified: Sat, 19 Mar 2022 15:11:57 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708c338db08b4e85061950c8cb417d1fdd8d11ab132c8869662712a9d49a856`  
		Last Modified: Sat, 19 Mar 2022 15:11:55 GMT  
		Size: 929.4 KB (929409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ab77260b346ebc4ffb2b67788f195a531157a6a926db586e202224550f95b5`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a15c093ce6465bc4b31ce2c94333e202d3a124194d56bb99438c8074746c3c`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0df29d03ead5b114014be21794a723b2a019942d32b8d108fe3f1f2de09ff`  
		Last Modified: Sat, 19 Mar 2022 15:12:12 GMT  
		Size: 113.7 MB (113727850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c4162cb8595bb82ce1922c26bc251eadd27b261925942c84f067f35057191`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:0c8c69d7af8f945591a5d089408490bf52d5bc01ddafc64b7143d5ec6676a8ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231634930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7996e14d3d401d9e6a086fdc28917a40774b46df8ec09f0dd2d332cf566df8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:56:02 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:56:12 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:57:00 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:57:03 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:57:07 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:57:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:57:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:57:17 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:57:19 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 20:57:21 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 20:57:22 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 20:57:25 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:57:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:36 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:57:37 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 20:57:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 20:58:01 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 20:58:07 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:58:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:58:14 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54998de650aec3ff8c87077551a8a8dedbac826f959645af516a214758030de1`  
		Last Modified: Sat, 19 Mar 2022 21:00:18 GMT  
		Size: 86.6 MB (86557500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80861eb3c1c18c4914806cea4a42cc6605837eb735445fe587096738b931ba`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3e83293caa8f19217184082aaf48f054162fd676b0bfe80c811db04b5fa07`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172e62718fccbad62107b4fe7fd7a9a97a92e26d79914dbc2cd2ce19c1ae3a3e`  
		Last Modified: Sat, 19 Mar 2022 21:00:01 GMT  
		Size: 904.2 KB (904217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ad91e85241ec6b752c76025976f23d679c8eda783616cb3d8830044dcb21a`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaebf6593ed9f193fbd8172caa14b34ddf91ceab1a3dc48c01ad9e695794966`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d1d821c92f5f66422e0625adaed7d15289260431916f065c873a51902db85`  
		Last Modified: Sat, 19 Mar 2022 21:00:10 GMT  
		Size: 113.7 MB (113727951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7730acde910ffb0b1920533e60561ebf0826b19c5d57baa84709e782722f8539`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:1dc812cf6152a1dbd7dd664e0764032b903cc57c50cff56b29cd4aca4225acd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:b8b90f3f8aa8a5a5a0ec94c45447c20d7e2653088cd2f92fadc0fc1adbdfe9c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235101881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d1ac77f073ff34cd4af6e8870392ef73eb84279d0aeb4e35641c72b1ae3d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:32:22 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 22:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:34:48 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 22:34:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 22:35:07 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 22:35:07 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 22:35:08 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 22:35:08 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 22:35:09 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 22:35:09 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 22:35:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 22:35:18 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 22:35:19 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 22:35:19 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 22:35:19 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 22:35:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918014104c9ad49400ad5b9cc91d4bcbae82a73fa5abc7a409bf899c6c43f707`  
		Last Modified: Sat, 19 Mar 2022 22:36:36 GMT  
		Size: 93.7 MB (93654889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948dbdd5fbdd128de63982a3bcd426031fd93f653efb545091ac58b78a211fe`  
		Last Modified: Sat, 19 Mar 2022 22:36:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b04accad0ea54945a94640fe15c4f18217ac339546430605562903bb6e198c`  
		Last Modified: Sat, 19 Mar 2022 22:36:23 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf332606cb830b506954d33ba501b217b0cf296e237e53ef52a6a9a64c442`  
		Last Modified: Sat, 19 Mar 2022 22:36:22 GMT  
		Size: 1.0 MB (1003224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212fc94ac887dd5a2399140898860c0a998fe2df050fc6e32930fee44eb331d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea58fb34b6055f277ccc1d770336f1a956999418f8c74dcac36d843e5b416d`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24ddcab601ff797ff8b88340a09e3597f00209e58763e8cf7ed883c7c7dcb87`  
		Last Modified: Sat, 19 Mar 2022 22:36:28 GMT  
		Size: 113.7 MB (113727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c310e4514d6b20246d217eb5e9eb415ba672947ac5986dff90d60de6cee91c`  
		Last Modified: Sat, 19 Mar 2022 22:36:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8145813d259caf6cd0bea5d1927b07af9b65099efde705c1b7dc4b12dc186c85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224156613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282818f0e70e12d2041d5851adc6e578279aaaed15d0a8744828bf7dc42eefed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:06:29 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 15:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:09:07 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 15:09:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 15:09:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 15:09:55 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 15:09:56 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 15:09:57 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 15:09:58 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 15:09:59 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 15:10:00 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 15:10:01 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 15:10:02 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 15:10:03 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 15:10:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 15:10:06 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 15:10:08 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 15:10:28 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 15:10:29 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 15:10:29 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 15:10:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 15:10:31 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 15:10:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3433408c5fc7f4ae638ee2b5297e626eccb6ef1eaa854483eaa88fe9452b9`  
		Last Modified: Sat, 19 Mar 2022 15:12:08 GMT  
		Size: 85.8 MB (85763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf766653b0804c4ca85b92cc0c0069fac5a3f16d050f228364daa9898cdddc`  
		Last Modified: Sat, 19 Mar 2022 15:11:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faef7cbb4cb2bf00d122900c6fc72a76a1c4ce7e507619ce147f81ef8541dd2`  
		Last Modified: Sat, 19 Mar 2022 15:11:57 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708c338db08b4e85061950c8cb417d1fdd8d11ab132c8869662712a9d49a856`  
		Last Modified: Sat, 19 Mar 2022 15:11:55 GMT  
		Size: 929.4 KB (929409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ab77260b346ebc4ffb2b67788f195a531157a6a926db586e202224550f95b5`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a15c093ce6465bc4b31ce2c94333e202d3a124194d56bb99438c8074746c3c`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0df29d03ead5b114014be21794a723b2a019942d32b8d108fe3f1f2de09ff`  
		Last Modified: Sat, 19 Mar 2022 15:12:12 GMT  
		Size: 113.7 MB (113727850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c4162cb8595bb82ce1922c26bc251eadd27b261925942c84f067f35057191`  
		Last Modified: Sat, 19 Mar 2022 15:11:54 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:0c8c69d7af8f945591a5d089408490bf52d5bc01ddafc64b7143d5ec6676a8ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231634930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7996e14d3d401d9e6a086fdc28917a40774b46df8ec09f0dd2d332cf566df8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:47:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Sat, 19 Mar 2022 20:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:56:02 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 19 Mar 2022 20:56:12 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 19 Mar 2022 20:57:00 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 19 Mar 2022 20:57:03 GMT
ARG BONITA_VERSION
# Sat, 19 Mar 2022 20:57:07 GMT
ARG BRANDING_VERSION
# Sat, 19 Mar 2022 20:57:12 GMT
ARG BONITA_SHA256
# Sat, 19 Mar 2022 20:57:15 GMT
ARG BASE_URL
# Sat, 19 Mar 2022 20:57:17 GMT
ARG BONITA_URL
# Sat, 19 Mar 2022 20:57:19 GMT
ENV BONITA_VERSION=7.13.0
# Sat, 19 Mar 2022 20:57:21 GMT
ENV BRANDING_VERSION=2021.2-u0
# Sat, 19 Mar 2022 20:57:22 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Sat, 19 Mar 2022 20:57:25 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:26 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 19 Mar 2022 20:57:28 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Sat, 19 Mar 2022 20:57:36 GMT
RUN mkdir /opt/files
# Sat, 19 Mar 2022 20:57:37 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Sat, 19 Mar 2022 20:57:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Sat, 19 Mar 2022 20:58:01 GMT
ENV HTTP_API=false
# Sat, 19 Mar 2022 20:58:07 GMT
VOLUME [/opt/bonita]
# Sat, 19 Mar 2022 20:58:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 19 Mar 2022 20:58:14 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 20:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54998de650aec3ff8c87077551a8a8dedbac826f959645af516a214758030de1`  
		Last Modified: Sat, 19 Mar 2022 21:00:18 GMT  
		Size: 86.6 MB (86557500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80861eb3c1c18c4914806cea4a42cc6605837eb735445fe587096738b931ba`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3e83293caa8f19217184082aaf48f054162fd676b0bfe80c811db04b5fa07`  
		Last Modified: Sat, 19 Mar 2022 21:00:04 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172e62718fccbad62107b4fe7fd7a9a97a92e26d79914dbc2cd2ce19c1ae3a3e`  
		Last Modified: Sat, 19 Mar 2022 21:00:01 GMT  
		Size: 904.2 KB (904217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ad91e85241ec6b752c76025976f23d679c8eda783616cb3d8830044dcb21a`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaebf6593ed9f193fbd8172caa14b34ddf91ceab1a3dc48c01ad9e695794966`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d1d821c92f5f66422e0625adaed7d15289260431916f065c873a51902db85`  
		Last Modified: Sat, 19 Mar 2022 21:00:10 GMT  
		Size: 113.7 MB (113727951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7730acde910ffb0b1920533e60561ebf0826b19c5d57baa84709e782722f8539`  
		Last Modified: Sat, 19 Mar 2022 21:00:00 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
