## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:fadccb99469503ee4f85ea645c7ba7b089ceca3e84579ba8e3020cf74b471192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:8cec39c7e37b50b3be9dc84f2ba9f9f5576d12f783831f36ba1e4710e30d4ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131079997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a6b621879d2018577667232c282eacf43111abe9574cd0c092135248997054`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Dec 2022 10:19:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 09 Dec 2022 10:20:00 GMT
ENV KAPACITOR_VERSION=1.6.5
# Fri, 09 Dec 2022 10:20:06 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 09 Dec 2022 10:20:07 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 09 Dec 2022 10:20:07 GMT
EXPOSE 9092
# Fri, 09 Dec 2022 10:20:07 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 09 Dec 2022 10:20:07 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 09 Dec 2022 10:20:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 09 Dec 2022 10:20:07 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c825b7c3eae2da575dfc0111b7abc127cac7fcabaad79f8ca7857c9ad282bda`  
		Last Modified: Fri, 09 Dec 2022 04:09:36 GMT  
		Size: 3.8 MB (3787753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a67ff2d29bee7f9b37c848edd6de7d644c3af0844afa2acaa3f8a4964957db`  
		Last Modified: Fri, 09 Dec 2022 04:09:36 GMT  
		Size: 3.6 MB (3561295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7efe91e59e7ddb3a591370ed7071dc5b5afb7f277f5f35ce15086f7f6ba868`  
		Last Modified: Fri, 09 Dec 2022 10:20:30 GMT  
		Size: 28.9 MB (28885453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47588d010403f158218c7513ca34204143423f5d934d01d643213de5880d5d58`  
		Last Modified: Fri, 09 Dec 2022 10:20:35 GMT  
		Size: 64.4 MB (64416332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd480ac8c32b0176fa2af5ea1409428d27f906be92425d4340b275b71c183e31`  
		Last Modified: Fri, 09 Dec 2022 10:20:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf53978fddf30b6e6718c3606c522fa381182e0f3a7fd7f485049f175874d04`  
		Last Modified: Fri, 09 Dec 2022 10:20:28 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0d202794e90aa9cac4ebc8210b8bff8948c52db8b6daa8413a5b1a2844a9ba68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125753937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be024843d4fc23b11425b5a25f0e793b0aef4e93f75afd016dab47d11e87d448`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 15:28:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 28 Apr 2023 22:39:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 28 Apr 2023 22:39:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 28 Apr 2023 22:39:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 22:39:45 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 22:39:46 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 22:39:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 28 Apr 2023 22:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 22:39:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a850c5eb17a3306f80957da70d5ca3d4e3aa30f97841e250decbd2c26c96c7`  
		Last Modified: Fri, 28 Apr 2023 22:39:57 GMT  
		Size: 28.4 MB (28400052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27994f0f01f7feaf072bc712d7065f3e49f31eb73e0c27c3773e09c44f3f206`  
		Last Modified: Fri, 28 Apr 2023 22:40:11 GMT  
		Size: 61.7 MB (61669186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9100f7f3c836715a691372724cd232b089f8734d9d9cf040eabab86a25aad5b`  
		Last Modified: Fri, 28 Apr 2023 22:40:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9aac8efdd51c3dd42848ae5c3ab1dbd047e6ac9818d768bdbc4249ea20940a`  
		Last Modified: Fri, 28 Apr 2023 22:40:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
