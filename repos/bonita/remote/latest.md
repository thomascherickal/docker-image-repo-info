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
