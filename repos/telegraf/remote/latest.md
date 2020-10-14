## `telegraf:latest`

```console
$ docker pull telegraf@sha256:3c3f13cad208ebd34fde683f1403c71428a74305ab86d586fd6d96cbed7c6479
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:655213a2041fb9eed5e8129baac75bc460005fb1f4ead6d7f3ddafd4bc884a89
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107283129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a36634a1efd7bcec80d2844ea5d7eb2b50f8e09cf5e2253534b0d9f56252e8a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 22:44:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:44:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 22:44:35 GMT
ENV TELEGRAF_VERSION=1.15.3
# Tue, 13 Oct 2020 22:44:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Oct 2020 22:44:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Oct 2020 22:44:40 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 13 Oct 2020 22:44:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 22:44:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9d3d4ee2cf178895c34ba3484e9620e7c241f8075dcf9aae610b1a33b2bef`  
		Last Modified: Tue, 13 Oct 2020 22:45:23 GMT  
		Size: 17.4 MB (17411706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe6b63091110a764935bedc335698000213e2bc4aaf334b6da2060639bf8027`  
		Last Modified: Tue, 13 Oct 2020 22:45:19 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f290c098c42b1eac131bb77b9e06fa9e797427e11d215f02e2b4c60089614cc`  
		Last Modified: Tue, 13 Oct 2020 22:45:25 GMT  
		Size: 21.7 MB (21664326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbbf75e5be78e0e096bde03713ee087ce97fb096d764fe1a4b11c7416465458`  
		Last Modified: Tue, 13 Oct 2020 22:45:19 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f0665c76213e129ceba8d76443011ea8332d850ebc3749577cd498f141bed7d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98874910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2377be38187aed7f12befaa3bd46679c22912ed01e9a4baecf1ded0e4335f20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:02 GMT
ADD file:e03270d36cef8171f1f6303860ff31bb1c0eb10642b8173bfdfef9f77fa4f89c in / 
# Tue, 13 Oct 2020 00:59:04 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 01:34:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 23:13:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 23:13:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 23:13:25 GMT
ENV TELEGRAF_VERSION=1.15.3
# Tue, 13 Oct 2020 23:13:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Oct 2020 23:13:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Oct 2020 23:13:36 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 13 Oct 2020 23:13:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 23:13:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5c0fdcca2cbb5e316a288f39c8c2006f45544568ea04623c036e0b1faa066bbe`  
		Last Modified: Tue, 13 Oct 2020 01:08:04 GMT  
		Size: 45.9 MB (45869258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8216e147de931a74896e75f60d0a331dd1438bc1ae4b2d4c29c8017548e8dcbd`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 7.1 MB (7097763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf6642121709e17d1419901978da7d29b673d5f936e42ec3241b7d7157e9541`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 9.3 MB (9343130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6a0d3562077749d37b0c9fc2fc28a538b7e7eb94ccea5e858358c15828841b`  
		Last Modified: Tue, 13 Oct 2020 23:14:38 GMT  
		Size: 16.2 MB (16158104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d734f702ca00ac70d67b7c72628aca0ab61bf44ea7d503e6050ae5e9b50d65e`  
		Last Modified: Tue, 13 Oct 2020 23:14:32 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878a78c842d18143a8f8d5576bc893edecde1b2de6b2750d6ad1a78ebe30f025`  
		Last Modified: Tue, 13 Oct 2020 23:14:39 GMT  
		Size: 20.4 MB (20403573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530015d40afc7430d7f08dac88254a3c82add482046e5e11261b1c095e13ea6f`  
		Last Modified: Tue, 13 Oct 2020 23:14:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:28fb4583d35fa39690bf84934165d41bb7f8d62686490fc87e149a5261abd6b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104133674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f67b82d5a3c132e3e7ea18e2fa7719b02cf7e09ca18985ece6c748fda04ea9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:33:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Oct 2020 02:15:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 02:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 14 Oct 2020 02:15:05 GMT
ENV TELEGRAF_VERSION=1.15.3
# Wed, 14 Oct 2020 02:15:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Oct 2020 02:15:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Oct 2020 02:15:11 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 14 Oct 2020 02:15:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Oct 2020 02:15:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d6e4f4b17bdbefbe60820da5f5711a26d31c075dc69bcaf9b077d7d29262d`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 7.7 MB (7681432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db65b8364fc73072a0d5b51199cc9c6b108b4229d92e784b92ae67898dd0bd`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 10.0 MB (9983936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e9a06b1254ac01a06e12efe2c55dd39f040017adf07ce8f6949dd06948ef1`  
		Last Modified: Wed, 14 Oct 2020 02:16:03 GMT  
		Size: 17.3 MB (17270065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed886e7e1546ecbc743ef4320f25c4709e68c90b33afbf9fe8cdfafc6b94449`  
		Last Modified: Wed, 14 Oct 2020 02:15:58 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf173c8dac3923a1f4503ed1c98790fde061e9270ed3c399f756b7ca7310392`  
		Last Modified: Wed, 14 Oct 2020 02:16:04 GMT  
		Size: 20.0 MB (20019753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec746eecb72b689b4c481f75c05f185d59863561988f01d0fdad476bbb50352`  
		Last Modified: Wed, 14 Oct 2020 02:15:58 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
