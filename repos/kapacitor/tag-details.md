<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.5`](#kapacitor165)
-	[`kapacitor:1.6.5-alpine`](#kapacitor165-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:35201623bdb82092c25a4f8c408de8a1ef2ea07ff738aac93d213b44cf550c80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:d69918dde8206b8093ebf4232f85cd3e2cf38db0f848b26e6005bb932a667011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111735184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc00b6e833611385f4ceb08786c82eb15567465e1a82839a32e1f010206afe22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:23:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Jun 2022 15:23:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:23:16 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 23 Jun 2022 15:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Jun 2022 15:23:21 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Jun 2022 15:23:21 GMT
EXPOSE 9092
# Thu, 23 Jun 2022 15:23:22 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Jun 2022 15:23:22 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Jun 2022 15:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:23:22 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ca30eaa3f2e4a14053445907d290c9e29fe087a4cd7f7607ea7ced493a2405`  
		Last Modified: Thu, 23 Jun 2022 15:23:51 GMT  
		Size: 13.4 MB (13436157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88da6edad4b4d98978e4fd397110c9d2f14f317fd3846dc196f8d8c95d1ba632`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb7eb8e6acbbca57e804e463d57e0e255e32445eeaaddc76c8e5a910ee927e`  
		Last Modified: Thu, 23 Jun 2022 15:23:54 GMT  
		Size: 37.2 MB (37219849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed57900e7789f09136c4dbf3c3848e6f4ddf2d4cc4d75afe52c633a40c72470`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a2e325e760c8c507dfb8d86f51accfe003b032a99742ef67b8816a676277c6`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d29dd39b2509a274e47e34def46e91d08c25011757dbfcf420e2080f83964ad4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104444245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680ab7c21ef4f4b0085727d6799e65396319c9fc49ffcb3efd5ce1f7bd29275b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:04 GMT
ADD file:4f45aa06c6a1c011e41ff7e4685f05d91970973768fc88ff3e825c5ac4fd6058 in / 
# Thu, 23 Jun 2022 01:05:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:58:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 03 Nov 2022 02:05:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 03 Nov 2022 02:05:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 03 Nov 2022 02:05:52 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 03 Nov 2022 02:05:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 03 Nov 2022 02:05:57 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 03 Nov 2022 02:05:57 GMT
EXPOSE 9092
# Thu, 03 Nov 2022 02:05:57 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 03 Nov 2022 02:05:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 03 Nov 2022 02:05:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Nov 2022 02:05:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cf35481e5c316d184dac1873898948d1e8108de590a2a940c32cda34173fe7c1`  
		Last Modified: Thu, 23 Jun 2022 01:22:04 GMT  
		Size: 42.2 MB (42150850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b740b174e94fb77095522004355bb6f430f0b25308acd5fc66d325f04f99c6`  
		Last Modified: Thu, 23 Jun 2022 02:21:27 GMT  
		Size: 10.0 MB (9957097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf98bd2fdfbc26a0f8c12d47c32e612d01389ff5e4aafc52aa04b72381a6c823`  
		Last Modified: Thu, 23 Jun 2022 02:21:24 GMT  
		Size: 3.9 MB (3921761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221501dcc1cbba3a57c72c6665204f7bd3633b4569913bd2e8813c3edb7e2a3`  
		Last Modified: Thu, 03 Nov 2022 02:06:15 GMT  
		Size: 13.6 MB (13624191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598da3f44ca1db3c0b3f8df98044d7a44573979648831775f61d39679227e956`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969be022826da8731ee8be86e2d9e1fc3cfd162ceda3d1f77b409715824c9692`  
		Last Modified: Thu, 03 Nov 2022 02:06:19 GMT  
		Size: 34.8 MB (34787064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90a9f00436060d3345b2b7a656647b21bcbef1a32961636921667347ffddb0b`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ebbe9546bb850a732deee548f071230cbe7a3c0bdcd1261b89b6205db38846`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3b3c78b8b4beb18b11602334a681eb1cb7a77830f0ec005de66c2a4684069631
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105016315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fde7e90a39afe526533c8d43e1cdc16449875fcf799ba44022eff7821345917`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:45 GMT
ADD file:3d8b1da94fcec5d068e3e6465fac70cce404c331bb52e30a5bf7cbd950baa5fe in / 
# Thu, 23 Jun 2022 00:42:45 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Oct 2022 09:32:16 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 26 Oct 2022 09:32:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Oct 2022 09:32:19 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 26 Oct 2022 09:32:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 26 Oct 2022 09:32:23 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 26 Oct 2022 09:32:23 GMT
EXPOSE 9092
# Wed, 26 Oct 2022 09:32:23 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 26 Oct 2022 09:32:23 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 26 Oct 2022 09:32:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 09:32:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d8ccec8a513f896fedd1d9765f3f2abf98bc8264f61cecf17919c80c9aa7ddbc`  
		Last Modified: Thu, 23 Jun 2022 00:51:18 GMT  
		Size: 43.2 MB (43213121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40625a6bb21cb2cd6b19ef7592951f90da9ea1d8abf359196bf48300c448b2`  
		Last Modified: Thu, 23 Jun 2022 01:25:28 GMT  
		Size: 10.2 MB (10218617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414226169d0f92fdcd77314cbd06ba7613675d62a3afd63aa88afbf0072c44c2`  
		Last Modified: Thu, 23 Jun 2022 01:25:27 GMT  
		Size: 3.9 MB (3874558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91e2ccc056ea41305b36e42a264023057da389f2a2587e6ab2b12ee209a82fd`  
		Last Modified: Wed, 26 Oct 2022 09:33:01 GMT  
		Size: 13.1 MB (13145056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c77f85e8621dc2475281878b1bea96078e265e411253c2b3a238aa0333a701`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17792d61932724fad60cec861dde378e6452226f1942e4f8faae22141dbafdbb`  
		Last Modified: Wed, 26 Oct 2022 09:33:03 GMT  
		Size: 34.6 MB (34561653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d03aec48eac8c13081a87c9626c4df2b24913ccbfee52365c12fa9ef157a28`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92518b99b158a694fccdfad0381c809c1def182c78badbf86e2642cd0cf253b`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:f0f31429af6264e22af1e8775ee4f5b068f8c252dbb12a18dc7ca8bca6021e17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:19babd50485107fc60c68c5575e10fcfcaab84a061f1f8d33c8777f89a83f67e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22653543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4c0dc3fc30734367b70939eab1f65f2b9415e94acb5a2a30ddbcd7cd9ff4a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:59:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 06 Oct 2022 22:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:59:32 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 06 Oct 2022 22:59:32 GMT
EXPOSE 9092
# Thu, 06 Oct 2022 22:59:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 06 Oct 2022 22:59:32 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 06 Oct 2022 22:59:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:59:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae6d710af90b1b33cb522971dfe089e2211f3ab1ca3fd49c413a6abb65bca3`  
		Last Modified: Thu, 06 Oct 2022 23:00:14 GMT  
		Size: 19.5 MB (19540837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824abcf1a6f5277dc3c036fcbd7fd7fe396a7e46833634600dd503e0dbb06cff`  
		Last Modified: Thu, 06 Oct 2022 23:00:11 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85cbf909734bf9f5784fa910bb4cd8b7b1dd2121001a8a1a34362ba54ae46e`  
		Last Modified: Thu, 06 Oct 2022 23:00:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:35201623bdb82092c25a4f8c408de8a1ef2ea07ff738aac93d213b44cf550c80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:d69918dde8206b8093ebf4232f85cd3e2cf38db0f848b26e6005bb932a667011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111735184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc00b6e833611385f4ceb08786c82eb15567465e1a82839a32e1f010206afe22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:23:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Jun 2022 15:23:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:23:16 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 23 Jun 2022 15:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Jun 2022 15:23:21 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Jun 2022 15:23:21 GMT
EXPOSE 9092
# Thu, 23 Jun 2022 15:23:22 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Jun 2022 15:23:22 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Jun 2022 15:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:23:22 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ca30eaa3f2e4a14053445907d290c9e29fe087a4cd7f7607ea7ced493a2405`  
		Last Modified: Thu, 23 Jun 2022 15:23:51 GMT  
		Size: 13.4 MB (13436157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88da6edad4b4d98978e4fd397110c9d2f14f317fd3846dc196f8d8c95d1ba632`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb7eb8e6acbbca57e804e463d57e0e255e32445eeaaddc76c8e5a910ee927e`  
		Last Modified: Thu, 23 Jun 2022 15:23:54 GMT  
		Size: 37.2 MB (37219849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed57900e7789f09136c4dbf3c3848e6f4ddf2d4cc4d75afe52c633a40c72470`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a2e325e760c8c507dfb8d86f51accfe003b032a99742ef67b8816a676277c6`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d29dd39b2509a274e47e34def46e91d08c25011757dbfcf420e2080f83964ad4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104444245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680ab7c21ef4f4b0085727d6799e65396319c9fc49ffcb3efd5ce1f7bd29275b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:04 GMT
ADD file:4f45aa06c6a1c011e41ff7e4685f05d91970973768fc88ff3e825c5ac4fd6058 in / 
# Thu, 23 Jun 2022 01:05:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:58:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 03 Nov 2022 02:05:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 03 Nov 2022 02:05:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 03 Nov 2022 02:05:52 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 03 Nov 2022 02:05:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 03 Nov 2022 02:05:57 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 03 Nov 2022 02:05:57 GMT
EXPOSE 9092
# Thu, 03 Nov 2022 02:05:57 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 03 Nov 2022 02:05:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 03 Nov 2022 02:05:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Nov 2022 02:05:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cf35481e5c316d184dac1873898948d1e8108de590a2a940c32cda34173fe7c1`  
		Last Modified: Thu, 23 Jun 2022 01:22:04 GMT  
		Size: 42.2 MB (42150850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b740b174e94fb77095522004355bb6f430f0b25308acd5fc66d325f04f99c6`  
		Last Modified: Thu, 23 Jun 2022 02:21:27 GMT  
		Size: 10.0 MB (9957097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf98bd2fdfbc26a0f8c12d47c32e612d01389ff5e4aafc52aa04b72381a6c823`  
		Last Modified: Thu, 23 Jun 2022 02:21:24 GMT  
		Size: 3.9 MB (3921761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221501dcc1cbba3a57c72c6665204f7bd3633b4569913bd2e8813c3edb7e2a3`  
		Last Modified: Thu, 03 Nov 2022 02:06:15 GMT  
		Size: 13.6 MB (13624191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598da3f44ca1db3c0b3f8df98044d7a44573979648831775f61d39679227e956`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969be022826da8731ee8be86e2d9e1fc3cfd162ceda3d1f77b409715824c9692`  
		Last Modified: Thu, 03 Nov 2022 02:06:19 GMT  
		Size: 34.8 MB (34787064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90a9f00436060d3345b2b7a656647b21bcbef1a32961636921667347ffddb0b`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ebbe9546bb850a732deee548f071230cbe7a3c0bdcd1261b89b6205db38846`  
		Last Modified: Thu, 03 Nov 2022 02:06:14 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3b3c78b8b4beb18b11602334a681eb1cb7a77830f0ec005de66c2a4684069631
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105016315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fde7e90a39afe526533c8d43e1cdc16449875fcf799ba44022eff7821345917`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:45 GMT
ADD file:3d8b1da94fcec5d068e3e6465fac70cce404c331bb52e30a5bf7cbd950baa5fe in / 
# Thu, 23 Jun 2022 00:42:45 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Oct 2022 09:32:16 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 26 Oct 2022 09:32:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Oct 2022 09:32:19 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 26 Oct 2022 09:32:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 26 Oct 2022 09:32:23 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 26 Oct 2022 09:32:23 GMT
EXPOSE 9092
# Wed, 26 Oct 2022 09:32:23 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 26 Oct 2022 09:32:23 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 26 Oct 2022 09:32:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 09:32:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d8ccec8a513f896fedd1d9765f3f2abf98bc8264f61cecf17919c80c9aa7ddbc`  
		Last Modified: Thu, 23 Jun 2022 00:51:18 GMT  
		Size: 43.2 MB (43213121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40625a6bb21cb2cd6b19ef7592951f90da9ea1d8abf359196bf48300c448b2`  
		Last Modified: Thu, 23 Jun 2022 01:25:28 GMT  
		Size: 10.2 MB (10218617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414226169d0f92fdcd77314cbd06ba7613675d62a3afd63aa88afbf0072c44c2`  
		Last Modified: Thu, 23 Jun 2022 01:25:27 GMT  
		Size: 3.9 MB (3874558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91e2ccc056ea41305b36e42a264023057da389f2a2587e6ab2b12ee209a82fd`  
		Last Modified: Wed, 26 Oct 2022 09:33:01 GMT  
		Size: 13.1 MB (13145056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c77f85e8621dc2475281878b1bea96078e265e411253c2b3a238aa0333a701`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17792d61932724fad60cec861dde378e6452226f1942e4f8faae22141dbafdbb`  
		Last Modified: Wed, 26 Oct 2022 09:33:03 GMT  
		Size: 34.6 MB (34561653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d03aec48eac8c13081a87c9626c4df2b24913ccbfee52365c12fa9ef157a28`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92518b99b158a694fccdfad0381c809c1def182c78badbf86e2642cd0cf253b`  
		Last Modified: Wed, 26 Oct 2022 09:33:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:f0f31429af6264e22af1e8775ee4f5b068f8c252dbb12a18dc7ca8bca6021e17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:19babd50485107fc60c68c5575e10fcfcaab84a061f1f8d33c8777f89a83f67e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22653543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4c0dc3fc30734367b70939eab1f65f2b9415e94acb5a2a30ddbcd7cd9ff4a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:59:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 06 Oct 2022 22:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:59:32 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 06 Oct 2022 22:59:32 GMT
EXPOSE 9092
# Thu, 06 Oct 2022 22:59:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 06 Oct 2022 22:59:32 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 06 Oct 2022 22:59:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:59:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae6d710af90b1b33cb522971dfe089e2211f3ab1ca3fd49c413a6abb65bca3`  
		Last Modified: Thu, 06 Oct 2022 23:00:14 GMT  
		Size: 19.5 MB (19540837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824abcf1a6f5277dc3c036fcbd7fd7fe396a7e46833634600dd503e0dbb06cff`  
		Last Modified: Thu, 06 Oct 2022 23:00:11 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85cbf909734bf9f5784fa910bb4cd8b7b1dd2121001a8a1a34362ba54ae46e`  
		Last Modified: Thu, 06 Oct 2022 23:00:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:da5b8e7bf0af1926d5094be5b3211758fee6decdc2e522e8b6057f10ca509bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:5861c0f972ca245dc6815103970cdb83ad62fae99a115de30dc6e19f50a9a03b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130650925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32bc2fab6d4cd5fa517effd6cd7d3553740b70e95a24dcbbfc7a21048b2e9e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:46:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:46:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:28:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:28:26 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:28:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:28:34 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:28:34 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:28:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a586f3d84de83b25cb9ca6d0e733d37d5283da35a837917e355f58833d27462`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.8 MB (3802823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac951de24f647413f348bfa4183b92c9962b167e0a3106d62300e97e4e88654`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.6 MB (3561223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4963b3f490e45446d36fdcd903a1c4172f4a1b1ec613148a3d72af489b6e89ca`  
		Last Modified: Wed, 02 Nov 2022 22:29:01 GMT  
		Size: 28.4 MB (28444534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b00314ef588c3820e8c84d46d2c50d720001723b841b136ce3feeb892036f92`  
		Last Modified: Wed, 02 Nov 2022 22:29:06 GMT  
		Size: 64.4 MB (64416281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2819edb7c604ca85ce1a48b9ea64588a17cd36160fd20d7c46ff812aa7809cef`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f0f8aa00c852a177c0c87c18cb45fdb504d9b0348aa0ac82ca36dd60a32cd`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:96db1ec56d1b9575a331736439b62a54f5d63adb120aebf0b1f9e200ffe9e925
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123381624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46652ebf59b8e50e9a4aad474725abf4b8b24a7c0c94e59cca26062d4c384747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:13:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:13:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:24:06 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:24:06 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:24:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:24:12 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:24:12 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:24:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:24:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313e8e06ef8938592eca84285a9592b5da4d25cb766e00353478f2a1bd1dd8e`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.8 MB (3774632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22acfa173fc250378a2f68d88a2bac0cfd1a06b5d9a844cf759b6411eb97fa48`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.5 MB (3535434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6621535dc4786df7ba10f9deb87a69f222185db056882f31537efd3833115`  
		Last Modified: Wed, 02 Nov 2022 22:24:29 GMT  
		Size: 26.8 MB (26768028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4d0f89e444d6d84d4c42e6f85111b001e6abe6abc004b7680d76c216bfd6de`  
		Last Modified: Wed, 02 Nov 2022 22:24:32 GMT  
		Size: 60.9 MB (60920919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156912e8f18c480a177b5e66d6fd64b0c8d0ae509f4f1a8b797e23dca446102c`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabd747c93b7c69d7c5ebdddc0611518b4ac949a1048a473fefbb48f085d9865`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:f2d77c86a9680f182d016c5eef51dcd039cd59a1f2dee8f1cc6b3e957519a812
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:e27445333bd7864ded5eba8f62c29e860e39bf6794201899c8b980587c676691
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67432365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6b500e445a620ee787bbfcdb314860d5713e0793b51a8cd8c1cc4b0dcaa562`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:59:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:59:38 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:59:38 GMT
ENV KAPACITOR_VERSION=1.6.5
# Thu, 06 Oct 2022 22:59:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 06 Oct 2022 22:59:51 GMT
EXPOSE 9092
# Thu, 06 Oct 2022 22:59:51 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 06 Oct 2022 22:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:59:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d30442cf8411e7f53657b11f2e08ef81065f359c49d13af3d255eb9ce50bd8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91274948dd8749eb88a1567b409dd579615c0d678f7154f95f15ddd03222163c`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 284.7 KB (284738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6038b15547c18f4ea2106297dda7195c2b4c68475ccc5765d20eb45abf50fc`  
		Last Modified: Thu, 06 Oct 2022 23:00:32 GMT  
		Size: 64.3 MB (64340964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2054ab7ab071cb17595fc05391099ad825cb1cb7a486d8594f8f3014fb0758e8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf528e02578aa4e995f00e5ea98eb572d949fb4748318ea2d11b15d6a3b28d`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.5`

```console
$ docker pull kapacitor@sha256:da5b8e7bf0af1926d5094be5b3211758fee6decdc2e522e8b6057f10ca509bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:5861c0f972ca245dc6815103970cdb83ad62fae99a115de30dc6e19f50a9a03b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130650925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32bc2fab6d4cd5fa517effd6cd7d3553740b70e95a24dcbbfc7a21048b2e9e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:46:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:46:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:28:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:28:26 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:28:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:28:34 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:28:34 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:28:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a586f3d84de83b25cb9ca6d0e733d37d5283da35a837917e355f58833d27462`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.8 MB (3802823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac951de24f647413f348bfa4183b92c9962b167e0a3106d62300e97e4e88654`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.6 MB (3561223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4963b3f490e45446d36fdcd903a1c4172f4a1b1ec613148a3d72af489b6e89ca`  
		Last Modified: Wed, 02 Nov 2022 22:29:01 GMT  
		Size: 28.4 MB (28444534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b00314ef588c3820e8c84d46d2c50d720001723b841b136ce3feeb892036f92`  
		Last Modified: Wed, 02 Nov 2022 22:29:06 GMT  
		Size: 64.4 MB (64416281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2819edb7c604ca85ce1a48b9ea64588a17cd36160fd20d7c46ff812aa7809cef`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f0f8aa00c852a177c0c87c18cb45fdb504d9b0348aa0ac82ca36dd60a32cd`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:96db1ec56d1b9575a331736439b62a54f5d63adb120aebf0b1f9e200ffe9e925
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123381624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46652ebf59b8e50e9a4aad474725abf4b8b24a7c0c94e59cca26062d4c384747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:13:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:13:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:24:06 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:24:06 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:24:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:24:12 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:24:12 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:24:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:24:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313e8e06ef8938592eca84285a9592b5da4d25cb766e00353478f2a1bd1dd8e`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.8 MB (3774632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22acfa173fc250378a2f68d88a2bac0cfd1a06b5d9a844cf759b6411eb97fa48`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.5 MB (3535434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6621535dc4786df7ba10f9deb87a69f222185db056882f31537efd3833115`  
		Last Modified: Wed, 02 Nov 2022 22:24:29 GMT  
		Size: 26.8 MB (26768028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4d0f89e444d6d84d4c42e6f85111b001e6abe6abc004b7680d76c216bfd6de`  
		Last Modified: Wed, 02 Nov 2022 22:24:32 GMT  
		Size: 60.9 MB (60920919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156912e8f18c480a177b5e66d6fd64b0c8d0ae509f4f1a8b797e23dca446102c`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabd747c93b7c69d7c5ebdddc0611518b4ac949a1048a473fefbb48f085d9865`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.5-alpine`

```console
$ docker pull kapacitor@sha256:f2d77c86a9680f182d016c5eef51dcd039cd59a1f2dee8f1cc6b3e957519a812
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:e27445333bd7864ded5eba8f62c29e860e39bf6794201899c8b980587c676691
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67432365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6b500e445a620ee787bbfcdb314860d5713e0793b51a8cd8c1cc4b0dcaa562`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:59:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:59:38 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:59:38 GMT
ENV KAPACITOR_VERSION=1.6.5
# Thu, 06 Oct 2022 22:59:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 06 Oct 2022 22:59:51 GMT
EXPOSE 9092
# Thu, 06 Oct 2022 22:59:51 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 06 Oct 2022 22:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:59:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d30442cf8411e7f53657b11f2e08ef81065f359c49d13af3d255eb9ce50bd8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91274948dd8749eb88a1567b409dd579615c0d678f7154f95f15ddd03222163c`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 284.7 KB (284738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6038b15547c18f4ea2106297dda7195c2b4c68475ccc5765d20eb45abf50fc`  
		Last Modified: Thu, 06 Oct 2022 23:00:32 GMT  
		Size: 64.3 MB (64340964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2054ab7ab071cb17595fc05391099ad825cb1cb7a486d8594f8f3014fb0758e8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf528e02578aa4e995f00e5ea98eb572d949fb4748318ea2d11b15d6a3b28d`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:f2d77c86a9680f182d016c5eef51dcd039cd59a1f2dee8f1cc6b3e957519a812
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:e27445333bd7864ded5eba8f62c29e860e39bf6794201899c8b980587c676691
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67432365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6b500e445a620ee787bbfcdb314860d5713e0793b51a8cd8c1cc4b0dcaa562`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:59:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:59:38 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:59:38 GMT
ENV KAPACITOR_VERSION=1.6.5
# Thu, 06 Oct 2022 22:59:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 06 Oct 2022 22:59:51 GMT
EXPOSE 9092
# Thu, 06 Oct 2022 22:59:51 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 06 Oct 2022 22:59:51 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 06 Oct 2022 22:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:59:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d30442cf8411e7f53657b11f2e08ef81065f359c49d13af3d255eb9ce50bd8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91274948dd8749eb88a1567b409dd579615c0d678f7154f95f15ddd03222163c`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 284.7 KB (284738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6038b15547c18f4ea2106297dda7195c2b4c68475ccc5765d20eb45abf50fc`  
		Last Modified: Thu, 06 Oct 2022 23:00:32 GMT  
		Size: 64.3 MB (64340964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2054ab7ab071cb17595fc05391099ad825cb1cb7a486d8594f8f3014fb0758e8`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf528e02578aa4e995f00e5ea98eb572d949fb4748318ea2d11b15d6a3b28d`  
		Last Modified: Thu, 06 Oct 2022 23:00:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:da5b8e7bf0af1926d5094be5b3211758fee6decdc2e522e8b6057f10ca509bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:5861c0f972ca245dc6815103970cdb83ad62fae99a115de30dc6e19f50a9a03b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130650925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32bc2fab6d4cd5fa517effd6cd7d3553740b70e95a24dcbbfc7a21048b2e9e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:46:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:46:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:28:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:28:26 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:28:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:28:34 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:28:34 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:28:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:28:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a586f3d84de83b25cb9ca6d0e733d37d5283da35a837917e355f58833d27462`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.8 MB (3802823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac951de24f647413f348bfa4183b92c9962b167e0a3106d62300e97e4e88654`  
		Last Modified: Wed, 02 Nov 2022 19:53:55 GMT  
		Size: 3.6 MB (3561223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4963b3f490e45446d36fdcd903a1c4172f4a1b1ec613148a3d72af489b6e89ca`  
		Last Modified: Wed, 02 Nov 2022 22:29:01 GMT  
		Size: 28.4 MB (28444534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b00314ef588c3820e8c84d46d2c50d720001723b841b136ce3feeb892036f92`  
		Last Modified: Wed, 02 Nov 2022 22:29:06 GMT  
		Size: 64.4 MB (64416281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2819edb7c604ca85ce1a48b9ea64588a17cd36160fd20d7c46ff812aa7809cef`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f0f8aa00c852a177c0c87c18cb45fdb504d9b0348aa0ac82ca36dd60a32cd`  
		Last Modified: Wed, 02 Nov 2022 22:28:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:96db1ec56d1b9575a331736439b62a54f5d63adb120aebf0b1f9e200ffe9e925
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123381624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46652ebf59b8e50e9a4aad474725abf4b8b24a7c0c94e59cca26062d4c384747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:13:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:13:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Nov 2022 22:24:06 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 02 Nov 2022 22:24:06 GMT
ENV KAPACITOR_VERSION=1.6.5
# Wed, 02 Nov 2022 22:24:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5 &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 02 Nov 2022 22:24:12 GMT
EXPOSE 9092
# Wed, 02 Nov 2022 22:24:12 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 02 Nov 2022 22:24:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 02 Nov 2022 22:24:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 22:24:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313e8e06ef8938592eca84285a9592b5da4d25cb766e00353478f2a1bd1dd8e`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.8 MB (3774632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22acfa173fc250378a2f68d88a2bac0cfd1a06b5d9a844cf759b6411eb97fa48`  
		Last Modified: Wed, 02 Nov 2022 20:21:47 GMT  
		Size: 3.5 MB (3535434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6621535dc4786df7ba10f9deb87a69f222185db056882f31537efd3833115`  
		Last Modified: Wed, 02 Nov 2022 22:24:29 GMT  
		Size: 26.8 MB (26768028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4d0f89e444d6d84d4c42e6f85111b001e6abe6abc004b7680d76c216bfd6de`  
		Last Modified: Wed, 02 Nov 2022 22:24:32 GMT  
		Size: 60.9 MB (60920919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156912e8f18c480a177b5e66d6fd64b0c8d0ae509f4f1a8b797e23dca446102c`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabd747c93b7c69d7c5ebdddc0611518b4ac949a1048a473fefbb48f085d9865`  
		Last Modified: Wed, 02 Nov 2022 22:24:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
