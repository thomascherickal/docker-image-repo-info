<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.2`](#kapacitor162)
-	[`kapacitor:1.6.2-alpine`](#kapacitor162-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:14577324bc17b3f8660e54e903447b848e40b751c6749851e7672b57e799b4a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:9c6b855a1de10e053b5335d84ee0d9a34f73306782c238123c05b9c74d11f6db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111634740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851ef852df1e9236115b5e62882d9ef6013382a1af2074beaff929ea2ac9f4fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:12:14 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 03 Dec 2021 04:12:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:12:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 03 Dec 2021 04:12:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 03 Dec 2021 04:12:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 03 Dec 2021 04:12:31 GMT
EXPOSE 9092
# Fri, 03 Dec 2021 04:12:31 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 03 Dec 2021 04:12:32 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 03 Dec 2021 04:12:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:12:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f386c5fc42a706d579b545a76f5bbdc7f4e6fcb70fd0a20b43dfc8a0af81fd`  
		Last Modified: Fri, 03 Dec 2021 04:13:07 GMT  
		Size: 13.4 MB (13386540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dbe82dad4e858075662b8c7efc998c08b678a206a2453855bc23b998e16de`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb074e27b5eda138387101e846e359aadbcf53bb92ed3df3f67a578435c9fcd1`  
		Last Modified: Fri, 03 Dec 2021 04:13:11 GMT  
		Size: 37.2 MB (37219542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594cd2313641b3310100f91d9ad6ec5aca4a6f06b615365c032608baa3a9efd5`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed806683ff066f2865bff5179bb97cb319011f55f3ca1354dab7738ebcf1456`  
		Last Modified: Fri, 03 Dec 2021 04:13:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:7eebf70016e1495cedadb812ed2cd5418e2ea39b16aa28394047f8054fa81f62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647021ff594087cab90b951cfd33557bb811b55a72956a6b77e64b5c3b50bc5c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:34:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 04 Dec 2021 02:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:34:49 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 04 Dec 2021 02:34:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 04 Dec 2021 02:34:59 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 04 Dec 2021 02:34:59 GMT
EXPOSE 9092
# Sat, 04 Dec 2021 02:35:00 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 04 Dec 2021 02:35:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 04 Dec 2021 02:35:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:35:01 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc29e0bfee4b10f33c08ad7bf910e32fae2cd552b9f9da3e6e55f68c55bb32b`  
		Last Modified: Sat, 04 Dec 2021 02:35:29 GMT  
		Size: 13.6 MB (13568967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835a2f9e4e8aea06850736b04f09bdc914ad5ee5f64e528f4a86f33c6914b20d`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8529713c8a16d854ae29177fa0de541cc26ade81acf868c2bb2104c73480a54`  
		Last Modified: Sat, 04 Dec 2021 02:35:40 GMT  
		Size: 34.8 MB (34786690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef6264bb9f049ef890e0c5e6f349a908afead317beacee90105755a29e5e70a`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6516f72aa17bf22ba8d7649246a5354d573e83ab59f034f0480e18ee8de03a`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3848faa7040f3e17f65dafe47a64a1dc88409772ddbd60ac1be680c0f78c9b8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104696015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2036fabe354f0ac8c48e9cafb1a14286b3098c1e3cbbd621295d8c571d1617`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:54:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 21 Dec 2021 19:54:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:54:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 21 Dec 2021 19:54:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 21 Dec 2021 19:54:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 21 Dec 2021 19:54:31 GMT
EXPOSE 9092
# Tue, 21 Dec 2021 19:54:32 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 21 Dec 2021 19:54:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 21 Dec 2021 19:54:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:54:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed6fa11e0f6f1e734859b88d88087b9d225172e5b5db1d931d83588a0fb9ce0`  
		Last Modified: Tue, 21 Dec 2021 19:55:13 GMT  
		Size: 12.9 MB (12867898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d462a55e4b587b356acce229472ec1bc794a86c2620fe52faf705ebb1423576`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf02361ed92fe9bc3d6d9137f43e15ab1fdd1e3ae76dcc744c0bbb6ab51c7d17`  
		Last Modified: Tue, 21 Dec 2021 19:55:16 GMT  
		Size: 34.6 MB (34560091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e89ca00e999c04b0557f744637166d5665e9215876fd4beb08f011b412f6638`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8c3323d9b5dc44bd2ce248c213fb2356e5ff477c03f31e36c65ba45744e83`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:751918e56fde6040974138659942dcb1dfefda5ea61321e20023e70f5b5c6d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:ebfc4af599b8126bdce9d95186ae296a9ac80697a0ae97bb758d6e15576915ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f8972ccc76427f5cba40c5b78c201cbdde44e128e47e642190767bb79e8c6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 13 Nov 2021 06:07:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:29 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:29 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:29 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:30 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:30 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c6344f55af907ec99dd18980cfac4d88970868515c05e6228b0fd8cfeff`  
		Last Modified: Sat, 13 Nov 2021 06:08:12 GMT  
		Size: 19.5 MB (19540901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e6d3e0710bdc72f26e2a54c0fed4abe60bc4496eb1c111287663d4257421c`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d938d5c3e3a42543955a737542599f0936f8268da48dbb42b3d23c4b512c0`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:14577324bc17b3f8660e54e903447b848e40b751c6749851e7672b57e799b4a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:9c6b855a1de10e053b5335d84ee0d9a34f73306782c238123c05b9c74d11f6db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111634740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851ef852df1e9236115b5e62882d9ef6013382a1af2074beaff929ea2ac9f4fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:12:14 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 03 Dec 2021 04:12:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:12:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 03 Dec 2021 04:12:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 03 Dec 2021 04:12:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 03 Dec 2021 04:12:31 GMT
EXPOSE 9092
# Fri, 03 Dec 2021 04:12:31 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 03 Dec 2021 04:12:32 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 03 Dec 2021 04:12:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:12:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f386c5fc42a706d579b545a76f5bbdc7f4e6fcb70fd0a20b43dfc8a0af81fd`  
		Last Modified: Fri, 03 Dec 2021 04:13:07 GMT  
		Size: 13.4 MB (13386540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dbe82dad4e858075662b8c7efc998c08b678a206a2453855bc23b998e16de`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb074e27b5eda138387101e846e359aadbcf53bb92ed3df3f67a578435c9fcd1`  
		Last Modified: Fri, 03 Dec 2021 04:13:11 GMT  
		Size: 37.2 MB (37219542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594cd2313641b3310100f91d9ad6ec5aca4a6f06b615365c032608baa3a9efd5`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed806683ff066f2865bff5179bb97cb319011f55f3ca1354dab7738ebcf1456`  
		Last Modified: Fri, 03 Dec 2021 04:13:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:7eebf70016e1495cedadb812ed2cd5418e2ea39b16aa28394047f8054fa81f62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647021ff594087cab90b951cfd33557bb811b55a72956a6b77e64b5c3b50bc5c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:34:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 04 Dec 2021 02:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:34:49 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 04 Dec 2021 02:34:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 04 Dec 2021 02:34:59 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 04 Dec 2021 02:34:59 GMT
EXPOSE 9092
# Sat, 04 Dec 2021 02:35:00 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 04 Dec 2021 02:35:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 04 Dec 2021 02:35:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:35:01 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc29e0bfee4b10f33c08ad7bf910e32fae2cd552b9f9da3e6e55f68c55bb32b`  
		Last Modified: Sat, 04 Dec 2021 02:35:29 GMT  
		Size: 13.6 MB (13568967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835a2f9e4e8aea06850736b04f09bdc914ad5ee5f64e528f4a86f33c6914b20d`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8529713c8a16d854ae29177fa0de541cc26ade81acf868c2bb2104c73480a54`  
		Last Modified: Sat, 04 Dec 2021 02:35:40 GMT  
		Size: 34.8 MB (34786690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef6264bb9f049ef890e0c5e6f349a908afead317beacee90105755a29e5e70a`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6516f72aa17bf22ba8d7649246a5354d573e83ab59f034f0480e18ee8de03a`  
		Last Modified: Sat, 04 Dec 2021 02:35:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3848faa7040f3e17f65dafe47a64a1dc88409772ddbd60ac1be680c0f78c9b8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104696015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2036fabe354f0ac8c48e9cafb1a14286b3098c1e3cbbd621295d8c571d1617`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:54:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 21 Dec 2021 19:54:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:54:26 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 21 Dec 2021 19:54:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 21 Dec 2021 19:54:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 21 Dec 2021 19:54:31 GMT
EXPOSE 9092
# Tue, 21 Dec 2021 19:54:32 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 21 Dec 2021 19:54:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 21 Dec 2021 19:54:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:54:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed6fa11e0f6f1e734859b88d88087b9d225172e5b5db1d931d83588a0fb9ce0`  
		Last Modified: Tue, 21 Dec 2021 19:55:13 GMT  
		Size: 12.9 MB (12867898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d462a55e4b587b356acce229472ec1bc794a86c2620fe52faf705ebb1423576`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf02361ed92fe9bc3d6d9137f43e15ab1fdd1e3ae76dcc744c0bbb6ab51c7d17`  
		Last Modified: Tue, 21 Dec 2021 19:55:16 GMT  
		Size: 34.6 MB (34560091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e89ca00e999c04b0557f744637166d5665e9215876fd4beb08f011b412f6638`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8c3323d9b5dc44bd2ce248c213fb2356e5ff477c03f31e36c65ba45744e83`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:751918e56fde6040974138659942dcb1dfefda5ea61321e20023e70f5b5c6d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:ebfc4af599b8126bdce9d95186ae296a9ac80697a0ae97bb758d6e15576915ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f8972ccc76427f5cba40c5b78c201cbdde44e128e47e642190767bb79e8c6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 13 Nov 2021 06:07:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:29 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:29 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:29 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:30 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:30 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c6344f55af907ec99dd18980cfac4d88970868515c05e6228b0fd8cfeff`  
		Last Modified: Sat, 13 Nov 2021 06:08:12 GMT  
		Size: 19.5 MB (19540901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e6d3e0710bdc72f26e2a54c0fed4abe60bc4496eb1c111287663d4257421c`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d938d5c3e3a42543955a737542599f0936f8268da48dbb42b3d23c4b512c0`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:1a141d34c6753c0b3747d426cbf91cfd772efcd6eb5ab44fdbb793333545f891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:f22333a187037afac2f54ab2684c847024f2a8fe2e881133548f7dc9e70e80b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132817765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdeb95960da51485e7d52c6bcb9cc1d05f67786c4d5cc5a5038bce724e3e0f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:12:14 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 03 Dec 2021 04:12:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:12:39 GMT
ENV KAPACITOR_VERSION=1.6.2
# Fri, 03 Dec 2021 04:12:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 03 Dec 2021 04:12:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 03 Dec 2021 04:12:45 GMT
EXPOSE 9092
# Fri, 03 Dec 2021 04:12:46 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 03 Dec 2021 04:12:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 03 Dec 2021 04:12:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:12:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f386c5fc42a706d579b545a76f5bbdc7f4e6fcb70fd0a20b43dfc8a0af81fd`  
		Last Modified: Fri, 03 Dec 2021 04:13:07 GMT  
		Size: 13.4 MB (13386540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dbe82dad4e858075662b8c7efc998c08b678a206a2453855bc23b998e16de`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e66467af94904944cb25e19ddf0e736ba153c62237db494083f48db588de3`  
		Last Modified: Fri, 03 Dec 2021 04:13:30 GMT  
		Size: 58.4 MB (58402566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee15ae00f32b97ce3556ce86a9785054717f722c4afb4fa7c957812dd7c20f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ae8b635e39b36ec87f48c309dd824ebba90bd8f60a1185ec2f8804e76b616f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:4c1a448a7e194d4ec48d5c8e00b7807b117c94d93e4b9503b35ffccb8db849d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124573370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bce67ba991ebac0c8a843e260ad320e055c07b6ad65755ca1309e4fcc7f7ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:54:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 21 Dec 2021 19:54:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:54:43 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 21 Dec 2021 19:54:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 21 Dec 2021 19:54:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 21 Dec 2021 19:54:49 GMT
EXPOSE 9092
# Tue, 21 Dec 2021 19:54:50 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 21 Dec 2021 19:54:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 21 Dec 2021 19:54:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:54:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed6fa11e0f6f1e734859b88d88087b9d225172e5b5db1d931d83588a0fb9ce0`  
		Last Modified: Tue, 21 Dec 2021 19:55:13 GMT  
		Size: 12.9 MB (12867898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d462a55e4b587b356acce229472ec1bc794a86c2620fe52faf705ebb1423576`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2069d3e69b228ba8c6102e451f7ccf18cb0535b197611ce3e86b9319803cee0e`  
		Last Modified: Tue, 21 Dec 2021 19:55:38 GMT  
		Size: 54.4 MB (54437446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3ed53973d044f73cf51963e1bd9aaadf7d89290941f79778767edf2672cf19`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd6cf25309fc44b18a227f76ae1eefea6432b4455682ba9051092508ce0c99d`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2`

```console
$ docker pull kapacitor@sha256:1a141d34c6753c0b3747d426cbf91cfd772efcd6eb5ab44fdbb793333545f891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.2` - linux; amd64

```console
$ docker pull kapacitor@sha256:f22333a187037afac2f54ab2684c847024f2a8fe2e881133548f7dc9e70e80b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132817765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdeb95960da51485e7d52c6bcb9cc1d05f67786c4d5cc5a5038bce724e3e0f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:12:14 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 03 Dec 2021 04:12:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:12:39 GMT
ENV KAPACITOR_VERSION=1.6.2
# Fri, 03 Dec 2021 04:12:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 03 Dec 2021 04:12:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 03 Dec 2021 04:12:45 GMT
EXPOSE 9092
# Fri, 03 Dec 2021 04:12:46 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 03 Dec 2021 04:12:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 03 Dec 2021 04:12:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:12:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f386c5fc42a706d579b545a76f5bbdc7f4e6fcb70fd0a20b43dfc8a0af81fd`  
		Last Modified: Fri, 03 Dec 2021 04:13:07 GMT  
		Size: 13.4 MB (13386540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dbe82dad4e858075662b8c7efc998c08b678a206a2453855bc23b998e16de`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e66467af94904944cb25e19ddf0e736ba153c62237db494083f48db588de3`  
		Last Modified: Fri, 03 Dec 2021 04:13:30 GMT  
		Size: 58.4 MB (58402566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee15ae00f32b97ce3556ce86a9785054717f722c4afb4fa7c957812dd7c20f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ae8b635e39b36ec87f48c309dd824ebba90bd8f60a1185ec2f8804e76b616f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.2` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:4c1a448a7e194d4ec48d5c8e00b7807b117c94d93e4b9503b35ffccb8db849d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124573370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bce67ba991ebac0c8a843e260ad320e055c07b6ad65755ca1309e4fcc7f7ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:54:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 21 Dec 2021 19:54:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:54:43 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 21 Dec 2021 19:54:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 21 Dec 2021 19:54:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 21 Dec 2021 19:54:49 GMT
EXPOSE 9092
# Tue, 21 Dec 2021 19:54:50 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 21 Dec 2021 19:54:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 21 Dec 2021 19:54:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:54:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed6fa11e0f6f1e734859b88d88087b9d225172e5b5db1d931d83588a0fb9ce0`  
		Last Modified: Tue, 21 Dec 2021 19:55:13 GMT  
		Size: 12.9 MB (12867898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d462a55e4b587b356acce229472ec1bc794a86c2620fe52faf705ebb1423576`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2069d3e69b228ba8c6102e451f7ccf18cb0535b197611ce3e86b9319803cee0e`  
		Last Modified: Tue, 21 Dec 2021 19:55:38 GMT  
		Size: 54.4 MB (54437446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3ed53973d044f73cf51963e1bd9aaadf7d89290941f79778767edf2672cf19`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd6cf25309fc44b18a227f76ae1eefea6432b4455682ba9051092508ce0c99d`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2-alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.2-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:1a141d34c6753c0b3747d426cbf91cfd772efcd6eb5ab44fdbb793333545f891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:f22333a187037afac2f54ab2684c847024f2a8fe2e881133548f7dc9e70e80b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132817765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdeb95960da51485e7d52c6bcb9cc1d05f67786c4d5cc5a5038bce724e3e0f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:12:14 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 03 Dec 2021 04:12:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:12:39 GMT
ENV KAPACITOR_VERSION=1.6.2
# Fri, 03 Dec 2021 04:12:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 03 Dec 2021 04:12:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 03 Dec 2021 04:12:45 GMT
EXPOSE 9092
# Fri, 03 Dec 2021 04:12:46 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 03 Dec 2021 04:12:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 03 Dec 2021 04:12:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:12:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f386c5fc42a706d579b545a76f5bbdc7f4e6fcb70fd0a20b43dfc8a0af81fd`  
		Last Modified: Fri, 03 Dec 2021 04:13:07 GMT  
		Size: 13.4 MB (13386540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dbe82dad4e858075662b8c7efc998c08b678a206a2453855bc23b998e16de`  
		Last Modified: Fri, 03 Dec 2021 04:13:05 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e66467af94904944cb25e19ddf0e736ba153c62237db494083f48db588de3`  
		Last Modified: Fri, 03 Dec 2021 04:13:30 GMT  
		Size: 58.4 MB (58402566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee15ae00f32b97ce3556ce86a9785054717f722c4afb4fa7c957812dd7c20f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ae8b635e39b36ec87f48c309dd824ebba90bd8f60a1185ec2f8804e76b616f`  
		Last Modified: Fri, 03 Dec 2021 04:13:22 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:4c1a448a7e194d4ec48d5c8e00b7807b117c94d93e4b9503b35ffccb8db849d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124573370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bce67ba991ebac0c8a843e260ad320e055c07b6ad65755ca1309e4fcc7f7ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:54:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 21 Dec 2021 19:54:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:54:43 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 21 Dec 2021 19:54:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 21 Dec 2021 19:54:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 21 Dec 2021 19:54:49 GMT
EXPOSE 9092
# Tue, 21 Dec 2021 19:54:50 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 21 Dec 2021 19:54:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 21 Dec 2021 19:54:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:54:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed6fa11e0f6f1e734859b88d88087b9d225172e5b5db1d931d83588a0fb9ce0`  
		Last Modified: Tue, 21 Dec 2021 19:55:13 GMT  
		Size: 12.9 MB (12867898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d462a55e4b587b356acce229472ec1bc794a86c2620fe52faf705ebb1423576`  
		Last Modified: Tue, 21 Dec 2021 19:55:11 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2069d3e69b228ba8c6102e451f7ccf18cb0535b197611ce3e86b9319803cee0e`  
		Last Modified: Tue, 21 Dec 2021 19:55:38 GMT  
		Size: 54.4 MB (54437446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3ed53973d044f73cf51963e1bd9aaadf7d89290941f79778767edf2672cf19`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd6cf25309fc44b18a227f76ae1eefea6432b4455682ba9051092508ce0c99d`  
		Last Modified: Tue, 21 Dec 2021 19:55:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
