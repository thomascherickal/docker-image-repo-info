<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8.8`](#chronograf188)
-	[`chronograf:1.8.8-alpine`](#chronograf188-alpine)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:7e05862e478a36db91a13f116b3147f818827d15b872c24b2671d341d3789718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:730fc77be2ecc963a903da0dfc48339111892743e84020e68dc143f77c2d3d61
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49331737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbd494d2fb674c25c520b18cdff32cf525e101b0b5b77b1005037e8db115945`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:09:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 02:09:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 13 Oct 2020 02:10:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:10:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Oct 2020 02:10:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Oct 2020 02:10:04 GMT
EXPOSE 8888
# Tue, 13 Oct 2020 02:10:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Oct 2020 02:10:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Oct 2020 02:10:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:10:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5c5a69c41807fd6b8c3b31003954bcde4dfc6b36fd4e0fbb056c39c793c97`  
		Last Modified: Tue, 13 Oct 2020 02:11:28 GMT  
		Size: 6.7 MB (6742155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13139271cc70660aba18c725cbe170524b2238d8e8ec10917322461927b60c70`  
		Last Modified: Tue, 13 Oct 2020 02:11:31 GMT  
		Size: 20.0 MB (20043093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ba67456ac130d784b6bb1893fdd10e5f3e1adc5006ef2a26d3c85c1ac0398`  
		Last Modified: Tue, 13 Oct 2020 02:11:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b8236ad7c97e8cc15c0c8b2cda94988fa4df91b0ccf8586363ba04e89da57d`  
		Last Modified: Tue, 13 Oct 2020 02:11:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a542b1d04b069ac77d64f3852533185ad3af43b12ff3c5e81608b6c132df87f6`  
		Last Modified: Tue, 13 Oct 2020 02:11:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3f3a92712d9e8896813694dc213be61fe743f2b1d3ff20878893d7a005b3fc7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43918507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201ad85b3c894637673b93f2e26ca7b8a520a3c4b32ea94ad41c0060e0895b5e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:15:07 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 17 Nov 2020 22:15:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:15:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:15:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:15:30 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:15:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:15:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:15:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:15:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5461676b0138b7ba57686fda461abe72ccfca32e9bb593759bb939828ea6a3`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 5.8 MB (5764642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e5a1478ad81e88813aaae39ea42ea6a56b31383d37a80026fc968464ef1ea`  
		Last Modified: Tue, 17 Nov 2020 22:17:44 GMT  
		Size: 18.8 MB (18816245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a63b20cef225a26d560966a29b75c93b89115300032cdda2a8faa73e4fe239`  
		Last Modified: Tue, 17 Nov 2020 22:17:38 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193c4eb87a678383202fff2db3e49b58bbb07a446eb0f59f4eb47816fc707e6f`  
		Last Modified: Tue, 17 Nov 2020 22:17:38 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c083af453f4e40efafa3e935d92158f6ad096858dddbefc4b896da6c1291422`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:035067b14a15ed5fc82a2d78fde7965ec2e0ff00f435a1300d36b2284304524b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45398395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cc48cf404ecda81785200a89da1268e0165510901a8cf690a30766b3e94329`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:43:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 17 Nov 2020 22:43:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:43:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:43:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:43:45 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:43:46 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:43:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:43:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:43:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31471b97a05001c188b69228f8341987e6e04e62decf66d8e8013c9fa62a90f`  
		Last Modified: Tue, 17 Nov 2020 22:45:26 GMT  
		Size: 6.0 MB (6027836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1679bbb8d17fef26f89803ce73b0f3e924afff7505b1d3946603a601f2244`  
		Last Modified: Tue, 17 Nov 2020 22:45:28 GMT  
		Size: 19.0 MB (18958390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2d77bb23b9a7f0a89e91f1fad31b352731329f41402ae7507b0042920e3d6b`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cbfe158e5b3e1c4fff01acbc21270031a781e17f2f15756b6388def3ed161`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c71705cb89f7891bcd9b29929fdef2481dca3fdb271bcf19d029c489eec4b4`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:7e05862e478a36db91a13f116b3147f818827d15b872c24b2671d341d3789718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:730fc77be2ecc963a903da0dfc48339111892743e84020e68dc143f77c2d3d61
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49331737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbd494d2fb674c25c520b18cdff32cf525e101b0b5b77b1005037e8db115945`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:09:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 02:09:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 13 Oct 2020 02:10:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:10:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Oct 2020 02:10:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Oct 2020 02:10:04 GMT
EXPOSE 8888
# Tue, 13 Oct 2020 02:10:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Oct 2020 02:10:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Oct 2020 02:10:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:10:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5c5a69c41807fd6b8c3b31003954bcde4dfc6b36fd4e0fbb056c39c793c97`  
		Last Modified: Tue, 13 Oct 2020 02:11:28 GMT  
		Size: 6.7 MB (6742155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13139271cc70660aba18c725cbe170524b2238d8e8ec10917322461927b60c70`  
		Last Modified: Tue, 13 Oct 2020 02:11:31 GMT  
		Size: 20.0 MB (20043093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ba67456ac130d784b6bb1893fdd10e5f3e1adc5006ef2a26d3c85c1ac0398`  
		Last Modified: Tue, 13 Oct 2020 02:11:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b8236ad7c97e8cc15c0c8b2cda94988fa4df91b0ccf8586363ba04e89da57d`  
		Last Modified: Tue, 13 Oct 2020 02:11:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a542b1d04b069ac77d64f3852533185ad3af43b12ff3c5e81608b6c132df87f6`  
		Last Modified: Tue, 13 Oct 2020 02:11:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3f3a92712d9e8896813694dc213be61fe743f2b1d3ff20878893d7a005b3fc7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43918507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201ad85b3c894637673b93f2e26ca7b8a520a3c4b32ea94ad41c0060e0895b5e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:15:07 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 17 Nov 2020 22:15:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:15:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:15:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:15:30 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:15:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:15:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:15:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:15:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5461676b0138b7ba57686fda461abe72ccfca32e9bb593759bb939828ea6a3`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 5.8 MB (5764642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e5a1478ad81e88813aaae39ea42ea6a56b31383d37a80026fc968464ef1ea`  
		Last Modified: Tue, 17 Nov 2020 22:17:44 GMT  
		Size: 18.8 MB (18816245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a63b20cef225a26d560966a29b75c93b89115300032cdda2a8faa73e4fe239`  
		Last Modified: Tue, 17 Nov 2020 22:17:38 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193c4eb87a678383202fff2db3e49b58bbb07a446eb0f59f4eb47816fc707e6f`  
		Last Modified: Tue, 17 Nov 2020 22:17:38 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c083af453f4e40efafa3e935d92158f6ad096858dddbefc4b896da6c1291422`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:035067b14a15ed5fc82a2d78fde7965ec2e0ff00f435a1300d36b2284304524b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45398395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cc48cf404ecda81785200a89da1268e0165510901a8cf690a30766b3e94329`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:43:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 17 Nov 2020 22:43:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:43:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:43:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:43:45 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:43:46 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:43:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:43:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:43:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31471b97a05001c188b69228f8341987e6e04e62decf66d8e8013c9fa62a90f`  
		Last Modified: Tue, 17 Nov 2020 22:45:26 GMT  
		Size: 6.0 MB (6027836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1679bbb8d17fef26f89803ce73b0f3e924afff7505b1d3946603a601f2244`  
		Last Modified: Tue, 17 Nov 2020 22:45:28 GMT  
		Size: 19.0 MB (18958390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2d77bb23b9a7f0a89e91f1fad31b352731329f41402ae7507b0042920e3d6b`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cbfe158e5b3e1c4fff01acbc21270031a781e17f2f15756b6388def3ed161`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c71705cb89f7891bcd9b29929fdef2481dca3fdb271bcf19d029c489eec4b4`  
		Last Modified: Tue, 17 Nov 2020 22:45:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:246926c7eb235266c7f7061cdd8e479ee892628af7eab3c1b76d86a843fce7ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:8b473e8c7361ed08efa694af78586f5b1bb0099c268ea5891f651c05c74697df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14838991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d504255af6e2c14e3c28b1b0f94f3fc623391078a507f1dbde513fcd21a5edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 22 Oct 2020 02:55:00 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Oct 2020 02:55:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 22 Oct 2020 02:55:05 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Thu, 22 Oct 2020 02:55:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Oct 2020 02:55:06 GMT
EXPOSE 8888
# Thu, 22 Oct 2020 02:55:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Oct 2020 02:55:06 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 22 Oct 2020 02:55:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:55:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98c701704af1e7af9feb343fc851a39bea7eb0372cca880af3ec5b088fa07`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 11.7 MB (11736797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa4a29f6057eb813dab6f0d7c56159ded9d926e19f2317ced58f77c5f8214`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 12.2 KB (12238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d7b39d647c5685e4d46c06c692c287b09dc934603db662779b44a3e368708a`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e58507b0200b84f82382a3bc2e249c87af9de14651fa16b6480fd97d9ec5b`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:246926c7eb235266c7f7061cdd8e479ee892628af7eab3c1b76d86a843fce7ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:8b473e8c7361ed08efa694af78586f5b1bb0099c268ea5891f651c05c74697df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14838991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d504255af6e2c14e3c28b1b0f94f3fc623391078a507f1dbde513fcd21a5edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 22 Oct 2020 02:55:00 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Oct 2020 02:55:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 22 Oct 2020 02:55:05 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Thu, 22 Oct 2020 02:55:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Oct 2020 02:55:06 GMT
EXPOSE 8888
# Thu, 22 Oct 2020 02:55:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Oct 2020 02:55:06 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 22 Oct 2020 02:55:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:55:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98c701704af1e7af9feb343fc851a39bea7eb0372cca880af3ec5b088fa07`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 11.7 MB (11736797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa4a29f6057eb813dab6f0d7c56159ded9d926e19f2317ced58f77c5f8214`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 12.2 KB (12238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d7b39d647c5685e4d46c06c692c287b09dc934603db662779b44a3e368708a`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e58507b0200b84f82382a3bc2e249c87af9de14651fa16b6480fd97d9ec5b`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:87e5d8f3632f8a501da2806411e48be21f5a91ff4e12305d4e7b252883c6b0b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:3533968f29b426f02c66987bd647a4d9ebf8645852aed19a6bb9ce5d5c89cbfb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65359789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6529b65fc10dcd4132647a69ed012c5b9a9d30364b1e919c58d0ba40d96f21`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:10:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 02:10:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Oct 2020 02:10:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:10:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Oct 2020 02:10:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Oct 2020 02:10:39 GMT
EXPOSE 8888
# Tue, 13 Oct 2020 02:10:40 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Oct 2020 02:10:40 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Oct 2020 02:10:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:10:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec3defa80f9f791ef2ad4f00149fb9a0e7a58a2a28e30a7986892707d7f356b`  
		Last Modified: Tue, 13 Oct 2020 02:11:36 GMT  
		Size: 4.5 MB (4504590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fb87e5ab3a014feb951ec022797f22837851d85257fd2be6afc6f07e818485`  
		Last Modified: Tue, 13 Oct 2020 02:11:42 GMT  
		Size: 38.3 MB (38308704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7caa5f92192ae6cf98f07de594d92a0d2cb84a0fcba120c93275417f437d4e3`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b07d6bf1b58a82bbec48bc361fad5633064b48c142a4a53c16ca0aa6eb7ed4`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0f9231deddae6cbcc5822e6eb81dd3f84b845c9d07caae0f0b7a19c4f0fa48`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b26979a467679005a3af84f688c44b7d3ec9c8ce14b9b16daa694b16914e3b71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58969019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b1c61a361971a9ab6a5e9d79687d04cf5ed7646c6300ffaa460ae8370b5b9cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:16:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:16:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 17 Nov 2020 22:16:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:16:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:16:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:16:34 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:16:36 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:16:38 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:16:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:16:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9a110e8d78f226df49f7046995bd62fe5934dfe4ce3461e81de7eeb29e2a9e`  
		Last Modified: Tue, 17 Nov 2020 22:17:53 GMT  
		Size: 3.9 MB (3879429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c458aa9cfd5e3b0fc14a275ff2c2b73b2b5b55406e49e204393a5a6505117cad`  
		Last Modified: Tue, 17 Nov 2020 22:18:03 GMT  
		Size: 35.8 MB (35751979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2734caa8d14e3feec2396dc59cf228c186cc9d1871987f7c23887da9240c0308`  
		Last Modified: Tue, 17 Nov 2020 22:17:52 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180354145eb509f9837b003b622e2c9776c6f53c0da00b8f081ebee52f5afca1`  
		Last Modified: Tue, 17 Nov 2020 22:17:52 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641bbab5be50154520bed88952a43cacae4c68e90522e4d6e509a96b7dca441`  
		Last Modified: Tue, 17 Nov 2020 22:17:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c13fe1c52ac8b4e33c013ed54cd7eab4f0996e09bd7c6882b58b2fd427c9edd0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60455554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ba10aa70e3dd6ebffb9c4e1bb9e08e79823c9f7c9cd83fe334f6e479f7a087`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:44:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:44:11 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 17 Nov 2020 22:44:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:44:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:44:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:44:32 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:44:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:44:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:44:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:44:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624272aeeab8c713a9f6b50cced823f5a3503714c0bf3d5f186d3e766ccef685`  
		Last Modified: Tue, 17 Nov 2020 22:45:37 GMT  
		Size: 4.1 MB (4082063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6907346db29580e3b76519e6717d8771f84d2494e82a669469202b3602e44f1c`  
		Last Modified: Tue, 17 Nov 2020 22:45:45 GMT  
		Size: 36.0 MB (35961315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f689f38d3b68a16efd9963bc3799ab32e3eb8d7f1b3ea795aba077f9526bae`  
		Last Modified: Tue, 17 Nov 2020 22:45:36 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016ef61645558447ab068e256b13877931389896d26ec863600e513a1cf6e59`  
		Last Modified: Tue, 17 Nov 2020 22:45:36 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799242819d8c426641c17743c5064d7f7f53c7b6b220d11b5b729d4fbd97d3b`  
		Last Modified: Tue, 17 Nov 2020 22:45:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:87e5d8f3632f8a501da2806411e48be21f5a91ff4e12305d4e7b252883c6b0b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:3533968f29b426f02c66987bd647a4d9ebf8645852aed19a6bb9ce5d5c89cbfb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65359789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6529b65fc10dcd4132647a69ed012c5b9a9d30364b1e919c58d0ba40d96f21`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:10:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 13 Oct 2020 02:10:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Oct 2020 02:10:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:10:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Oct 2020 02:10:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Oct 2020 02:10:39 GMT
EXPOSE 8888
# Tue, 13 Oct 2020 02:10:40 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Oct 2020 02:10:40 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Oct 2020 02:10:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:10:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec3defa80f9f791ef2ad4f00149fb9a0e7a58a2a28e30a7986892707d7f356b`  
		Last Modified: Tue, 13 Oct 2020 02:11:36 GMT  
		Size: 4.5 MB (4504590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fb87e5ab3a014feb951ec022797f22837851d85257fd2be6afc6f07e818485`  
		Last Modified: Tue, 13 Oct 2020 02:11:42 GMT  
		Size: 38.3 MB (38308704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7caa5f92192ae6cf98f07de594d92a0d2cb84a0fcba120c93275417f437d4e3`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b07d6bf1b58a82bbec48bc361fad5633064b48c142a4a53c16ca0aa6eb7ed4`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0f9231deddae6cbcc5822e6eb81dd3f84b845c9d07caae0f0b7a19c4f0fa48`  
		Last Modified: Tue, 13 Oct 2020 02:11:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b26979a467679005a3af84f688c44b7d3ec9c8ce14b9b16daa694b16914e3b71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58969019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b1c61a361971a9ab6a5e9d79687d04cf5ed7646c6300ffaa460ae8370b5b9cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:16:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:16:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 17 Nov 2020 22:16:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:16:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:16:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:16:34 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:16:36 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:16:38 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:16:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:16:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9a110e8d78f226df49f7046995bd62fe5934dfe4ce3461e81de7eeb29e2a9e`  
		Last Modified: Tue, 17 Nov 2020 22:17:53 GMT  
		Size: 3.9 MB (3879429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c458aa9cfd5e3b0fc14a275ff2c2b73b2b5b55406e49e204393a5a6505117cad`  
		Last Modified: Tue, 17 Nov 2020 22:18:03 GMT  
		Size: 35.8 MB (35751979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2734caa8d14e3feec2396dc59cf228c186cc9d1871987f7c23887da9240c0308`  
		Last Modified: Tue, 17 Nov 2020 22:17:52 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180354145eb509f9837b003b622e2c9776c6f53c0da00b8f081ebee52f5afca1`  
		Last Modified: Tue, 17 Nov 2020 22:17:52 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641bbab5be50154520bed88952a43cacae4c68e90522e4d6e509a96b7dca441`  
		Last Modified: Tue, 17 Nov 2020 22:17:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c13fe1c52ac8b4e33c013ed54cd7eab4f0996e09bd7c6882b58b2fd427c9edd0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60455554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ba10aa70e3dd6ebffb9c4e1bb9e08e79823c9f7c9cd83fe334f6e479f7a087`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:44:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:44:11 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 17 Nov 2020 22:44:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:44:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:44:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:44:32 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:44:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:44:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:44:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:44:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624272aeeab8c713a9f6b50cced823f5a3503714c0bf3d5f186d3e766ccef685`  
		Last Modified: Tue, 17 Nov 2020 22:45:37 GMT  
		Size: 4.1 MB (4082063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6907346db29580e3b76519e6717d8771f84d2494e82a669469202b3602e44f1c`  
		Last Modified: Tue, 17 Nov 2020 22:45:45 GMT  
		Size: 36.0 MB (35961315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f689f38d3b68a16efd9963bc3799ab32e3eb8d7f1b3ea795aba077f9526bae`  
		Last Modified: Tue, 17 Nov 2020 22:45:36 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016ef61645558447ab068e256b13877931389896d26ec863600e513a1cf6e59`  
		Last Modified: Tue, 17 Nov 2020 22:45:36 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799242819d8c426641c17743c5064d7f7f53c7b6b220d11b5b729d4fbd97d3b`  
		Last Modified: Tue, 17 Nov 2020 22:45:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:7c3e23b76aee672373d9d1d982380d4afe0eec4efd56951fe922bf46c0108e1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:87e4c1ab08dac75daa497243e090f6554cbd8060f610cd04ca66cab556170c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22657450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16816a1091a90cadea376ffeb65e85306b4a4a0b3b2883fe2c0b8cd8d51822b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 22 Oct 2020 02:55:17 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Oct 2020 02:55:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 22 Oct 2020 02:55:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Oct 2020 02:55:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Oct 2020 02:55:23 GMT
EXPOSE 8888
# Thu, 22 Oct 2020 02:55:24 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Oct 2020 02:55:24 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 22 Oct 2020 02:55:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:55:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049dc3779eaa76ec7e5631f721bb2df67ffc0ae0c835dacb7f6c3c1d5a29db62`  
		Last Modified: Thu, 22 Oct 2020 02:56:18 GMT  
		Size: 19.6 MB (19555245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cca6e73343294d6c4d222c76784f6de8e9775945afed035df3a88e9547289c`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c45fcc1cc26198e5eda0c08ca51cdf0e8ac4604cb3602f5b56264885d6d107`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef77cd0742fa18cacd87b9d9c8bd4bf0cc0d6c94adcd70172448edf6dc6143a`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:7c3e23b76aee672373d9d1d982380d4afe0eec4efd56951fe922bf46c0108e1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:87e4c1ab08dac75daa497243e090f6554cbd8060f610cd04ca66cab556170c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22657450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16816a1091a90cadea376ffeb65e85306b4a4a0b3b2883fe2c0b8cd8d51822b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 22 Oct 2020 02:55:17 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Oct 2020 02:55:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 22 Oct 2020 02:55:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Oct 2020 02:55:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Oct 2020 02:55:23 GMT
EXPOSE 8888
# Thu, 22 Oct 2020 02:55:24 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Oct 2020 02:55:24 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 22 Oct 2020 02:55:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:55:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049dc3779eaa76ec7e5631f721bb2df67ffc0ae0c835dacb7f6c3c1d5a29db62`  
		Last Modified: Thu, 22 Oct 2020 02:56:18 GMT  
		Size: 19.6 MB (19555245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cca6e73343294d6c4d222c76784f6de8e9775945afed035df3a88e9547289c`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c45fcc1cc26198e5eda0c08ca51cdf0e8ac4604cb3602f5b56264885d6d107`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef77cd0742fa18cacd87b9d9c8bd4bf0cc0d6c94adcd70172448edf6dc6143a`  
		Last Modified: Thu, 22 Oct 2020 02:56:12 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:82a33cafa3faea0119c499d02317fe012ea4486ae83a04ba686918bf79ce5d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:364a317b483d58ad680eda4923a98d336a9eca7505517c7afa361c0acd9a0c45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70416919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81126f11ded2cb40148cb7a0ffc886b22d1c765e40de151389ca4b4dfdb5d719`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:09:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 05 Nov 2020 00:19:52 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:02 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5c5a69c41807fd6b8c3b31003954bcde4dfc6b36fd4e0fbb056c39c793c97`  
		Last Modified: Tue, 13 Oct 2020 02:11:28 GMT  
		Size: 6.7 MB (6742155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50083d05b2c9638c681124e9b49d0135bce000d175536a70bd285e2ccbb8a1`  
		Last Modified: Thu, 05 Nov 2020 00:20:35 GMT  
		Size: 41.1 MB (41128276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b755a599080bad25c1297121352b31f045577f2330a0fba8738ed63044d4110`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ed7f68ca337a45a0bb4002ede9897a0d5786dfd0904984941e9f48b2f3a00b`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43e2af8c70cd03ac9cafd99bf15d892aa03415b3724966637e4499adf3d364e`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d51caca64e55e698d0ec1ee98dba2d4ee6e5530055b8be1e91d742def85d3541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bfe5d588f9e01f105d1668dfadea8278fcc6beac161e2a6c3d1f2151212e78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:16:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:17:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:17:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:17:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:17:22 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:17:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:17:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:17:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:17:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5461676b0138b7ba57686fda461abe72ccfca32e9bb593759bb939828ea6a3`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 5.8 MB (5764642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89732112fbae6aeeb8806ac08af582e8b0fc855ef4b2afd1970550def68c8d8a`  
		Last Modified: Tue, 17 Nov 2020 22:18:25 GMT  
		Size: 38.7 MB (38733936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188c76f40003ccab06b27417e650739fdf7e8381cd473db826298cf36375cc6`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd694c1536c6268949273074a32d31021fea8a40405feb71cf1688cc00a8ca2`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6f3fc68eb3028a589cefc66f7f54bf277178849be02d326f8c39cfef12508d`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17686e0de5796440eedce056489630f5ed4d8ab9f6c3707e8610b4e41ab78691
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c257287e007c2a7b2f98e515a9d48289df0403905c1420d758c3d44cf4bb099`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:44:47 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:45:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:45:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:45:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:45:03 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:45:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:45:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:45:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31471b97a05001c188b69228f8341987e6e04e62decf66d8e8013c9fa62a90f`  
		Last Modified: Tue, 17 Nov 2020 22:45:26 GMT  
		Size: 6.0 MB (6027836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dae08df397b700abc2a9afd939c062140901753c1c70cc7445bbdedbe898d0`  
		Last Modified: Tue, 17 Nov 2020 22:46:03 GMT  
		Size: 38.5 MB (38502245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fd088282455dabfbc7699f0b3952efe3abffb43f391d7567c6489f4d0483c`  
		Last Modified: Tue, 17 Nov 2020 22:45:55 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24bbde08decabe8e69a96d6da307735c3a7c3f2222ce0018d2a0198154d8a73`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fef33880f1c4d184ecadc4e74fec55a0f527ba6aac781f3e829b558592b9d6a`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:82a33cafa3faea0119c499d02317fe012ea4486ae83a04ba686918bf79ce5d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:364a317b483d58ad680eda4923a98d336a9eca7505517c7afa361c0acd9a0c45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70416919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81126f11ded2cb40148cb7a0ffc886b22d1c765e40de151389ca4b4dfdb5d719`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:09:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 05 Nov 2020 00:19:52 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:02 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5c5a69c41807fd6b8c3b31003954bcde4dfc6b36fd4e0fbb056c39c793c97`  
		Last Modified: Tue, 13 Oct 2020 02:11:28 GMT  
		Size: 6.7 MB (6742155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50083d05b2c9638c681124e9b49d0135bce000d175536a70bd285e2ccbb8a1`  
		Last Modified: Thu, 05 Nov 2020 00:20:35 GMT  
		Size: 41.1 MB (41128276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b755a599080bad25c1297121352b31f045577f2330a0fba8738ed63044d4110`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ed7f68ca337a45a0bb4002ede9897a0d5786dfd0904984941e9f48b2f3a00b`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43e2af8c70cd03ac9cafd99bf15d892aa03415b3724966637e4499adf3d364e`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d51caca64e55e698d0ec1ee98dba2d4ee6e5530055b8be1e91d742def85d3541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bfe5d588f9e01f105d1668dfadea8278fcc6beac161e2a6c3d1f2151212e78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:16:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:17:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:17:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:17:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:17:22 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:17:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:17:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:17:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:17:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5461676b0138b7ba57686fda461abe72ccfca32e9bb593759bb939828ea6a3`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 5.8 MB (5764642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89732112fbae6aeeb8806ac08af582e8b0fc855ef4b2afd1970550def68c8d8a`  
		Last Modified: Tue, 17 Nov 2020 22:18:25 GMT  
		Size: 38.7 MB (38733936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188c76f40003ccab06b27417e650739fdf7e8381cd473db826298cf36375cc6`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd694c1536c6268949273074a32d31021fea8a40405feb71cf1688cc00a8ca2`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6f3fc68eb3028a589cefc66f7f54bf277178849be02d326f8c39cfef12508d`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17686e0de5796440eedce056489630f5ed4d8ab9f6c3707e8610b4e41ab78691
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c257287e007c2a7b2f98e515a9d48289df0403905c1420d758c3d44cf4bb099`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:44:47 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:45:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:45:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:45:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:45:03 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:45:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:45:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:45:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31471b97a05001c188b69228f8341987e6e04e62decf66d8e8013c9fa62a90f`  
		Last Modified: Tue, 17 Nov 2020 22:45:26 GMT  
		Size: 6.0 MB (6027836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dae08df397b700abc2a9afd939c062140901753c1c70cc7445bbdedbe898d0`  
		Last Modified: Tue, 17 Nov 2020 22:46:03 GMT  
		Size: 38.5 MB (38502245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fd088282455dabfbc7699f0b3952efe3abffb43f391d7567c6489f4d0483c`  
		Last Modified: Tue, 17 Nov 2020 22:45:55 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24bbde08decabe8e69a96d6da307735c3a7c3f2222ce0018d2a0198154d8a73`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fef33880f1c4d184ecadc4e74fec55a0f527ba6aac781f3e829b558592b9d6a`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:6a8db053bf02a118ad81e2c80753354e36bfd8b09e413e49c2f90fe341360ce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3c13ab83668a324524129a12911188925beb4bb994e92663a05a93de3bf293fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0151e294e6c824ce37e9818967379364d034dd92f65d7f7f3674cbab9de95463`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 05 Nov 2020 00:20:08 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:13 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:13 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e06d277240720969af4b20362c38bc256876946f986cd854894383d703b9d`  
		Last Modified: Thu, 05 Nov 2020 00:21:02 GMT  
		Size: 22.2 MB (22245639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0f11b93f5183f604029385446a4bcfec5e376171051da12c64366cfe43bf0e`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddace948c9b77e0fa44a20a0f170953ab5a4bb2ea15b52b8bbcf2d04bf00d362`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f01e7d7a0a3888f9e3b7eef396baf4609df09430341a20b3f2295086bca340a`  
		Last Modified: Thu, 05 Nov 2020 00:20:59 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:6a8db053bf02a118ad81e2c80753354e36bfd8b09e413e49c2f90fe341360ce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3c13ab83668a324524129a12911188925beb4bb994e92663a05a93de3bf293fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0151e294e6c824ce37e9818967379364d034dd92f65d7f7f3674cbab9de95463`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 05 Nov 2020 00:20:08 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:13 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:13 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e06d277240720969af4b20362c38bc256876946f986cd854894383d703b9d`  
		Last Modified: Thu, 05 Nov 2020 00:21:02 GMT  
		Size: 22.2 MB (22245639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0f11b93f5183f604029385446a4bcfec5e376171051da12c64366cfe43bf0e`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddace948c9b77e0fa44a20a0f170953ab5a4bb2ea15b52b8bbcf2d04bf00d362`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f01e7d7a0a3888f9e3b7eef396baf4609df09430341a20b3f2295086bca340a`  
		Last Modified: Thu, 05 Nov 2020 00:20:59 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:6a8db053bf02a118ad81e2c80753354e36bfd8b09e413e49c2f90fe341360ce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3c13ab83668a324524129a12911188925beb4bb994e92663a05a93de3bf293fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0151e294e6c824ce37e9818967379364d034dd92f65d7f7f3674cbab9de95463`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:54:58 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:55:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 05 Nov 2020 00:20:08 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:13 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:13 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:13 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab57a7256718fa42bedfa2c660a5f0de9129121c4f27e021d960eea00eb85650`  
		Last Modified: Thu, 22 Oct 2020 02:56:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea603847a3b82b32a20eba9b8d97e8d5da78d7491d9412b148947a123d8c4ffd`  
		Last Modified: Thu, 22 Oct 2020 02:56:04 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e06d277240720969af4b20362c38bc256876946f986cd854894383d703b9d`  
		Last Modified: Thu, 05 Nov 2020 00:21:02 GMT  
		Size: 22.2 MB (22245639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0f11b93f5183f604029385446a4bcfec5e376171051da12c64366cfe43bf0e`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddace948c9b77e0fa44a20a0f170953ab5a4bb2ea15b52b8bbcf2d04bf00d362`  
		Last Modified: Thu, 05 Nov 2020 00:20:58 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f01e7d7a0a3888f9e3b7eef396baf4609df09430341a20b3f2295086bca340a`  
		Last Modified: Thu, 05 Nov 2020 00:20:59 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:82a33cafa3faea0119c499d02317fe012ea4486ae83a04ba686918bf79ce5d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:364a317b483d58ad680eda4923a98d336a9eca7505517c7afa361c0acd9a0c45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70416919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81126f11ded2cb40148cb7a0ffc886b22d1c765e40de151389ca4b4dfdb5d719`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:09:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 05 Nov 2020 00:19:52 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 05 Nov 2020 00:20:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 05 Nov 2020 00:20:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 05 Nov 2020 00:20:02 GMT
EXPOSE 8888
# Thu, 05 Nov 2020 00:20:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 05 Nov 2020 00:20:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 05 Nov 2020 00:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 00:20:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5c5a69c41807fd6b8c3b31003954bcde4dfc6b36fd4e0fbb056c39c793c97`  
		Last Modified: Tue, 13 Oct 2020 02:11:28 GMT  
		Size: 6.7 MB (6742155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50083d05b2c9638c681124e9b49d0135bce000d175536a70bd285e2ccbb8a1`  
		Last Modified: Thu, 05 Nov 2020 00:20:35 GMT  
		Size: 41.1 MB (41128276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b755a599080bad25c1297121352b31f045577f2330a0fba8738ed63044d4110`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ed7f68ca337a45a0bb4002ede9897a0d5786dfd0904984941e9f48b2f3a00b`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43e2af8c70cd03ac9cafd99bf15d892aa03415b3724966637e4499adf3d364e`  
		Last Modified: Thu, 05 Nov 2020 00:20:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d51caca64e55e698d0ec1ee98dba2d4ee6e5530055b8be1e91d742def85d3541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bfe5d588f9e01f105d1668dfadea8278fcc6beac161e2a6c3d1f2151212e78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:16:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:17:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:17:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:17:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:17:22 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:17:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:17:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:17:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:17:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5461676b0138b7ba57686fda461abe72ccfca32e9bb593759bb939828ea6a3`  
		Last Modified: Tue, 17 Nov 2020 22:17:40 GMT  
		Size: 5.8 MB (5764642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89732112fbae6aeeb8806ac08af582e8b0fc855ef4b2afd1970550def68c8d8a`  
		Last Modified: Tue, 17 Nov 2020 22:18:25 GMT  
		Size: 38.7 MB (38733936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188c76f40003ccab06b27417e650739fdf7e8381cd473db826298cf36375cc6`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd694c1536c6268949273074a32d31021fea8a40405feb71cf1688cc00a8ca2`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6f3fc68eb3028a589cefc66f7f54bf277178849be02d326f8c39cfef12508d`  
		Last Modified: Tue, 17 Nov 2020 22:18:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17686e0de5796440eedce056489630f5ed4d8ab9f6c3707e8610b4e41ab78691
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c257287e007c2a7b2f98e515a9d48289df0403905c1420d758c3d44cf4bb099`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 17 Nov 2020 22:44:47 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 17 Nov 2020 22:45:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:45:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 17 Nov 2020 22:45:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 17 Nov 2020 22:45:03 GMT
EXPOSE 8888
# Tue, 17 Nov 2020 22:45:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 17 Nov 2020 22:45:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 17 Nov 2020 22:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Nov 2020 22:45:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31471b97a05001c188b69228f8341987e6e04e62decf66d8e8013c9fa62a90f`  
		Last Modified: Tue, 17 Nov 2020 22:45:26 GMT  
		Size: 6.0 MB (6027836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dae08df397b700abc2a9afd939c062140901753c1c70cc7445bbdedbe898d0`  
		Last Modified: Tue, 17 Nov 2020 22:46:03 GMT  
		Size: 38.5 MB (38502245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fd088282455dabfbc7699f0b3952efe3abffb43f391d7567c6489f4d0483c`  
		Last Modified: Tue, 17 Nov 2020 22:45:55 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24bbde08decabe8e69a96d6da307735c3a7c3f2222ce0018d2a0198154d8a73`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fef33880f1c4d184ecadc4e74fec55a0f527ba6aac781f3e829b558592b9d6a`  
		Last Modified: Tue, 17 Nov 2020 22:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
