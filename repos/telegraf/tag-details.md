<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.23`](#telegraf123)
-	[`telegraf:1.23-alpine`](#telegraf123-alpine)
-	[`telegraf:1.23.4`](#telegraf1234)
-	[`telegraf:1.23.4-alpine`](#telegraf1234-alpine)
-	[`telegraf:1.24`](#telegraf124)
-	[`telegraf:1.24-alpine`](#telegraf124-alpine)
-	[`telegraf:1.24.4`](#telegraf1244)
-	[`telegraf:1.24.4-alpine`](#telegraf1244-alpine)
-	[`telegraf:1.25`](#telegraf125)
-	[`telegraf:1.25-alpine`](#telegraf125-alpine)
-	[`telegraf:1.25.2`](#telegraf1252)
-	[`telegraf:1.25.2-alpine`](#telegraf1252-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:7f029bdff2c588224e777243cef31d4add976ef02f1018cfb2a406cdc9aa442f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:a4a8c70cd66e250a12ccc4d1632ba71781a10e0fc193e514cefa908ad5b4bdf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131700929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f040209fa5b9c1f326d0932bb9d8545c9e8f189a2754cae8f870c98b32121b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 11 Feb 2023 03:43:26 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 11 Feb 2023 03:43:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 11 Feb 2023 03:43:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 03:43:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 11 Feb 2023 03:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 03:43:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b80c6fe5b19770ae7024456f1889cbf9647a69156483778c65ff867ec39ea1`  
		Last Modified: Sat, 11 Feb 2023 03:44:20 GMT  
		Size: 41.8 MB (41849223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e24e14800abfb2d0a0161156f4ef8682450737d37b010651936a48ca97389c`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:3fce82135914505f165f485c7b77855ae7ae8547761c7e5106cf20a49a4898ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121936419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0d345d144381f151120da454ae329bbaf36d45829f69c98362bc6c7122a07d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 10 Feb 2023 07:34:49 GMT
ENV TELEGRAF_VERSION=1.23.4
# Fri, 10 Feb 2023 07:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 10 Feb 2023 07:34:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 10 Feb 2023 07:34:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 10 Feb 2023 07:34:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 07:34:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a10b729bfac2ea3481ab837ab52175b15cc01c6d9555f1f05138defc9761f07`  
		Last Modified: Fri, 10 Feb 2023 07:35:57 GMT  
		Size: 39.1 MB (39106561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2890863edf69f2e1619a2b57e6b1a4bb13dae4fccbac62f84aa0d83290b4a0b6`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:803ce566e208b5f8124c5d9110231d74e1e36813f23c72bab336d0dcae25fad5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada1da98a288fa93eb3b3c3532d9f71b94386aa5da0c3204aba83364c9711d87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:01 GMT
ENV TELEGRAF_VERSION=1.23.4
# Thu, 09 Feb 2023 21:13:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d473f1eec5c3dcb1d5c7294b693bbec569739a50d80506187158d7cf1aab05cd`  
		Last Modified: Thu, 09 Feb 2023 21:13:40 GMT  
		Size: 38.0 MB (38031312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17533e605e0d05eacbff5dc53b26578293af1bf87f0e63acf06d6488bd756ad4`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:b0b6df22c36d9512e8104f6c489879a8dc4405b6e1f13d80a1ef966ae277ad54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e0c338f7b496fd6982cd03f3fce4e23707d541d3a7becc4dc60264963052e3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47792482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a5557b69645ff3384a4290d3d0e4f9058a96372e528b215d62f4cac8d0e572`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 11 Feb 2023 14:07:54 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 11 Feb 2023 14:08:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 11 Feb 2023 14:08:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 14:08:02 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 11 Feb 2023 14:08:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:08:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673a7089d4c9e3e02019adb098f3d94695041275ff6436c7d2cbe29cf2d9696d`  
		Last Modified: Sat, 11 Feb 2023 14:08:56 GMT  
		Size: 41.7 MB (41685835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed3f9863332cc5cd2ae9f50206da5f0e325af3dd7d298835cd3efc57f60cbf3`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4`

```console
$ docker pull telegraf@sha256:7f029bdff2c588224e777243cef31d4add976ef02f1018cfb2a406cdc9aa442f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.4` - linux; amd64

```console
$ docker pull telegraf@sha256:a4a8c70cd66e250a12ccc4d1632ba71781a10e0fc193e514cefa908ad5b4bdf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131700929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f040209fa5b9c1f326d0932bb9d8545c9e8f189a2754cae8f870c98b32121b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 11 Feb 2023 03:43:26 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 11 Feb 2023 03:43:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 11 Feb 2023 03:43:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 03:43:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 11 Feb 2023 03:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 03:43:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b80c6fe5b19770ae7024456f1889cbf9647a69156483778c65ff867ec39ea1`  
		Last Modified: Sat, 11 Feb 2023 03:44:20 GMT  
		Size: 41.8 MB (41849223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e24e14800abfb2d0a0161156f4ef8682450737d37b010651936a48ca97389c`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:3fce82135914505f165f485c7b77855ae7ae8547761c7e5106cf20a49a4898ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121936419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0d345d144381f151120da454ae329bbaf36d45829f69c98362bc6c7122a07d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 10 Feb 2023 07:34:49 GMT
ENV TELEGRAF_VERSION=1.23.4
# Fri, 10 Feb 2023 07:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 10 Feb 2023 07:34:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 10 Feb 2023 07:34:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 10 Feb 2023 07:34:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 07:34:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a10b729bfac2ea3481ab837ab52175b15cc01c6d9555f1f05138defc9761f07`  
		Last Modified: Fri, 10 Feb 2023 07:35:57 GMT  
		Size: 39.1 MB (39106561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2890863edf69f2e1619a2b57e6b1a4bb13dae4fccbac62f84aa0d83290b4a0b6`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:803ce566e208b5f8124c5d9110231d74e1e36813f23c72bab336d0dcae25fad5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada1da98a288fa93eb3b3c3532d9f71b94386aa5da0c3204aba83364c9711d87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:01 GMT
ENV TELEGRAF_VERSION=1.23.4
# Thu, 09 Feb 2023 21:13:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d473f1eec5c3dcb1d5c7294b693bbec569739a50d80506187158d7cf1aab05cd`  
		Last Modified: Thu, 09 Feb 2023 21:13:40 GMT  
		Size: 38.0 MB (38031312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17533e605e0d05eacbff5dc53b26578293af1bf87f0e63acf06d6488bd756ad4`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4-alpine`

```console
$ docker pull telegraf@sha256:b0b6df22c36d9512e8104f6c489879a8dc4405b6e1f13d80a1ef966ae277ad54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e0c338f7b496fd6982cd03f3fce4e23707d541d3a7becc4dc60264963052e3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47792482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a5557b69645ff3384a4290d3d0e4f9058a96372e528b215d62f4cac8d0e572`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 11 Feb 2023 14:07:54 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 11 Feb 2023 14:08:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 11 Feb 2023 14:08:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 14:08:02 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 11 Feb 2023 14:08:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:08:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673a7089d4c9e3e02019adb098f3d94695041275ff6436c7d2cbe29cf2d9696d`  
		Last Modified: Sat, 11 Feb 2023 14:08:56 GMT  
		Size: 41.7 MB (41685835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed3f9863332cc5cd2ae9f50206da5f0e325af3dd7d298835cd3efc57f60cbf3`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:8a2a1291aa743ec93f0521fe081b92eeebfa5f9c8330a723df8dd2a96556fc6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:1657a6cb821658f92d53331684b24c2af8202f385e70fbec1af949b7cfdb0e08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134319110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64492c819aeb4fb7f0d2683d00729fd3ccbe062876fbd35486d2a59c8b42668`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 11 Feb 2023 03:43:39 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sat, 11 Feb 2023 03:43:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 11 Feb 2023 03:43:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 03:43:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 11 Feb 2023 03:43:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 03:43:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c726ff6cfabf8ffae2ac693c17d7b14535156b32981b890a8a2e8079d6dfbfc4`  
		Last Modified: Sat, 11 Feb 2023 03:44:37 GMT  
		Size: 44.5 MB (44467406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108c74ab1d1eadcc2b62c72bc742ee8d754c1619e99ce02d9919a67f6ac8ddd4`  
		Last Modified: Sat, 11 Feb 2023 03:44:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0f541a69e585b87ae669d6eb89823791332b57808e281f8353d0ebe9dc6c540c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124336929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58157d545aa1da9f54b43491756b698806d04c28a92a44c77929299b9cf0f8b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 10 Feb 2023 07:35:02 GMT
ENV TELEGRAF_VERSION=1.24.4
# Fri, 10 Feb 2023 07:35:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 10 Feb 2023 07:35:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 10 Feb 2023 07:35:08 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 10 Feb 2023 07:35:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 07:35:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f56a7d52954a55f4dcb31bff678fbe654e2e5341076007416caad5b8c4dc94`  
		Last Modified: Fri, 10 Feb 2023 07:36:16 GMT  
		Size: 41.5 MB (41507074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4be7ec8dab8442b6738c0fb28368b71b42c458b658393e7b54a404971511da`  
		Last Modified: Fri, 10 Feb 2023 07:36:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:fc102f828ca9dc2878b61e68bd31609ba1a29e1ccc1500489a03c4d73bdf77bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bc5498388a6a51559b9772559d5ac3e6040317fee182b3d460947e995486e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 09 Feb 2023 21:13:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98825686562eec0e4213e16e3734b97e44fa66bc3c69e516e31af1820939f93`  
		Last Modified: Thu, 09 Feb 2023 21:13:54 GMT  
		Size: 40.3 MB (40305460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8318a7b649fffb5e902a0b741a5c54d51ee7b0a6b6715295c031b94293d666b`  
		Last Modified: Thu, 09 Feb 2023 21:13:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:2e2e14c99c17464602e65cd89a095b755410b01853a88f8a1e0e137841b33167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ea87e6530418dea56b240838bf620c00625c9273b928ea82387e59869f4b035f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50404478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4256548ab14d2ac9434897e2f54eb4bba0e80a33a8a74333f2d6a9ba0235a67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 11 Feb 2023 14:08:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sat, 11 Feb 2023 14:08:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 11 Feb 2023 14:08:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 14:08:16 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 11 Feb 2023 14:08:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:08:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c72f3490ef958b34abba3216f60222ce0a09bc3ba25392ea46cf1e62813b6`  
		Last Modified: Sat, 11 Feb 2023 14:09:12 GMT  
		Size: 44.3 MB (44297832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ef14f3c9c3ce5940dfdfe7deaef2e8505d4b8ee41f0a73ad76493ebf4269f0`  
		Last Modified: Sat, 11 Feb 2023 14:09:05 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4`

```console
$ docker pull telegraf@sha256:8a2a1291aa743ec93f0521fe081b92eeebfa5f9c8330a723df8dd2a96556fc6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.4` - linux; amd64

```console
$ docker pull telegraf@sha256:1657a6cb821658f92d53331684b24c2af8202f385e70fbec1af949b7cfdb0e08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134319110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64492c819aeb4fb7f0d2683d00729fd3ccbe062876fbd35486d2a59c8b42668`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 11 Feb 2023 03:43:39 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sat, 11 Feb 2023 03:43:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 11 Feb 2023 03:43:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 03:43:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 11 Feb 2023 03:43:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 03:43:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c726ff6cfabf8ffae2ac693c17d7b14535156b32981b890a8a2e8079d6dfbfc4`  
		Last Modified: Sat, 11 Feb 2023 03:44:37 GMT  
		Size: 44.5 MB (44467406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108c74ab1d1eadcc2b62c72bc742ee8d754c1619e99ce02d9919a67f6ac8ddd4`  
		Last Modified: Sat, 11 Feb 2023 03:44:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0f541a69e585b87ae669d6eb89823791332b57808e281f8353d0ebe9dc6c540c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124336929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58157d545aa1da9f54b43491756b698806d04c28a92a44c77929299b9cf0f8b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 10 Feb 2023 07:35:02 GMT
ENV TELEGRAF_VERSION=1.24.4
# Fri, 10 Feb 2023 07:35:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 10 Feb 2023 07:35:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 10 Feb 2023 07:35:08 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 10 Feb 2023 07:35:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 07:35:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f56a7d52954a55f4dcb31bff678fbe654e2e5341076007416caad5b8c4dc94`  
		Last Modified: Fri, 10 Feb 2023 07:36:16 GMT  
		Size: 41.5 MB (41507074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4be7ec8dab8442b6738c0fb28368b71b42c458b658393e7b54a404971511da`  
		Last Modified: Fri, 10 Feb 2023 07:36:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:fc102f828ca9dc2878b61e68bd31609ba1a29e1ccc1500489a03c4d73bdf77bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bc5498388a6a51559b9772559d5ac3e6040317fee182b3d460947e995486e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 09 Feb 2023 21:13:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98825686562eec0e4213e16e3734b97e44fa66bc3c69e516e31af1820939f93`  
		Last Modified: Thu, 09 Feb 2023 21:13:54 GMT  
		Size: 40.3 MB (40305460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8318a7b649fffb5e902a0b741a5c54d51ee7b0a6b6715295c031b94293d666b`  
		Last Modified: Thu, 09 Feb 2023 21:13:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4-alpine`

```console
$ docker pull telegraf@sha256:2e2e14c99c17464602e65cd89a095b755410b01853a88f8a1e0e137841b33167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ea87e6530418dea56b240838bf620c00625c9273b928ea82387e59869f4b035f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50404478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4256548ab14d2ac9434897e2f54eb4bba0e80a33a8a74333f2d6a9ba0235a67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 11 Feb 2023 14:08:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sat, 11 Feb 2023 14:08:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 11 Feb 2023 14:08:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 14:08:16 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 11 Feb 2023 14:08:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:08:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c72f3490ef958b34abba3216f60222ce0a09bc3ba25392ea46cf1e62813b6`  
		Last Modified: Sat, 11 Feb 2023 14:09:12 GMT  
		Size: 44.3 MB (44297832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ef14f3c9c3ce5940dfdfe7deaef2e8505d4b8ee41f0a73ad76493ebf4269f0`  
		Last Modified: Sat, 11 Feb 2023 14:09:05 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:62e35a0740d8b26b712f87ca2f052a78e375f3905fe2df8214b0314e6aa7a63a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:95a250a62c508d873a68303826f33452352a31b96d7e1413b0f147fde225d893
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136408213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8699c4d8ea4c21f8d00b82f56e7f4e49309e1d4ca1dd0879b19c499a369ab55`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:20:17 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:20:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785a618ce17aa0251054e585c435ab62626c52da138ff96b7a962d317e4261be`  
		Last Modified: Tue, 14 Feb 2023 00:21:03 GMT  
		Size: 46.6 MB (46556507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52926a97fe6d19223a3dfc349eb0e31cd76c444c7971813230d31455794e0157`  
		Last Modified: Tue, 14 Feb 2023 00:20:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c01ba0460e20900a3db68dd5aa68dc60a7c26cff31692c901ca909ab6e40cc94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126191050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678acdbf12bd32cca75a8c164d1fa20eb0291125a94b83e73e50568fc893da9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:30:09 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:30:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:30:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:30:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:30:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c438dafb249caaded45ac617e3a4b955d82421a3d532704b440909d8503bc39f`  
		Last Modified: Tue, 14 Feb 2023 00:30:56 GMT  
		Size: 43.4 MB (43361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf98b54365b8dc9738d1ecfc5b75e9a8463849ff4f1aea21abd6469d9c66387`  
		Last Modified: Tue, 14 Feb 2023 00:30:47 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3404002f25c3565f82b626675f4c77650e88b58f56feece08ce816aff9d92bb9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130619872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c51e014d51045d55be46ef9f1a95c231b4bb7626602ca42f7ccb2eb1c7d23c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Feb 2023 23:46:56 GMT
ENV TELEGRAF_VERSION=1.25.2
# Mon, 13 Feb 2023 23:47:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Feb 2023 23:47:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Feb 2023 23:47:02 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Feb 2023 23:47:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Feb 2023 23:47:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb79a0e15a5c5586a3d84a6b1c04401bb0a38f9cbbb48153fed650f5ac6a3ce`  
		Last Modified: Mon, 13 Feb 2023 23:47:22 GMT  
		Size: 42.3 MB (42290314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a62448c3c566f23c3e474b690942bab4026abb70a4299e4f1e3a8082f34e1f9`  
		Last Modified: Mon, 13 Feb 2023 23:47:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:5f8e4e68c928527997013b450849c4080d3f3fdde8fceccf995769d8b3b3f06c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4aa69cce85d7d9f6eb478a2a913aa3fb7ae4e69139a853a4e320d58440cf36e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52477643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9649518e44c1b172c648867e3aa895eaad584f7ed4f64f512c6abad8dd6464d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 14 Feb 2023 00:20:27 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 14 Feb 2023 00:20:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3c31b28da4569a5041683f5798e26109236281de69401d20d1dfb49459e89a`  
		Last Modified: Tue, 14 Feb 2023 00:21:21 GMT  
		Size: 46.4 MB (46370997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92235faf2fe9f66b7cd08fe4db4357c829e05a80ae8fbf1d07142a94d73f4c3f`  
		Last Modified: Tue, 14 Feb 2023 00:21:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.2`

```console
$ docker pull telegraf@sha256:62e35a0740d8b26b712f87ca2f052a78e375f3905fe2df8214b0314e6aa7a63a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.2` - linux; amd64

```console
$ docker pull telegraf@sha256:95a250a62c508d873a68303826f33452352a31b96d7e1413b0f147fde225d893
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136408213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8699c4d8ea4c21f8d00b82f56e7f4e49309e1d4ca1dd0879b19c499a369ab55`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:20:17 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:20:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785a618ce17aa0251054e585c435ab62626c52da138ff96b7a962d317e4261be`  
		Last Modified: Tue, 14 Feb 2023 00:21:03 GMT  
		Size: 46.6 MB (46556507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52926a97fe6d19223a3dfc349eb0e31cd76c444c7971813230d31455794e0157`  
		Last Modified: Tue, 14 Feb 2023 00:20:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c01ba0460e20900a3db68dd5aa68dc60a7c26cff31692c901ca909ab6e40cc94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126191050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678acdbf12bd32cca75a8c164d1fa20eb0291125a94b83e73e50568fc893da9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:30:09 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:30:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:30:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:30:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:30:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c438dafb249caaded45ac617e3a4b955d82421a3d532704b440909d8503bc39f`  
		Last Modified: Tue, 14 Feb 2023 00:30:56 GMT  
		Size: 43.4 MB (43361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf98b54365b8dc9738d1ecfc5b75e9a8463849ff4f1aea21abd6469d9c66387`  
		Last Modified: Tue, 14 Feb 2023 00:30:47 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3404002f25c3565f82b626675f4c77650e88b58f56feece08ce816aff9d92bb9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130619872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c51e014d51045d55be46ef9f1a95c231b4bb7626602ca42f7ccb2eb1c7d23c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Feb 2023 23:46:56 GMT
ENV TELEGRAF_VERSION=1.25.2
# Mon, 13 Feb 2023 23:47:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Feb 2023 23:47:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Feb 2023 23:47:02 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Feb 2023 23:47:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Feb 2023 23:47:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb79a0e15a5c5586a3d84a6b1c04401bb0a38f9cbbb48153fed650f5ac6a3ce`  
		Last Modified: Mon, 13 Feb 2023 23:47:22 GMT  
		Size: 42.3 MB (42290314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a62448c3c566f23c3e474b690942bab4026abb70a4299e4f1e3a8082f34e1f9`  
		Last Modified: Mon, 13 Feb 2023 23:47:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.2-alpine`

```console
$ docker pull telegraf@sha256:5f8e4e68c928527997013b450849c4080d3f3fdde8fceccf995769d8b3b3f06c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4aa69cce85d7d9f6eb478a2a913aa3fb7ae4e69139a853a4e320d58440cf36e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52477643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9649518e44c1b172c648867e3aa895eaad584f7ed4f64f512c6abad8dd6464d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 14 Feb 2023 00:20:27 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 14 Feb 2023 00:20:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3c31b28da4569a5041683f5798e26109236281de69401d20d1dfb49459e89a`  
		Last Modified: Tue, 14 Feb 2023 00:21:21 GMT  
		Size: 46.4 MB (46370997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92235faf2fe9f66b7cd08fe4db4357c829e05a80ae8fbf1d07142a94d73f4c3f`  
		Last Modified: Tue, 14 Feb 2023 00:21:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:5f8e4e68c928527997013b450849c4080d3f3fdde8fceccf995769d8b3b3f06c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4aa69cce85d7d9f6eb478a2a913aa3fb7ae4e69139a853a4e320d58440cf36e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52477643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9649518e44c1b172c648867e3aa895eaad584f7ed4f64f512c6abad8dd6464d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 14 Feb 2023 00:20:27 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 14 Feb 2023 00:20:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3c31b28da4569a5041683f5798e26109236281de69401d20d1dfb49459e89a`  
		Last Modified: Tue, 14 Feb 2023 00:21:21 GMT  
		Size: 46.4 MB (46370997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92235faf2fe9f66b7cd08fe4db4357c829e05a80ae8fbf1d07142a94d73f4c3f`  
		Last Modified: Tue, 14 Feb 2023 00:21:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:62e35a0740d8b26b712f87ca2f052a78e375f3905fe2df8214b0314e6aa7a63a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:95a250a62c508d873a68303826f33452352a31b96d7e1413b0f147fde225d893
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136408213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8699c4d8ea4c21f8d00b82f56e7f4e49309e1d4ca1dd0879b19c499a369ab55`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 11 Feb 2023 03:43:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 11 Feb 2023 03:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:20:17 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:20:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c45678ee92be805f3bb9e319e7413cfbf9e7a6664212b0df2b948cb16bd70`  
		Last Modified: Sat, 11 Feb 2023 03:44:16 GMT  
		Size: 18.8 MB (18760006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9494f4cdf48f3c7ab1cf7dbb7104861fc2b19bed508cebb46bf80b21a80f1e8b`  
		Last Modified: Sat, 11 Feb 2023 03:44:13 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785a618ce17aa0251054e585c435ab62626c52da138ff96b7a962d317e4261be`  
		Last Modified: Tue, 14 Feb 2023 00:21:03 GMT  
		Size: 46.6 MB (46556507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52926a97fe6d19223a3dfc349eb0e31cd76c444c7971813230d31455794e0157`  
		Last Modified: Tue, 14 Feb 2023 00:20:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c01ba0460e20900a3db68dd5aa68dc60a7c26cff31692c901ca909ab6e40cc94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126191050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678acdbf12bd32cca75a8c164d1fa20eb0291125a94b83e73e50568fc893da9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 07:34:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 07:34:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 14 Feb 2023 00:30:09 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Feb 2023 00:30:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:30:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 14 Feb 2023 00:30:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:30:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2fff1078b66b8cce5e0fb8940f73d3369a304f0c72e76c768740f68dd6eb6`  
		Last Modified: Thu, 09 Feb 2023 17:47:05 GMT  
		Size: 4.9 MB (4934034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29288d9697500ec9b229f20d8fb486702e9751dd06ca3b694bd49c34769b479`  
		Last Modified: Thu, 09 Feb 2023 17:47:06 GMT  
		Size: 10.2 MB (10217702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae143166fa1336280214d308cdad2d6884b6926ede5e0f21a3647b58766ea674`  
		Last Modified: Fri, 10 Feb 2023 07:35:53 GMT  
		Size: 17.5 MB (17462301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906f50e92186dc755dde4da63b1ec2519fcab94e415d126e036f12ba2d5f68`  
		Last Modified: Fri, 10 Feb 2023 07:35:49 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c438dafb249caaded45ac617e3a4b955d82421a3d532704b440909d8503bc39f`  
		Last Modified: Tue, 14 Feb 2023 00:30:56 GMT  
		Size: 43.4 MB (43361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf98b54365b8dc9738d1ecfc5b75e9a8463849ff4f1aea21abd6469d9c66387`  
		Last Modified: Tue, 14 Feb 2023 00:30:47 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3404002f25c3565f82b626675f4c77650e88b58f56feece08ce816aff9d92bb9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130619872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c51e014d51045d55be46ef9f1a95c231b4bb7626602ca42f7ccb2eb1c7d23c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Feb 2023 23:46:56 GMT
ENV TELEGRAF_VERSION=1.25.2
# Mon, 13 Feb 2023 23:47:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Feb 2023 23:47:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Feb 2023 23:47:02 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Feb 2023 23:47:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Feb 2023 23:47:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb79a0e15a5c5586a3d84a6b1c04401bb0a38f9cbbb48153fed650f5ac6a3ce`  
		Last Modified: Mon, 13 Feb 2023 23:47:22 GMT  
		Size: 42.3 MB (42290314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a62448c3c566f23c3e474b690942bab4026abb70a4299e4f1e3a8082f34e1f9`  
		Last Modified: Mon, 13 Feb 2023 23:47:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
