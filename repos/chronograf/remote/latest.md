## `chronograf:latest`

```console
$ docker pull chronograf@sha256:5e627aee97cf4105e0c92aa1c5f79c10526ead500f8d4fee099c116144fc4a73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:2e42b20660b4b9b29fd977dae1525c921bc50310501d3eef6e7ab9b7d2e44b1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70197163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e5b936fde30edd440a8a01f65254c38a443f7b49b612ea5d65f790e1a54472a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:59:57 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 15 May 2020 18:00:40 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Fri, 15 May 2020 18:00:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 18:00:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 15 May 2020 18:00:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 15 May 2020 18:00:54 GMT
EXPOSE 8888
# Fri, 15 May 2020 18:00:54 GMT
VOLUME [/var/lib/chronograf]
# Fri, 15 May 2020 18:00:54 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 15 May 2020 18:00:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 18:00:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7761e67ad5faabbbdd2bb2babf383e41826d1d7f495f4a232c3318e4b8a8602`  
		Last Modified: Fri, 15 May 2020 18:01:13 GMT  
		Size: 4.5 MB (4503562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfba40331895fe9ec84613caa00d0011bfa3baa56afa73c2e7a1486963c1bfa`  
		Last Modified: Fri, 15 May 2020 18:01:58 GMT  
		Size: 43.1 MB (43149320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c638029640473ba59f76d5658198a6c52496cc027b4ce461518ba0f866a02`  
		Last Modified: Fri, 15 May 2020 18:01:50 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cd14d06ac6c82d9e93b2e4588e560eb4e8c9b2610a60333f488639e66ea2e9`  
		Last Modified: Fri, 15 May 2020 18:01:50 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4222cd18cd6b1e6fcbc5049e23635930fee8c7d38ea3137b827de597d0c105`  
		Last Modified: Fri, 15 May 2020 18:01:50 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:521f2ac22edd1064ba17fdb3cacade3fc569bf18abc9e1f260acf515bf3cdc8d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63610183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091b415ce8d220e076a5d2772c166032c0eaa34880200c3527caa3d0487bf8b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 15 May 2020 01:06:56 GMT
ADD file:a0ecfe1283dbc15e795cd274e422095545ef6e8af80bc23ee7063abb597a5a88 in / 
# Fri, 15 May 2020 01:07:00 GMT
CMD ["bash"]
# Fri, 15 May 2020 09:26:45 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 15 May 2020 09:28:00 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Fri, 15 May 2020 09:28:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 09:28:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 15 May 2020 09:28:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 15 May 2020 09:28:25 GMT
EXPOSE 8888
# Fri, 15 May 2020 09:28:25 GMT
VOLUME [/var/lib/chronograf]
# Fri, 15 May 2020 09:28:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 15 May 2020 09:28:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 09:28:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:90cadb81644e46b7fbfb33027f8b34af18f1e04db99f6b29cc1ff98aafe9b5d6`  
		Last Modified: Fri, 15 May 2020 01:15:03 GMT  
		Size: 19.3 MB (19304729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee349b145e568cb54ad903d7ade88720cd9780b99224d42494f84569f693ad1`  
		Last Modified: Fri, 15 May 2020 09:28:46 GMT  
		Size: 3.9 MB (3877295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0869fc51efd7f725d71e438851f9ce4e0fe175c07502b8c2acc722e4fa9d1139`  
		Last Modified: Fri, 15 May 2020 09:29:31 GMT  
		Size: 40.4 MB (40403760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949be68af8dd26ae9d5ccce119d7e555880164e94815efd7e3cab6e996e44570`  
		Last Modified: Fri, 15 May 2020 09:29:19 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db522a140106cac4de364e96d0e9636a04f921e732e6619aebd951626d587cf5`  
		Last Modified: Fri, 15 May 2020 09:29:19 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554069704a261c5dd12f02a4f5c10c6501e754a347ac9d2d404f594bd2ffed77`  
		Last Modified: Fri, 15 May 2020 09:29:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9369dc6d98735f8b79bc1076d9be8e1517452fa5a796be7c90186b5b77c15ac5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc19e90c0f79e3da3fbf0d4892bfb01ff957566c7d97f0f0d0a5e29e7ae6d40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:50:22 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Thu, 14 May 2020 00:50:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:45 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a71fe07ad9b05ef55473a46159658ea8427311e4bc8b39a9ae6d384dd5c1f63`  
		Last Modified: Thu, 14 May 2020 00:51:36 GMT  
		Size: 40.2 MB (40239346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534e3a2953b36d5d1ebc359f5338af4eaf36d7e709f31df4bf6a235e6ee20be`  
		Last Modified: Thu, 14 May 2020 00:51:27 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34bd489cf7347846985910cb4e2513fd2760d84d00ea520c54686b14009813`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8f7e28ce4718da060028d491bbb042da94690056e2c737956a4ca6ab891879`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
