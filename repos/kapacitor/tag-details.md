<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.4`](#kapacitor14)
-	[`kapacitor:1.4.1`](#kapacitor141)
-	[`kapacitor:1.4.1-alpine`](#kapacitor141-alpine)
-	[`kapacitor:1.4-alpine`](#kapacitor14-alpine)
-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5.8`](#kapacitor158)
-	[`kapacitor:1.5.8-alpine`](#kapacitor158-alpine)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.4`

```console
$ docker pull kapacitor@sha256:d7f45abcf5f65cc3ff77f96eee4d2893db9c544e7adcacb292cf325eecfacb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:ea35a0814241287b07ab4afb003d387f59e28a1e654923dbaec28d594c4ddbae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96930343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896319b28c0c086b0dcdfc39ce22f7b5c631be5c691b66510548e35db346aad7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 00:34:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 06 Feb 2021 00:34:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 00:34:13 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 06 Feb 2021 00:34:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 06 Feb 2021 00:34:18 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 06 Feb 2021 00:34:18 GMT
EXPOSE 9092
# Sat, 06 Feb 2021 00:34:18 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 06 Feb 2021 00:34:18 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 06 Feb 2021 00:34:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 00:34:19 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85448296a98e89417030cbaa2637eb7f3ca25a8c0df10224dddc81b14f2711d2`  
		Last Modified: Sat, 06 Feb 2021 00:34:55 GMT  
		Size: 13.2 MB (13241611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbad8d39af10a56b6a2dc1d95c0d7d9f87dd876a81631246a598023852dace4`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7189a68c404d49db302a2642bd2ac3e361429e3bbd3c9aa74ef93cc312ecbb`  
		Last Modified: Sat, 06 Feb 2021 00:35:00 GMT  
		Size: 22.7 MB (22695022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f595adc8679b76c16b421a7ca34d075145a1530a88976ce09438a3f81dacba`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca817c82b53cb322b3cfc64233b117d62339d3139b26edcdf6c40a1b56f24260`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:abeb475394eb10fe096062e0bffb0988fe2f4fbc9d8e299966ac12ce6604d63b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90202861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae3a16d0cb223c9ce0c9d049699046d127a61380215de6e90397ac6aa8bbde5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:02:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 21:02:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:02:32 GMT
ENV KAPACITOR_VERSION=1.4.1
# Tue, 12 Jan 2021 21:02:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 21:02:40 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Jan 2021 21:02:41 GMT
EXPOSE 9092
# Tue, 12 Jan 2021 21:02:43 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Jan 2021 21:02:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Jan 2021 21:02:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:02:45 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2d8759a0d27be8d9687c637d713b464c4446cee610a2cbb15d6792f82638f6`  
		Last Modified: Tue, 12 Jan 2021 21:03:23 GMT  
		Size: 13.4 MB (13405330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558886d3184a4e4f2c7a648ddcf082ec0e8ff6698bae58dbab4299afb1962c99`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c85a6723838ca952a46231082f6716475b096ce28bb56f73823a86bcee5022`  
		Last Modified: Tue, 12 Jan 2021 21:03:28 GMT  
		Size: 21.3 MB (21308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152de1f8863805f91c68cce798bd457881406face53344bc1c6b43d460aca28b`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def7f2f2c217322b3c0d141a7cf0a1d356795925086d8dc5138751cb059f0b`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:751985a16160d8d26dd557db05da0a999d619f60665144be480b1411e766406b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91222429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b42704b208f14159d9def4c6dd3e9ffbb3cdacd5956b27d282d3240b632929d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:32:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 23:32:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:32:26 GMT
ENV KAPACITOR_VERSION=1.4.1
# Tue, 12 Jan 2021 23:32:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 23:32:32 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Jan 2021 23:32:32 GMT
EXPOSE 9092
# Tue, 12 Jan 2021 23:32:33 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Jan 2021 23:32:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Jan 2021 23:32:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:32:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa62402c1259a03b7eacd6e8fe73e36ef197604f27fc96f1bc658fa58b67133`  
		Last Modified: Tue, 12 Jan 2021 23:33:14 GMT  
		Size: 12.9 MB (12934117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e787fe247913d0877422c3e4188d63d876cc27ddb8308beab0429165b5c17ce4`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2650892e5c87dbf490593d8f4a5e5a46cff5ca6601991ef5c1a1577812c1c919`  
		Last Modified: Tue, 12 Jan 2021 23:33:19 GMT  
		Size: 21.3 MB (21307930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58ea90b6db7de02310be568f3135ff5c37dbae9068832c1dbc4bb48eeb92eb2`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49e988c34ed7b3c3c779794b622bd81edda6b5eba70930be20ca31b992052f`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1`

```console
$ docker pull kapacitor@sha256:d7f45abcf5f65cc3ff77f96eee4d2893db9c544e7adcacb292cf325eecfacb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:ea35a0814241287b07ab4afb003d387f59e28a1e654923dbaec28d594c4ddbae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96930343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896319b28c0c086b0dcdfc39ce22f7b5c631be5c691b66510548e35db346aad7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 00:34:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 06 Feb 2021 00:34:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 00:34:13 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 06 Feb 2021 00:34:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 06 Feb 2021 00:34:18 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 06 Feb 2021 00:34:18 GMT
EXPOSE 9092
# Sat, 06 Feb 2021 00:34:18 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 06 Feb 2021 00:34:18 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 06 Feb 2021 00:34:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 00:34:19 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85448296a98e89417030cbaa2637eb7f3ca25a8c0df10224dddc81b14f2711d2`  
		Last Modified: Sat, 06 Feb 2021 00:34:55 GMT  
		Size: 13.2 MB (13241611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbad8d39af10a56b6a2dc1d95c0d7d9f87dd876a81631246a598023852dace4`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7189a68c404d49db302a2642bd2ac3e361429e3bbd3c9aa74ef93cc312ecbb`  
		Last Modified: Sat, 06 Feb 2021 00:35:00 GMT  
		Size: 22.7 MB (22695022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f595adc8679b76c16b421a7ca34d075145a1530a88976ce09438a3f81dacba`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca817c82b53cb322b3cfc64233b117d62339d3139b26edcdf6c40a1b56f24260`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:abeb475394eb10fe096062e0bffb0988fe2f4fbc9d8e299966ac12ce6604d63b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90202861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae3a16d0cb223c9ce0c9d049699046d127a61380215de6e90397ac6aa8bbde5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:02:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 21:02:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:02:32 GMT
ENV KAPACITOR_VERSION=1.4.1
# Tue, 12 Jan 2021 21:02:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 21:02:40 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Jan 2021 21:02:41 GMT
EXPOSE 9092
# Tue, 12 Jan 2021 21:02:43 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Jan 2021 21:02:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Jan 2021 21:02:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:02:45 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2d8759a0d27be8d9687c637d713b464c4446cee610a2cbb15d6792f82638f6`  
		Last Modified: Tue, 12 Jan 2021 21:03:23 GMT  
		Size: 13.4 MB (13405330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558886d3184a4e4f2c7a648ddcf082ec0e8ff6698bae58dbab4299afb1962c99`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c85a6723838ca952a46231082f6716475b096ce28bb56f73823a86bcee5022`  
		Last Modified: Tue, 12 Jan 2021 21:03:28 GMT  
		Size: 21.3 MB (21308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152de1f8863805f91c68cce798bd457881406face53344bc1c6b43d460aca28b`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def7f2f2c217322b3c0d141a7cf0a1d356795925086d8dc5138751cb059f0b`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:751985a16160d8d26dd557db05da0a999d619f60665144be480b1411e766406b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91222429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b42704b208f14159d9def4c6dd3e9ffbb3cdacd5956b27d282d3240b632929d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:32:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 23:32:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:32:26 GMT
ENV KAPACITOR_VERSION=1.4.1
# Tue, 12 Jan 2021 23:32:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 23:32:32 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Jan 2021 23:32:32 GMT
EXPOSE 9092
# Tue, 12 Jan 2021 23:32:33 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Jan 2021 23:32:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Jan 2021 23:32:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:32:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa62402c1259a03b7eacd6e8fe73e36ef197604f27fc96f1bc658fa58b67133`  
		Last Modified: Tue, 12 Jan 2021 23:33:14 GMT  
		Size: 12.9 MB (12934117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e787fe247913d0877422c3e4188d63d876cc27ddb8308beab0429165b5c17ce4`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2650892e5c87dbf490593d8f4a5e5a46cff5ca6601991ef5c1a1577812c1c919`  
		Last Modified: Tue, 12 Jan 2021 23:33:19 GMT  
		Size: 21.3 MB (21307930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58ea90b6db7de02310be568f3135ff5c37dbae9068832c1dbc4bb48eeb92eb2`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49e988c34ed7b3c3c779794b622bd81edda6b5eba70930be20ca31b992052f`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1-alpine`

```console
$ docker pull kapacitor@sha256:797102b5cdb633ea9bcd98f02e6df6b81b4ae92971315d982f497676251bb1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:a3cd5f7ac34d6ed8bb02192555ef40a3078e4194187e91829fb8690ed985592e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19678995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157a6cbb3d71432ffe9773020bff6a82308d8bbcdd4796b2befb8b2539249498`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:23:31 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 17 Dec 2020 13:23:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:23:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Dec 2020 13:23:35 GMT
EXPOSE 9092
# Thu, 17 Dec 2020 13:23:35 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Dec 2020 13:23:35 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Dec 2020 13:23:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:23:36 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2700961e2aa9d8b1a747e151bac0e7e85eaf621a73e665aa091034cdbb9fa`  
		Last Modified: Thu, 17 Dec 2020 13:24:11 GMT  
		Size: 16.6 MB (16598520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f0945c6384dc59f39c26a68228e5e75d062e8b903846f0dac9ec9822fddba6`  
		Last Modified: Thu, 17 Dec 2020 13:24:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5717d74957dbfe0e93c0cfe6e49d336e9533eea3f7ae7141f42aa72c708d3c63`  
		Last Modified: Thu, 17 Dec 2020 13:24:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4-alpine`

```console
$ docker pull kapacitor@sha256:797102b5cdb633ea9bcd98f02e6df6b81b4ae92971315d982f497676251bb1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:a3cd5f7ac34d6ed8bb02192555ef40a3078e4194187e91829fb8690ed985592e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19678995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157a6cbb3d71432ffe9773020bff6a82308d8bbcdd4796b2befb8b2539249498`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:23:31 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 17 Dec 2020 13:23:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:23:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Dec 2020 13:23:35 GMT
EXPOSE 9092
# Thu, 17 Dec 2020 13:23:35 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Dec 2020 13:23:35 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Dec 2020 13:23:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:23:36 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2700961e2aa9d8b1a747e151bac0e7e85eaf621a73e665aa091034cdbb9fa`  
		Last Modified: Thu, 17 Dec 2020 13:24:11 GMT  
		Size: 16.6 MB (16598520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f0945c6384dc59f39c26a68228e5e75d062e8b903846f0dac9ec9822fddba6`  
		Last Modified: Thu, 17 Dec 2020 13:24:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5717d74957dbfe0e93c0cfe6e49d336e9533eea3f7ae7141f42aa72c708d3c63`  
		Last Modified: Thu, 17 Dec 2020 13:24:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:be1df4df7e96a68ca558a17928e92ee799384ba7bb06b03bf821b60e270b7cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:e069696a9ce88a53c9731b19ff6c570b4dbce699ca8cf1212a3ba598da08d12c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111409370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5fce69def3c60c8198860552549dd860756a314c08f4b601768a06e00a20d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 00:34:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 06 Feb 2021 00:34:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 00:34:28 GMT
ENV KAPACITOR_VERSION=1.5.8
# Sat, 06 Feb 2021 00:34:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 06 Feb 2021 00:34:33 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 06 Feb 2021 00:34:33 GMT
EXPOSE 9092
# Sat, 06 Feb 2021 00:34:33 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 06 Feb 2021 00:34:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 06 Feb 2021 00:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 00:34:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85448296a98e89417030cbaa2637eb7f3ca25a8c0df10224dddc81b14f2711d2`  
		Last Modified: Sat, 06 Feb 2021 00:34:55 GMT  
		Size: 13.2 MB (13241611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbad8d39af10a56b6a2dc1d95c0d7d9f87dd876a81631246a598023852dace4`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce99d388eecedfef51e277c4b93be8395bc054ebac47afa3425d39ca2fc38a2`  
		Last Modified: Sat, 06 Feb 2021 00:35:11 GMT  
		Size: 37.2 MB (37174051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62282a8635bcdb6a46aa91c2c785b5b06b3a08193eb4370c461c115eaebe9b50`  
		Last Modified: Sat, 06 Feb 2021 00:35:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7950436a783095ad9f9a5f4087a1a4a5706114e44ae827005ffe7bdb0028a13`  
		Last Modified: Sat, 06 Feb 2021 00:35:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:2a98ff4422fb38e7178d667c17376a1a0b4c0aa7fc78dc7cda9c46c170497002
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103632923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae720a111b57d05b2b75550f0ee0f157f8682b756903043137ecaffbb61d8cb8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:02:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 21:02:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:58:57 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:59:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:59:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:59:07 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:59:08 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:59:08 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:59:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:59:10 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2d8759a0d27be8d9687c637d713b464c4446cee610a2cbb15d6792f82638f6`  
		Last Modified: Tue, 12 Jan 2021 21:03:23 GMT  
		Size: 13.4 MB (13405330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558886d3184a4e4f2c7a648ddcf082ec0e8ff6698bae58dbab4299afb1962c99`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bd1289480c546d734380e3fe497c8bd5af35eedfc45d1a41507e439b06fec2`  
		Last Modified: Thu, 28 Jan 2021 22:59:32 GMT  
		Size: 34.7 MB (34738170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05838db8e14f0eb21668f0045c9ba2d94567f17b9a3168500812589e2e9ad1ed`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30bb23f4c560cf65fdd8920d4b678e31372a2083a1d3aa807175638cd8794b0`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b8c0d80b3e7aed783c5ae3d9206736bb57154365bf4ae06889405210e0d95222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104444441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1793dec1b2481c763d6bed728e91e8a3056549baf7a1a52093d97955fcb34b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:32:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 23:32:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:52:35 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:52:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:52:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:52:46 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:52:46 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:52:47 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:52:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa62402c1259a03b7eacd6e8fe73e36ef197604f27fc96f1bc658fa58b67133`  
		Last Modified: Tue, 12 Jan 2021 23:33:14 GMT  
		Size: 12.9 MB (12934117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e787fe247913d0877422c3e4188d63d876cc27ddb8308beab0429165b5c17ce4`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ee37de473e59e926ce4ad939bdde43b8a72806bb966c199bf42d31b2c3d99`  
		Last Modified: Thu, 28 Jan 2021 22:53:09 GMT  
		Size: 34.5 MB (34529943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404dc687f62267a890ea45f5308725a6f3219295c8e20ba5139d411f47e06e6`  
		Last Modified: Thu, 28 Jan 2021 22:53:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8e0df45345b2b2131fd03e919d54c5daca4f6b583d6bcb77b3482a8591e066`  
		Last Modified: Thu, 28 Jan 2021 22:53:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.8`

```console
$ docker pull kapacitor@sha256:be1df4df7e96a68ca558a17928e92ee799384ba7bb06b03bf821b60e270b7cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.8` - linux; amd64

```console
$ docker pull kapacitor@sha256:e069696a9ce88a53c9731b19ff6c570b4dbce699ca8cf1212a3ba598da08d12c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111409370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5fce69def3c60c8198860552549dd860756a314c08f4b601768a06e00a20d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 00:34:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 06 Feb 2021 00:34:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 00:34:28 GMT
ENV KAPACITOR_VERSION=1.5.8
# Sat, 06 Feb 2021 00:34:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 06 Feb 2021 00:34:33 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 06 Feb 2021 00:34:33 GMT
EXPOSE 9092
# Sat, 06 Feb 2021 00:34:33 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 06 Feb 2021 00:34:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 06 Feb 2021 00:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 00:34:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85448296a98e89417030cbaa2637eb7f3ca25a8c0df10224dddc81b14f2711d2`  
		Last Modified: Sat, 06 Feb 2021 00:34:55 GMT  
		Size: 13.2 MB (13241611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbad8d39af10a56b6a2dc1d95c0d7d9f87dd876a81631246a598023852dace4`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce99d388eecedfef51e277c4b93be8395bc054ebac47afa3425d39ca2fc38a2`  
		Last Modified: Sat, 06 Feb 2021 00:35:11 GMT  
		Size: 37.2 MB (37174051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62282a8635bcdb6a46aa91c2c785b5b06b3a08193eb4370c461c115eaebe9b50`  
		Last Modified: Sat, 06 Feb 2021 00:35:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7950436a783095ad9f9a5f4087a1a4a5706114e44ae827005ffe7bdb0028a13`  
		Last Modified: Sat, 06 Feb 2021 00:35:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.8` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:2a98ff4422fb38e7178d667c17376a1a0b4c0aa7fc78dc7cda9c46c170497002
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103632923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae720a111b57d05b2b75550f0ee0f157f8682b756903043137ecaffbb61d8cb8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:02:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 21:02:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:58:57 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:59:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:59:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:59:07 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:59:08 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:59:08 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:59:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:59:10 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2d8759a0d27be8d9687c637d713b464c4446cee610a2cbb15d6792f82638f6`  
		Last Modified: Tue, 12 Jan 2021 21:03:23 GMT  
		Size: 13.4 MB (13405330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558886d3184a4e4f2c7a648ddcf082ec0e8ff6698bae58dbab4299afb1962c99`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bd1289480c546d734380e3fe497c8bd5af35eedfc45d1a41507e439b06fec2`  
		Last Modified: Thu, 28 Jan 2021 22:59:32 GMT  
		Size: 34.7 MB (34738170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05838db8e14f0eb21668f0045c9ba2d94567f17b9a3168500812589e2e9ad1ed`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30bb23f4c560cf65fdd8920d4b678e31372a2083a1d3aa807175638cd8794b0`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.8` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b8c0d80b3e7aed783c5ae3d9206736bb57154365bf4ae06889405210e0d95222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104444441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1793dec1b2481c763d6bed728e91e8a3056549baf7a1a52093d97955fcb34b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:32:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 23:32:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:52:35 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:52:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:52:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:52:46 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:52:46 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:52:47 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:52:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa62402c1259a03b7eacd6e8fe73e36ef197604f27fc96f1bc658fa58b67133`  
		Last Modified: Tue, 12 Jan 2021 23:33:14 GMT  
		Size: 12.9 MB (12934117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e787fe247913d0877422c3e4188d63d876cc27ddb8308beab0429165b5c17ce4`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ee37de473e59e926ce4ad939bdde43b8a72806bb966c199bf42d31b2c3d99`  
		Last Modified: Thu, 28 Jan 2021 22:53:09 GMT  
		Size: 34.5 MB (34529943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404dc687f62267a890ea45f5308725a6f3219295c8e20ba5139d411f47e06e6`  
		Last Modified: Thu, 28 Jan 2021 22:53:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8e0df45345b2b2131fd03e919d54c5daca4f6b583d6bcb77b3482a8591e066`  
		Last Modified: Thu, 28 Jan 2021 22:53:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.8-alpine`

```console
$ docker pull kapacitor@sha256:fbd4868cae4b9120a0ff967d8b9566d3dec6d3f2a4dabf343a10c8367e4a17db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5.8-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:72221f66afde98ab75b9c11110d88bcb73cfb317a85c5547eeeafd4caedb9481
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22597445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8176b8540df511d9259ce17ccbc98abaa07629d5cf9a9373c7b52d5ed60b87f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 28 Jan 2021 23:20:49 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 23:20:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 28 Jan 2021 23:20:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 23:20:53 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 23:20:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 23:20:54 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 28 Jan 2021 23:20:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 23:20:54 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4490cc4730a688f4c1e98ef48da92bfb00684539e9a8d0c3851e9ba007ea0c26`  
		Last Modified: Thu, 28 Jan 2021 23:21:27 GMT  
		Size: 19.5 MB (19516971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966d57ac7304061eec1a6d3e58cfc72b50607e1e0030a3d049c2449c4d2c10fd`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adab7b964a7a37e3d6a62e6298dd36b1f04116f35302a5a4235f6f27018bb53c`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:fbd4868cae4b9120a0ff967d8b9566d3dec6d3f2a4dabf343a10c8367e4a17db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:72221f66afde98ab75b9c11110d88bcb73cfb317a85c5547eeeafd4caedb9481
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22597445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8176b8540df511d9259ce17ccbc98abaa07629d5cf9a9373c7b52d5ed60b87f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 28 Jan 2021 23:20:49 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 23:20:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 28 Jan 2021 23:20:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 23:20:53 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 23:20:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 23:20:54 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 28 Jan 2021 23:20:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 23:20:54 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4490cc4730a688f4c1e98ef48da92bfb00684539e9a8d0c3851e9ba007ea0c26`  
		Last Modified: Thu, 28 Jan 2021 23:21:27 GMT  
		Size: 19.5 MB (19516971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966d57ac7304061eec1a6d3e58cfc72b50607e1e0030a3d049c2449c4d2c10fd`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adab7b964a7a37e3d6a62e6298dd36b1f04116f35302a5a4235f6f27018bb53c`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:fbd4868cae4b9120a0ff967d8b9566d3dec6d3f2a4dabf343a10c8367e4a17db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:72221f66afde98ab75b9c11110d88bcb73cfb317a85c5547eeeafd4caedb9481
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22597445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8176b8540df511d9259ce17ccbc98abaa07629d5cf9a9373c7b52d5ed60b87f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 28 Jan 2021 23:20:49 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 23:20:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 28 Jan 2021 23:20:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 23:20:53 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 23:20:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 23:20:54 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 28 Jan 2021 23:20:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 23:20:54 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4490cc4730a688f4c1e98ef48da92bfb00684539e9a8d0c3851e9ba007ea0c26`  
		Last Modified: Thu, 28 Jan 2021 23:21:27 GMT  
		Size: 19.5 MB (19516971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966d57ac7304061eec1a6d3e58cfc72b50607e1e0030a3d049c2449c4d2c10fd`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adab7b964a7a37e3d6a62e6298dd36b1f04116f35302a5a4235f6f27018bb53c`  
		Last Modified: Thu, 28 Jan 2021 23:21:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:be1df4df7e96a68ca558a17928e92ee799384ba7bb06b03bf821b60e270b7cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:e069696a9ce88a53c9731b19ff6c570b4dbce699ca8cf1212a3ba598da08d12c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111409370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5fce69def3c60c8198860552549dd860756a314c08f4b601768a06e00a20d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 00:34:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 06 Feb 2021 00:34:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 00:34:28 GMT
ENV KAPACITOR_VERSION=1.5.8
# Sat, 06 Feb 2021 00:34:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 06 Feb 2021 00:34:33 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 06 Feb 2021 00:34:33 GMT
EXPOSE 9092
# Sat, 06 Feb 2021 00:34:33 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 06 Feb 2021 00:34:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 06 Feb 2021 00:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 00:34:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85448296a98e89417030cbaa2637eb7f3ca25a8c0df10224dddc81b14f2711d2`  
		Last Modified: Sat, 06 Feb 2021 00:34:55 GMT  
		Size: 13.2 MB (13241611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbad8d39af10a56b6a2dc1d95c0d7d9f87dd876a81631246a598023852dace4`  
		Last Modified: Sat, 06 Feb 2021 00:34:54 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce99d388eecedfef51e277c4b93be8395bc054ebac47afa3425d39ca2fc38a2`  
		Last Modified: Sat, 06 Feb 2021 00:35:11 GMT  
		Size: 37.2 MB (37174051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62282a8635bcdb6a46aa91c2c785b5b06b3a08193eb4370c461c115eaebe9b50`  
		Last Modified: Sat, 06 Feb 2021 00:35:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7950436a783095ad9f9a5f4087a1a4a5706114e44ae827005ffe7bdb0028a13`  
		Last Modified: Sat, 06 Feb 2021 00:35:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:2a98ff4422fb38e7178d667c17376a1a0b4c0aa7fc78dc7cda9c46c170497002
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103632923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae720a111b57d05b2b75550f0ee0f157f8682b756903043137ecaffbb61d8cb8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:02:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 21:02:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:58:57 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:59:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:59:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:59:07 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:59:08 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:59:08 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:59:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:59:10 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2d8759a0d27be8d9687c637d713b464c4446cee610a2cbb15d6792f82638f6`  
		Last Modified: Tue, 12 Jan 2021 21:03:23 GMT  
		Size: 13.4 MB (13405330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558886d3184a4e4f2c7a648ddcf082ec0e8ff6698bae58dbab4299afb1962c99`  
		Last Modified: Tue, 12 Jan 2021 21:03:21 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bd1289480c546d734380e3fe497c8bd5af35eedfc45d1a41507e439b06fec2`  
		Last Modified: Thu, 28 Jan 2021 22:59:32 GMT  
		Size: 34.7 MB (34738170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05838db8e14f0eb21668f0045c9ba2d94567f17b9a3168500812589e2e9ad1ed`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30bb23f4c560cf65fdd8920d4b678e31372a2083a1d3aa807175638cd8794b0`  
		Last Modified: Thu, 28 Jan 2021 22:59:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b8c0d80b3e7aed783c5ae3d9206736bb57154365bf4ae06889405210e0d95222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104444441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1793dec1b2481c763d6bed728e91e8a3056549baf7a1a52093d97955fcb34b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:32:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Jan 2021 23:32:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 28 Jan 2021 22:52:35 GMT
ENV KAPACITOR_VERSION=1.5.8
# Thu, 28 Jan 2021 22:52:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 28 Jan 2021 22:52:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 28 Jan 2021 22:52:46 GMT
EXPOSE 9092
# Thu, 28 Jan 2021 22:52:46 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 28 Jan 2021 22:52:47 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 28 Jan 2021 22:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 28 Jan 2021 22:52:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa62402c1259a03b7eacd6e8fe73e36ef197604f27fc96f1bc658fa58b67133`  
		Last Modified: Tue, 12 Jan 2021 23:33:14 GMT  
		Size: 12.9 MB (12934117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e787fe247913d0877422c3e4188d63d876cc27ddb8308beab0429165b5c17ce4`  
		Last Modified: Tue, 12 Jan 2021 23:33:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ee37de473e59e926ce4ad939bdde43b8a72806bb966c199bf42d31b2c3d99`  
		Last Modified: Thu, 28 Jan 2021 22:53:09 GMT  
		Size: 34.5 MB (34529943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404dc687f62267a890ea45f5308725a6f3219295c8e20ba5139d411f47e06e6`  
		Last Modified: Thu, 28 Jan 2021 22:53:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8e0df45345b2b2131fd03e919d54c5daca4f6b583d6bcb77b3482a8591e066`  
		Last Modified: Thu, 28 Jan 2021 22:53:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
