<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:1.8.8`](#chronograf188)
-	[`chronograf:1.8.8-alpine`](#chronograf188-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:1d473e92a4c686d5dfe22dd4cdb5d2060c253dcb522b2b9c01277ada0a7551c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:74fc93c1c96a86cf152fe459b93649c86c72bd1226a0b55974d8ea4ed8556197
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca153c63947e1abd29e1bf99eb9b4984c8095bc57b5852f2989d9a2f32a1d658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:57:14 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 30 Mar 2021 22:57:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:57:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:57:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:57:23 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:57:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:57:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:57:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:57:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb5e63586af7d23e085defc2d66fb6043506fc4207522e583eb8b307cd9d04`  
		Last Modified: Tue, 30 Mar 2021 22:58:59 GMT  
		Size: 6.8 MB (6760089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a75679e9a2cf3baaefb20aa322f3fad72a35c7887a34b4564be93096339a2c`  
		Last Modified: Tue, 30 Mar 2021 22:59:07 GMT  
		Size: 20.0 MB (20044284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8c5c240b9cc56607fc70d43c7a7c524916f2985f6fe45b2f16ff2c06bbf55e`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47a59bde66eefa0e38812f8a9876a9c6e02c911167b1e265788aac3978e50d9`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c25b7730bbf78ff86fc59c82429ef1dcd0ca671af61a1276c5bad99998f0c`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:53873c89ea815ef99dd0b8a08b96195aa9ec2605f1206389b2db17cd2f034e52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43936358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422facc8f952ad9871981c4916399ae9a9609093ce279ceb9b80ef11fed69652`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:14:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:14:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 18:14:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:14:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:14:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:14:58 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:14:59 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:15:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:15:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:15:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59a68a97e8e2d980ebdbd6cc4e0d02a1d682e732f0408185a01f3fc7abef6c`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 5.8 MB (5779536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3217e270e8fc571f9765f81c3283ee92c1b674b47dfe98cbd1adbf0edf2071de`  
		Last Modified: Fri, 26 Mar 2021 18:17:25 GMT  
		Size: 18.8 MB (18816805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0636f729eb2fb71c6349c73bb7db2667e2005511d26ffe0c18f0dd74b8694`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11912ad7b01cf2e2487cca2e69ff987a23ea167b873ab096deab1685b07b1777`  
		Last Modified: Fri, 26 Mar 2021 18:17:18 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a465d77903e80f05261c78af6ac51cbc9b9253281eaabf3afeb0465dab1d181c`  
		Last Modified: Fri, 26 Mar 2021 18:17:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:09508483ddbf522705c9463e8f9ef97ead20669ef42036589e495f81ae47e5ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45419981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9b98004dd9cfd9594a70a7991fa85245ffdcbc6029562b43a6326375d5f16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:35:47 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 31 Mar 2021 00:36:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:36:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:36:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:36:04 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:36:05 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:36:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:36:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:36:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fb0292c785020e4d806224fad8e726db9930f08d23b4916773dc04474da75`  
		Last Modified: Wed, 31 Mar 2021 00:38:06 GMT  
		Size: 6.0 MB (6047578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d963f63e09992bb8e06a8b9d639e8cc9f2db4545856ed82525649096d8ac98`  
		Last Modified: Wed, 31 Mar 2021 00:38:10 GMT  
		Size: 19.0 MB (18958705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e638e4b681f0a6344eeab4d41349c10fc6cc81cf5baecea66b5f85e9309bc2`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00a035342319bea10e97fd77b84af85ddc7ff4b68ec93821ea0fde7a26a0186`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a012423bc466d20f3bff63ced76957ea560ac204a0fb8f948bee9db1062179a`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:865641b1f7a0ec7d2eacdd0431132ce8d4a96e648d5981193f3ae8f31b337a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0aebf3a16b9438a5aeed9c108b0af42564477cee319bc062a088273af6076cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eedf76ed9ed86a8f5aaefa50c855fd386b31bd9b6f4b6451237a49024e863d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:40:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 02:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:40:52 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:40:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:40:53 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:40:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:40:54 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:40:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:40:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12e5ff56de26f4ed0958fb375c07c902515fdc8665f4a11b472c4b867bd856`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 11.7 MB (11736751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b555b8110c844c0e86847b84adf1bb0a942dfc22cbafc4eb9d3639170bb85e`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 12.3 KB (12277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12381a23b90f4eeeaf431a6749c00bdd2b74ebf9af28c63c666f66980dbab`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f1bb27bd5414c71fb0835174d5e9edf0cf37d1ec243753f036ec89833d9de`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:1d473e92a4c686d5dfe22dd4cdb5d2060c253dcb522b2b9c01277ada0a7551c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:74fc93c1c96a86cf152fe459b93649c86c72bd1226a0b55974d8ea4ed8556197
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca153c63947e1abd29e1bf99eb9b4984c8095bc57b5852f2989d9a2f32a1d658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:57:14 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 30 Mar 2021 22:57:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:57:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:57:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:57:23 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:57:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:57:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:57:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:57:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb5e63586af7d23e085defc2d66fb6043506fc4207522e583eb8b307cd9d04`  
		Last Modified: Tue, 30 Mar 2021 22:58:59 GMT  
		Size: 6.8 MB (6760089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a75679e9a2cf3baaefb20aa322f3fad72a35c7887a34b4564be93096339a2c`  
		Last Modified: Tue, 30 Mar 2021 22:59:07 GMT  
		Size: 20.0 MB (20044284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8c5c240b9cc56607fc70d43c7a7c524916f2985f6fe45b2f16ff2c06bbf55e`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47a59bde66eefa0e38812f8a9876a9c6e02c911167b1e265788aac3978e50d9`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c25b7730bbf78ff86fc59c82429ef1dcd0ca671af61a1276c5bad99998f0c`  
		Last Modified: Tue, 30 Mar 2021 22:58:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:53873c89ea815ef99dd0b8a08b96195aa9ec2605f1206389b2db17cd2f034e52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43936358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422facc8f952ad9871981c4916399ae9a9609093ce279ceb9b80ef11fed69652`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:14:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:14:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 18:14:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:14:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:14:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:14:58 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:14:59 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:15:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:15:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:15:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59a68a97e8e2d980ebdbd6cc4e0d02a1d682e732f0408185a01f3fc7abef6c`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 5.8 MB (5779536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3217e270e8fc571f9765f81c3283ee92c1b674b47dfe98cbd1adbf0edf2071de`  
		Last Modified: Fri, 26 Mar 2021 18:17:25 GMT  
		Size: 18.8 MB (18816805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0636f729eb2fb71c6349c73bb7db2667e2005511d26ffe0c18f0dd74b8694`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11912ad7b01cf2e2487cca2e69ff987a23ea167b873ab096deab1685b07b1777`  
		Last Modified: Fri, 26 Mar 2021 18:17:18 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a465d77903e80f05261c78af6ac51cbc9b9253281eaabf3afeb0465dab1d181c`  
		Last Modified: Fri, 26 Mar 2021 18:17:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:09508483ddbf522705c9463e8f9ef97ead20669ef42036589e495f81ae47e5ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45419981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9b98004dd9cfd9594a70a7991fa85245ffdcbc6029562b43a6326375d5f16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:35:47 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 31 Mar 2021 00:36:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:36:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:36:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:36:04 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:36:05 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:36:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:36:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:36:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fb0292c785020e4d806224fad8e726db9930f08d23b4916773dc04474da75`  
		Last Modified: Wed, 31 Mar 2021 00:38:06 GMT  
		Size: 6.0 MB (6047578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d963f63e09992bb8e06a8b9d639e8cc9f2db4545856ed82525649096d8ac98`  
		Last Modified: Wed, 31 Mar 2021 00:38:10 GMT  
		Size: 19.0 MB (18958705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e638e4b681f0a6344eeab4d41349c10fc6cc81cf5baecea66b5f85e9309bc2`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00a035342319bea10e97fd77b84af85ddc7ff4b68ec93821ea0fde7a26a0186`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a012423bc466d20f3bff63ced76957ea560ac204a0fb8f948bee9db1062179a`  
		Last Modified: Wed, 31 Mar 2021 00:38:05 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:865641b1f7a0ec7d2eacdd0431132ce8d4a96e648d5981193f3ae8f31b337a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0aebf3a16b9438a5aeed9c108b0af42564477cee319bc062a088273af6076cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eedf76ed9ed86a8f5aaefa50c855fd386b31bd9b6f4b6451237a49024e863d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:40:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 02:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:40:52 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:40:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:40:53 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:40:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:40:54 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:40:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:40:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12e5ff56de26f4ed0958fb375c07c902515fdc8665f4a11b472c4b867bd856`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 11.7 MB (11736751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b555b8110c844c0e86847b84adf1bb0a942dfc22cbafc4eb9d3639170bb85e`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 12.3 KB (12277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12381a23b90f4eeeaf431a6749c00bdd2b74ebf9af28c63c666f66980dbab`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f1bb27bd5414c71fb0835174d5e9edf0cf37d1ec243753f036ec89833d9de`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:e65ecd67a0fecf84ea08ed7955f37c0793859717c3a08116ab4d20455a763ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:c530ab20f7d3f0b5eb67d857060ba1caea1b0a0449e3c2b0aeca752b7900da01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65375465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91cd61754ad91503717107537eb4e227b9e4cb0afe8ffd8bbe554f14a32a593`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:57:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 30 Mar 2021 22:57:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:57:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:57:56 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:57:56 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:57:56 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:57:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:57:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:57:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af08da074a0a94457bd5eeb2d855343351c3b18262db2d3a6feb8626b811229`  
		Last Modified: Tue, 30 Mar 2021 22:59:21 GMT  
		Size: 4.5 MB (4506032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d9557f97d04cad45e8594dd1be3f66a3b2cd9c1fbe1592a203033c8f56655d`  
		Last Modified: Tue, 30 Mar 2021 22:59:28 GMT  
		Size: 38.3 MB (38316772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2143eff8dfd55cf1967cb16022151ee15fc8ead88e4b9bde0b04ae649440e`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df0233bca2fc85172bfe9f88c130d09d47aadfad72655b624668c073aa1ead`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e46992aec30815225cbfd914ca0d95a3e8a870ea6076a8ad423f8c04df0ffe`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:988d0d3fa2c397ef8b562989b1bb6bb0cd7dd4f69d44b7d41ff1397cd4bf19b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58994006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57ddb3251c6c355ccbdeae0af8937e05019d95e95a957cfacbb299aad161281`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:15:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:15:34 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 18:15:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:16:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:16:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:16:05 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:16:06 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:16:07 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:16:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b75fbd498c1e0104cd0bfa5f97c66beaa4c8163b10a72142c33a1ba3b991835`  
		Last Modified: Fri, 26 Mar 2021 18:17:33 GMT  
		Size: 3.9 MB (3879538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e8e98fe0d3c69f4778207f312911140421f3250d3193307d0410f5e94e7e8`  
		Last Modified: Fri, 26 Mar 2021 18:17:45 GMT  
		Size: 35.8 MB (35774454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4f3959d152ef4aba7a73ebda9c98ed1154da99080d07b711880fcef5c088fd`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd62fafd31e2f1e76e15e2ce615fa4c3cd0b27d0032039ba648b2916dbcd8f67`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d63d3d3f0270f5bb767e3626bb6b77cd56a0ab7caf65ed6f30ef5e9a4635e`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:909fe504f3a8d0ce4382c1f72db0d02f325849e67208e0e53fb3c3365bf4441d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60477245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6561e2eefb88b49f291db74e7620987e227c6f3beac4489dfc5ff03ee9864686`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:36:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:36:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 31 Mar 2021 00:36:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:36:59 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:37:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:37:01 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:37:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:37:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:37:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:37:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f79332eba6d531ed7d7f7098ef5b3c9bdf5b2d226411e34a84af572d7765b5`  
		Last Modified: Wed, 31 Mar 2021 00:38:21 GMT  
		Size: 4.1 MB (4082290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329100e36c1415f1b13f306bca5dc0381c529b1a1b42186141a86b18bd577bcd`  
		Last Modified: Wed, 31 Mar 2021 00:38:31 GMT  
		Size: 36.0 MB (35981251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182347e51ab4f375e0fec2cb9bc9df4ceb68acb4025fc055d5c5b5e71ba4475d`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa0b2d21d61dbe4afda954bb0cced4aecca93c4ac367d1a109cf921bd486080`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a1bbd48a4790e5d7c1f465ae2ef2f934a970b739d2c71fc7bc617c06dce56c`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:2c763ee4efeabcda89d91708e177111bb459c3c4e2174ad697c671d780eec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:428e98a9f624def380648c24e4ab802f136b56e81459119580b83855902bf989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22660462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7abe0632a70257e96d02ebf9c0f8f779291d0eaae40a5d32bbffb313658b2119`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 02:41:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:13 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:14 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:14 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8347978863206fd815b2a3bb0be789f20244679d01952c7cf99a2b62f26e50`  
		Last Modified: Fri, 26 Mar 2021 02:42:27 GMT  
		Size: 19.6 MB (19555255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83be8e29182aea4959f986a45df5392775825ead1857be98fec722452d59eb7`  
		Last Modified: Fri, 26 Mar 2021 02:42:23 GMT  
		Size: 12.3 KB (12272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bba321eed11d28f7c89bf86c98104bfe62a8bdb233953efb77cda61c4b0304`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7060062a0a29d0380f03a272669a9230258bab2dfa7df2d7d90bce2c3f60d60d`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:e65ecd67a0fecf84ea08ed7955f37c0793859717c3a08116ab4d20455a763ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:c530ab20f7d3f0b5eb67d857060ba1caea1b0a0449e3c2b0aeca752b7900da01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65375465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91cd61754ad91503717107537eb4e227b9e4cb0afe8ffd8bbe554f14a32a593`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:57:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 30 Mar 2021 22:57:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:57:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:57:56 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:57:56 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:57:56 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:57:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:57:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:57:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af08da074a0a94457bd5eeb2d855343351c3b18262db2d3a6feb8626b811229`  
		Last Modified: Tue, 30 Mar 2021 22:59:21 GMT  
		Size: 4.5 MB (4506032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d9557f97d04cad45e8594dd1be3f66a3b2cd9c1fbe1592a203033c8f56655d`  
		Last Modified: Tue, 30 Mar 2021 22:59:28 GMT  
		Size: 38.3 MB (38316772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2143eff8dfd55cf1967cb16022151ee15fc8ead88e4b9bde0b04ae649440e`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df0233bca2fc85172bfe9f88c130d09d47aadfad72655b624668c073aa1ead`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e46992aec30815225cbfd914ca0d95a3e8a870ea6076a8ad423f8c04df0ffe`  
		Last Modified: Tue, 30 Mar 2021 22:59:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:988d0d3fa2c397ef8b562989b1bb6bb0cd7dd4f69d44b7d41ff1397cd4bf19b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58994006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57ddb3251c6c355ccbdeae0af8937e05019d95e95a957cfacbb299aad161281`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:15:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:15:34 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 18:15:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:16:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:16:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:16:05 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:16:06 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:16:07 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:16:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b75fbd498c1e0104cd0bfa5f97c66beaa4c8163b10a72142c33a1ba3b991835`  
		Last Modified: Fri, 26 Mar 2021 18:17:33 GMT  
		Size: 3.9 MB (3879538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e8e98fe0d3c69f4778207f312911140421f3250d3193307d0410f5e94e7e8`  
		Last Modified: Fri, 26 Mar 2021 18:17:45 GMT  
		Size: 35.8 MB (35774454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4f3959d152ef4aba7a73ebda9c98ed1154da99080d07b711880fcef5c088fd`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd62fafd31e2f1e76e15e2ce615fa4c3cd0b27d0032039ba648b2916dbcd8f67`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d63d3d3f0270f5bb767e3626bb6b77cd56a0ab7caf65ed6f30ef5e9a4635e`  
		Last Modified: Fri, 26 Mar 2021 18:17:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:909fe504f3a8d0ce4382c1f72db0d02f325849e67208e0e53fb3c3365bf4441d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60477245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6561e2eefb88b49f291db74e7620987e227c6f3beac4489dfc5ff03ee9864686`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:36:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:36:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 31 Mar 2021 00:36:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:36:59 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:37:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:37:01 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:37:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:37:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:37:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:37:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f79332eba6d531ed7d7f7098ef5b3c9bdf5b2d226411e34a84af572d7765b5`  
		Last Modified: Wed, 31 Mar 2021 00:38:21 GMT  
		Size: 4.1 MB (4082290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329100e36c1415f1b13f306bca5dc0381c529b1a1b42186141a86b18bd577bcd`  
		Last Modified: Wed, 31 Mar 2021 00:38:31 GMT  
		Size: 36.0 MB (35981251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182347e51ab4f375e0fec2cb9bc9df4ceb68acb4025fc055d5c5b5e71ba4475d`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa0b2d21d61dbe4afda954bb0cced4aecca93c4ac367d1a109cf921bd486080`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a1bbd48a4790e5d7c1f465ae2ef2f934a970b739d2c71fc7bc617c06dce56c`  
		Last Modified: Wed, 31 Mar 2021 00:38:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:2c763ee4efeabcda89d91708e177111bb459c3c4e2174ad697c671d780eec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:428e98a9f624def380648c24e4ab802f136b56e81459119580b83855902bf989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22660462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7abe0632a70257e96d02ebf9c0f8f779291d0eaae40a5d32bbffb313658b2119`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 02:41:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:13 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:14 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:14 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8347978863206fd815b2a3bb0be789f20244679d01952c7cf99a2b62f26e50`  
		Last Modified: Fri, 26 Mar 2021 02:42:27 GMT  
		Size: 19.6 MB (19555255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83be8e29182aea4959f986a45df5392775825ead1857be98fec722452d59eb7`  
		Last Modified: Fri, 26 Mar 2021 02:42:23 GMT  
		Size: 12.3 KB (12272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bba321eed11d28f7c89bf86c98104bfe62a8bdb233953efb77cda61c4b0304`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7060062a0a29d0380f03a272669a9230258bab2dfa7df2d7d90bce2c3f60d60d`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:3522cec94b281d12808ab4a024f6bbe5afb75f1a83311d22e901beb77c174d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:8e062780dc9c65f4a405023d3cf867a815a02011966dba1b6e7e7010c55e6321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70442358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e0d78af7cfe7799b524d498bbf79cfe38695a3fe78fdade083c54baa1744a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:58:06 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 30 Mar 2021 22:58:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:58:23 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:58:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:58:23 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:58:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:58:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb5e63586af7d23e085defc2d66fb6043506fc4207522e583eb8b307cd9d04`  
		Last Modified: Tue, 30 Mar 2021 22:58:59 GMT  
		Size: 6.8 MB (6760089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40855271a33467209bfee7ed24db57e09a01b50b5fe166470d8e011feb03b9d7`  
		Last Modified: Tue, 30 Mar 2021 22:59:51 GMT  
		Size: 41.1 MB (41129609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7143835b82c0e088d61b34fa2b50a904b2369cc726e96fe5e19e2f7b4fdbb7`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d3f836df3a0dbbd04722b3dfe67d79def8f79a1d5f44d8b6a2ad3692d5c736`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0d6617e569b3176a4a46579ee2f1ade418dd6d5a91fd2a7887a19cd057bc1`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1d9df68e91ba20b751f4760c5fabaca38c6874de29207dda7f4c00d5ad9c2e26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63854101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fbcadf2ecd47b50d238dde57fee8d1d24c88122b5207a711bcc5a8a9259a0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:14:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:16:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 18:16:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:16:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:16:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:16:54 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:16:54 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:16:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:16:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59a68a97e8e2d980ebdbd6cc4e0d02a1d682e732f0408185a01f3fc7abef6c`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 5.8 MB (5779536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5855622570678275615b72e95d0c0044a8435e176078aa2dfd1342509bb04aa`  
		Last Modified: Fri, 26 Mar 2021 18:18:05 GMT  
		Size: 38.7 MB (38734547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59cbe06e7c5068580455be04762c45c2d78d22aae1fe3ab4f25ef98c248eaf`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7714a91dfe02bb117af1853e0194f773d5a05041f50e95c2d7d68dfce3b115`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54799bf673eb5a2c297c3b5b50c0b4596c443073e45f523e7456e9f91611d6e4`  
		Last Modified: Fri, 26 Mar 2021 18:17:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:519f13ae5b625134ff1c0e600fce69033081652806b74a55043978578a3ea1f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6683b6ef31a555d4e1c92d045a9fe99288bfd3d0a4f558d36fe891723b47666`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:37:18 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 31 Mar 2021 00:37:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:37:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:37:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:37:42 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:37:43 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:37:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:37:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:37:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fb0292c785020e4d806224fad8e726db9930f08d23b4916773dc04474da75`  
		Last Modified: Wed, 31 Mar 2021 00:38:06 GMT  
		Size: 6.0 MB (6047578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9622c25c19098315bc04704645ecd35a3564e5dfa018eacda6a238933666b0`  
		Last Modified: Wed, 31 Mar 2021 00:38:50 GMT  
		Size: 38.5 MB (38502578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68871724ebaf31349eb1f8344a88dfd08f5816cdfa35350c6cf2f0e47987880e`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506175f0ca8e2948278b1718ee099a65dcf182ec9882267ae7d55454bd937747`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11574cdb39e484768e017e7960d44b048add049f8adfc4e0cf8c9dd1e28a0141`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:3522cec94b281d12808ab4a024f6bbe5afb75f1a83311d22e901beb77c174d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:8e062780dc9c65f4a405023d3cf867a815a02011966dba1b6e7e7010c55e6321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70442358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e0d78af7cfe7799b524d498bbf79cfe38695a3fe78fdade083c54baa1744a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:58:06 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 30 Mar 2021 22:58:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:58:23 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:58:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:58:23 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:58:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:58:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb5e63586af7d23e085defc2d66fb6043506fc4207522e583eb8b307cd9d04`  
		Last Modified: Tue, 30 Mar 2021 22:58:59 GMT  
		Size: 6.8 MB (6760089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40855271a33467209bfee7ed24db57e09a01b50b5fe166470d8e011feb03b9d7`  
		Last Modified: Tue, 30 Mar 2021 22:59:51 GMT  
		Size: 41.1 MB (41129609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7143835b82c0e088d61b34fa2b50a904b2369cc726e96fe5e19e2f7b4fdbb7`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d3f836df3a0dbbd04722b3dfe67d79def8f79a1d5f44d8b6a2ad3692d5c736`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0d6617e569b3176a4a46579ee2f1ade418dd6d5a91fd2a7887a19cd057bc1`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1d9df68e91ba20b751f4760c5fabaca38c6874de29207dda7f4c00d5ad9c2e26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63854101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fbcadf2ecd47b50d238dde57fee8d1d24c88122b5207a711bcc5a8a9259a0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:14:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:16:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 18:16:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:16:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:16:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:16:54 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:16:54 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:16:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:16:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59a68a97e8e2d980ebdbd6cc4e0d02a1d682e732f0408185a01f3fc7abef6c`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 5.8 MB (5779536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5855622570678275615b72e95d0c0044a8435e176078aa2dfd1342509bb04aa`  
		Last Modified: Fri, 26 Mar 2021 18:18:05 GMT  
		Size: 38.7 MB (38734547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59cbe06e7c5068580455be04762c45c2d78d22aae1fe3ab4f25ef98c248eaf`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7714a91dfe02bb117af1853e0194f773d5a05041f50e95c2d7d68dfce3b115`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54799bf673eb5a2c297c3b5b50c0b4596c443073e45f523e7456e9f91611d6e4`  
		Last Modified: Fri, 26 Mar 2021 18:17:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:519f13ae5b625134ff1c0e600fce69033081652806b74a55043978578a3ea1f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6683b6ef31a555d4e1c92d045a9fe99288bfd3d0a4f558d36fe891723b47666`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:37:18 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 31 Mar 2021 00:37:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:37:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:37:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:37:42 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:37:43 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:37:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:37:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:37:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fb0292c785020e4d806224fad8e726db9930f08d23b4916773dc04474da75`  
		Last Modified: Wed, 31 Mar 2021 00:38:06 GMT  
		Size: 6.0 MB (6047578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9622c25c19098315bc04704645ecd35a3564e5dfa018eacda6a238933666b0`  
		Last Modified: Wed, 31 Mar 2021 00:38:50 GMT  
		Size: 38.5 MB (38502578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68871724ebaf31349eb1f8344a88dfd08f5816cdfa35350c6cf2f0e47987880e`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506175f0ca8e2948278b1718ee099a65dcf182ec9882267ae7d55454bd937747`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11574cdb39e484768e017e7960d44b048add049f8adfc4e0cf8c9dd1e28a0141`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:3522cec94b281d12808ab4a024f6bbe5afb75f1a83311d22e901beb77c174d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:8e062780dc9c65f4a405023d3cf867a815a02011966dba1b6e7e7010c55e6321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70442358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e0d78af7cfe7799b524d498bbf79cfe38695a3fe78fdade083c54baa1744a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:57:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Mar 2021 22:58:06 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 30 Mar 2021 22:58:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 30 Mar 2021 22:58:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 30 Mar 2021 22:58:23 GMT
EXPOSE 8888
# Tue, 30 Mar 2021 22:58:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 30 Mar 2021 22:58:23 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 30 Mar 2021 22:58:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Mar 2021 22:58:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb5e63586af7d23e085defc2d66fb6043506fc4207522e583eb8b307cd9d04`  
		Last Modified: Tue, 30 Mar 2021 22:58:59 GMT  
		Size: 6.8 MB (6760089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40855271a33467209bfee7ed24db57e09a01b50b5fe166470d8e011feb03b9d7`  
		Last Modified: Tue, 30 Mar 2021 22:59:51 GMT  
		Size: 41.1 MB (41129609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7143835b82c0e088d61b34fa2b50a904b2369cc726e96fe5e19e2f7b4fdbb7`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d3f836df3a0dbbd04722b3dfe67d79def8f79a1d5f44d8b6a2ad3692d5c736`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0d6617e569b3176a4a46579ee2f1ade418dd6d5a91fd2a7887a19cd057bc1`  
		Last Modified: Tue, 30 Mar 2021 22:59:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1d9df68e91ba20b751f4760c5fabaca38c6874de29207dda7f4c00d5ad9c2e26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63854101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fbcadf2ecd47b50d238dde57fee8d1d24c88122b5207a711bcc5a8a9259a0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:47 GMT
ADD file:b1a5bfd28534bad7b8c5855866772582382ed83f0066f18ee2a8641adfd9ba0c in / 
# Fri, 26 Mar 2021 11:22:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:14:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 26 Mar 2021 18:16:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 18:16:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:16:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 18:16:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 18:16:54 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 18:16:54 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 18:16:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 26 Mar 2021 18:16:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f45436284e34e941cb0711d5901be5a1fd36d7b444c793225978d28caa2fe50c`  
		Last Modified: Fri, 26 Mar 2021 11:31:36 GMT  
		Size: 19.3 MB (19315624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59a68a97e8e2d980ebdbd6cc4e0d02a1d682e732f0408185a01f3fc7abef6c`  
		Last Modified: Fri, 26 Mar 2021 18:17:19 GMT  
		Size: 5.8 MB (5779536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5855622570678275615b72e95d0c0044a8435e176078aa2dfd1342509bb04aa`  
		Last Modified: Fri, 26 Mar 2021 18:18:05 GMT  
		Size: 38.7 MB (38734547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59cbe06e7c5068580455be04762c45c2d78d22aae1fe3ab4f25ef98c248eaf`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7714a91dfe02bb117af1853e0194f773d5a05041f50e95c2d7d68dfce3b115`  
		Last Modified: Fri, 26 Mar 2021 18:17:53 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54799bf673eb5a2c297c3b5b50c0b4596c443073e45f523e7456e9f91611d6e4`  
		Last Modified: Fri, 26 Mar 2021 18:17:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:519f13ae5b625134ff1c0e600fce69033081652806b74a55043978578a3ea1f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6683b6ef31a555d4e1c92d045a9fe99288bfd3d0a4f558d36fe891723b47666`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:13 GMT
ADD file:6c50a12d856589b3002e4262ecb952f6fe3fd89eddc1f9c23391aa0f6228f6ac in / 
# Tue, 30 Mar 2021 21:50:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 00:37:18 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 31 Mar 2021 00:37:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:37:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 31 Mar 2021 00:37:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 31 Mar 2021 00:37:42 GMT
EXPOSE 8888
# Wed, 31 Mar 2021 00:37:43 GMT
VOLUME [/var/lib/chronograf]
# Wed, 31 Mar 2021 00:37:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 31 Mar 2021 00:37:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 00:37:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:723b7d0e9b209513e3eedf36e7b5f2cab85bc1bb7d8fbee1286ee2a0e982ddda`  
		Last Modified: Tue, 30 Mar 2021 21:57:06 GMT  
		Size: 20.4 MB (20389310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fb0292c785020e4d806224fad8e726db9930f08d23b4916773dc04474da75`  
		Last Modified: Wed, 31 Mar 2021 00:38:06 GMT  
		Size: 6.0 MB (6047578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9622c25c19098315bc04704645ecd35a3564e5dfa018eacda6a238933666b0`  
		Last Modified: Wed, 31 Mar 2021 00:38:50 GMT  
		Size: 38.5 MB (38502578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68871724ebaf31349eb1f8344a88dfd08f5816cdfa35350c6cf2f0e47987880e`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506175f0ca8e2948278b1718ee099a65dcf182ec9882267ae7d55454bd937747`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11574cdb39e484768e017e7960d44b048add049f8adfc4e0cf8c9dd1e28a0141`  
		Last Modified: Wed, 31 Mar 2021 00:38:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
