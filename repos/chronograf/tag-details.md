<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.10`](#chronograf110)
-	[`chronograf:1.10-alpine`](#chronograf110-alpine)
-	[`chronograf:1.10.1`](#chronograf1101)
-	[`chronograf:1.10.1-alpine`](#chronograf1101-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:1.8.10`](#chronograf1810)
-	[`chronograf:1.8.10-alpine`](#chronograf1810-alpine)
-	[`chronograf:1.9`](#chronograf19)
-	[`chronograf:1.9-alpine`](#chronograf19-alpine)
-	[`chronograf:1.9.4`](#chronograf194)
-	[`chronograf:1.9.4-alpine`](#chronograf194-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.10`

```console
$ docker pull chronograf@sha256:17fbcca51ffab90339d6159af4e49f02876dbcf764d8a490609bc24efacadc6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:dd3e274c70d1e918d7557a5a22bc263f9520955e9cafbd2e6e406e842aa81e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82813614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dcffc85b1020b6c1349e8b0d85e42504a37d00f7a47189283e6faca134b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:45 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 21:40:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86698d89d6c3dde0460cdb05177c837c89fb32c0bb80ff6b841b818c184ce61`  
		Last Modified: Wed, 11 Oct 2023 21:41:58 GMT  
		Size: 46.1 MB (46142829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab43b91776800fa352500eda229e6b786a23d001ff3fbf26a76fcc72ebd6143`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7fc16fd35f70d4a5bd24d31a620cfc14bb8d54818676a025e8906eb1cdb057`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4b880b9b33aeeecdc6875caa8802679f7b16c998298031d92c7f5c4260dd10`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:461e52b9a754b47bf7423f5da79f85ed8d895d260ff598d5360aee448b4a0a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74948076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32762b89fcd01dc9ea5e327fd5f52aef474186557c319888ce70065e6cec46ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:32 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 18:19:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:42 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:42 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e03b1faee778a4bd70f37e75c2fbeec637f5d6e639512b5bcb3c531e678db0`  
		Last Modified: Wed, 11 Oct 2023 18:20:51 GMT  
		Size: 43.9 MB (43851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2dd9421ed768dd2da50dadee4f34805cfd1fe9406e5ade502e9f240d0330ee`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1f392246c4168d72ea94c6e02aa5e271b7ca97b2bf6a756213105872d701dc`  
		Last Modified: Wed, 11 Oct 2023 18:20:42 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52df86b9601d2fb3ba46a6c7139bb5808332b8eb4e3e5ce28a31ec1fd85d5d0f`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9bb0443c77efdcb1c1fb5f2232117b4fbad7fb708779459820c2c62be7f1f2b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79156374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2dedae1902d8d47d6c06105acf40fc49e9194e3705c02adeffa9dc5a48ba1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 19:59:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f0f1b8216870ec4fc89ea90b2d5842eb84769dbba516acbe398af3d7b5c469`  
		Last Modified: Wed, 11 Oct 2023 20:00:57 GMT  
		Size: 43.9 MB (43857074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c31842fe067310fe37b74a4fe28b1f8a8d9eea8389d1f7857116578c293fe4`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a049891bb7d4ac39a241baccdd9aed47a3ebf939187dcd9b2191cd0ffb96e41`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc1099f9669e66d9357f64008a0489a072a72a8b1e6893c443992530ccb1d16`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10-alpine`

```console
$ docker pull chronograf@sha256:295a5326cfe15ce099810d75e7e5783b14714901e075aefad634509771aa0a44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:bf8dcd958a130af2edac25ec90a1f6cc3171c755cf4b71ee58bf4ba2b3f7a8f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31475375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102b6042d5b4368888ad4486202556ca79b95d4e264498f1d23aa7258596fd06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:31:14 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Mon, 07 Aug 2023 20:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:31:19 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:31:19 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:31:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:31:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0716291e97dd3aa9b4ac1e505f495e39980163e703e70b7b3879a5300c9ca61`  
		Last Modified: Mon, 07 Aug 2023 20:32:24 GMT  
		Size: 27.8 MB (27787164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b966dde18c834e300e92baee365b79921f6533d96965a14c81a571d2e2fbf8`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 12.3 KB (12261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d98ce7134d836d5477458e108616a2cf46af05b192c50a53572ffb050be98`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578856a072c164ed8ec025c2e31ea1756d1109b02b8a38c11b74fb67040848b8`  
		Last Modified: Mon, 07 Aug 2023 20:32:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1`

```console
$ docker pull chronograf@sha256:17fbcca51ffab90339d6159af4e49f02876dbcf764d8a490609bc24efacadc6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.1` - linux; amd64

```console
$ docker pull chronograf@sha256:dd3e274c70d1e918d7557a5a22bc263f9520955e9cafbd2e6e406e842aa81e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82813614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dcffc85b1020b6c1349e8b0d85e42504a37d00f7a47189283e6faca134b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:45 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 21:40:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86698d89d6c3dde0460cdb05177c837c89fb32c0bb80ff6b841b818c184ce61`  
		Last Modified: Wed, 11 Oct 2023 21:41:58 GMT  
		Size: 46.1 MB (46142829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab43b91776800fa352500eda229e6b786a23d001ff3fbf26a76fcc72ebd6143`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7fc16fd35f70d4a5bd24d31a620cfc14bb8d54818676a025e8906eb1cdb057`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4b880b9b33aeeecdc6875caa8802679f7b16c998298031d92c7f5c4260dd10`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:461e52b9a754b47bf7423f5da79f85ed8d895d260ff598d5360aee448b4a0a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74948076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32762b89fcd01dc9ea5e327fd5f52aef474186557c319888ce70065e6cec46ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:32 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 18:19:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:42 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:42 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e03b1faee778a4bd70f37e75c2fbeec637f5d6e639512b5bcb3c531e678db0`  
		Last Modified: Wed, 11 Oct 2023 18:20:51 GMT  
		Size: 43.9 MB (43851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2dd9421ed768dd2da50dadee4f34805cfd1fe9406e5ade502e9f240d0330ee`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1f392246c4168d72ea94c6e02aa5e271b7ca97b2bf6a756213105872d701dc`  
		Last Modified: Wed, 11 Oct 2023 18:20:42 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52df86b9601d2fb3ba46a6c7139bb5808332b8eb4e3e5ce28a31ec1fd85d5d0f`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9bb0443c77efdcb1c1fb5f2232117b4fbad7fb708779459820c2c62be7f1f2b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79156374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2dedae1902d8d47d6c06105acf40fc49e9194e3705c02adeffa9dc5a48ba1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 19:59:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f0f1b8216870ec4fc89ea90b2d5842eb84769dbba516acbe398af3d7b5c469`  
		Last Modified: Wed, 11 Oct 2023 20:00:57 GMT  
		Size: 43.9 MB (43857074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c31842fe067310fe37b74a4fe28b1f8a8d9eea8389d1f7857116578c293fe4`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a049891bb7d4ac39a241baccdd9aed47a3ebf939187dcd9b2191cd0ffb96e41`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc1099f9669e66d9357f64008a0489a072a72a8b1e6893c443992530ccb1d16`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1-alpine`

```console
$ docker pull chronograf@sha256:295a5326cfe15ce099810d75e7e5783b14714901e075aefad634509771aa0a44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10.1-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:bf8dcd958a130af2edac25ec90a1f6cc3171c755cf4b71ee58bf4ba2b3f7a8f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31475375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102b6042d5b4368888ad4486202556ca79b95d4e264498f1d23aa7258596fd06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:31:14 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Mon, 07 Aug 2023 20:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:31:19 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:31:19 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:31:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:31:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0716291e97dd3aa9b4ac1e505f495e39980163e703e70b7b3879a5300c9ca61`  
		Last Modified: Mon, 07 Aug 2023 20:32:24 GMT  
		Size: 27.8 MB (27787164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b966dde18c834e300e92baee365b79921f6533d96965a14c81a571d2e2fbf8`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 12.3 KB (12261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d98ce7134d836d5477458e108616a2cf46af05b192c50a53572ffb050be98`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578856a072c164ed8ec025c2e31ea1756d1109b02b8a38c11b74fb67040848b8`  
		Last Modified: Mon, 07 Aug 2023 20:32:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:c921382cbbab41d4c958c6940de65563810abb6492dc8ba6a4ee0b1e9dd6f018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:6e4abb3a177be569efd588ff739141d01b30d9d394534ef757abfa382d966e6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70598963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f97fef9c84de67d2db7edcbc55164ae2d22d1382a185e3dc87547bdc85a99e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:39:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:39:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 21:40:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:02 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde01f900f890669249c3c1a50f5395d18304eff777733d7ef1b4c67726bfbc`  
		Last Modified: Wed, 11 Oct 2023 21:41:11 GMT  
		Size: 4.4 MB (4417383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc28bafc26298bbf0f4e8e39bc8ca93decd2da5290117fa25dc86f3da295c6b7`  
		Last Modified: Wed, 11 Oct 2023 21:41:15 GMT  
		Size: 34.7 MB (34739328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7fcf5d9b5a950c23004b1a446bb6c8d5140e7be69da47b1fb4ca968f73afe1`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3b4ac9f8564515e87b438d4b0c0be5910f0ac430f82d20173765d6facbe91`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c69e8b57467c099a6fde95fb25ebe17638c1d68b392b1275800c71e1fd3e99`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e278faaa6a70c4414503d4d935a84bc4611e69121ded1d5a8e3c513ff801bd4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63422665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829d42ad58a614d78757b478590d61c59e93b97ac394614cbac0be10f76f380a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:18:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:18:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 18:18:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:18:57 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:18:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:18:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:18:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b1d927d01dca9cb7a6bb783e36cace9cd8f5bac3a65d1d93af6336082169f7`  
		Last Modified: Wed, 11 Oct 2023 18:19:57 GMT  
		Size: 3.7 MB (3719890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142e5bafbc8ece06dd411e0e2a88e4834e87ccce2bab85d84c5dcbf82956d7f5`  
		Last Modified: Wed, 11 Oct 2023 18:20:01 GMT  
		Size: 33.1 MB (33099374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f1e379f64d26dc3fc57a3d0e40480d27394af49ebac6cdc4beb6106f037ea4`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15091ab8f90eb6742de83da9442de1e61204bd02311957e8200ac1178061bd8f`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c8762af1ea37ebdac079efb34864bf01333da66a264907b5fe0dd907454fdb`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:389c74876512f03e023854e70553230c444008af1738a1fee36896c64b90f9be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91d89d56aaf500c64614c43342c9c3f3c89e577ed2386551996558f15caf000`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:05 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 19:59:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:13 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:13 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5726819688860c7f93aa6f1d45e20cdb98e56e717eccc9c74e4a8602ed8929`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 4.4 MB (4418969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bd84476afe6fd96dc7cd71031753d7892ea0ce78f7c9e3605d3cb16a62760f`  
		Last Modified: Wed, 11 Oct 2023 20:00:17 GMT  
		Size: 33.2 MB (33239692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0d1452407272a49f6bf371b7a2c936fa5dffd31d98de67ff621b97dd4a26e`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018a72239f48ec52a2faad1f6559f359763e46bfc6f2728bb37185f81cf24009`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d515cfa9cd89177129fb9538629a3b9a9f0aec0bcaecc5be1f34bd56dcfcf21`  
		Last Modified: Wed, 11 Oct 2023 20:00:09 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:8ec288d479d956964cf2b38c0d1097482155b7e59f03bf9aa520da4021537e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f42d647b759e8598c7026b23e0e716e40db12f047c2bd098f8f8e3d6e3d75c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23245400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ef4a9983e4104a0a81502341beb8408b00c6d95630b535907907f1924f7a7f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:30:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Mon, 07 Aug 2023 20:30:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:30:47 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:30:47 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:30:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9e0598146a04dd875c5c8bfd4fe65a6d787b5e7aa7eddd44d8b045688b51ea`  
		Last Modified: Mon, 07 Aug 2023 20:31:41 GMT  
		Size: 19.6 MB (19557185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f4683669de6527191a8edbd84f3ad92e3077b18991ccc9cdff51a926b9a77d`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20905209fe10e56722ee9a48ac5d6dab2f3a2b257f2a93433737c3caacafc08`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452d0b7e35169d35ff46f375d21430f2a3d707d684583398166b4f9d14ed215`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:c921382cbbab41d4c958c6940de65563810abb6492dc8ba6a4ee0b1e9dd6f018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:6e4abb3a177be569efd588ff739141d01b30d9d394534ef757abfa382d966e6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70598963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f97fef9c84de67d2db7edcbc55164ae2d22d1382a185e3dc87547bdc85a99e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:39:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:39:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 21:40:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:02 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde01f900f890669249c3c1a50f5395d18304eff777733d7ef1b4c67726bfbc`  
		Last Modified: Wed, 11 Oct 2023 21:41:11 GMT  
		Size: 4.4 MB (4417383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc28bafc26298bbf0f4e8e39bc8ca93decd2da5290117fa25dc86f3da295c6b7`  
		Last Modified: Wed, 11 Oct 2023 21:41:15 GMT  
		Size: 34.7 MB (34739328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7fcf5d9b5a950c23004b1a446bb6c8d5140e7be69da47b1fb4ca968f73afe1`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3b4ac9f8564515e87b438d4b0c0be5910f0ac430f82d20173765d6facbe91`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c69e8b57467c099a6fde95fb25ebe17638c1d68b392b1275800c71e1fd3e99`  
		Last Modified: Wed, 11 Oct 2023 21:41:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e278faaa6a70c4414503d4d935a84bc4611e69121ded1d5a8e3c513ff801bd4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63422665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829d42ad58a614d78757b478590d61c59e93b97ac394614cbac0be10f76f380a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:18:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:18:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 18:18:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:18:57 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:18:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:18:57 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:18:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:18:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b1d927d01dca9cb7a6bb783e36cace9cd8f5bac3a65d1d93af6336082169f7`  
		Last Modified: Wed, 11 Oct 2023 18:19:57 GMT  
		Size: 3.7 MB (3719890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142e5bafbc8ece06dd411e0e2a88e4834e87ccce2bab85d84c5dcbf82956d7f5`  
		Last Modified: Wed, 11 Oct 2023 18:20:01 GMT  
		Size: 33.1 MB (33099374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f1e379f64d26dc3fc57a3d0e40480d27394af49ebac6cdc4beb6106f037ea4`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15091ab8f90eb6742de83da9442de1e61204bd02311957e8200ac1178061bd8f`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c8762af1ea37ebdac079efb34864bf01333da66a264907b5fe0dd907454fdb`  
		Last Modified: Wed, 11 Oct 2023 18:19:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:389c74876512f03e023854e70553230c444008af1738a1fee36896c64b90f9be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91d89d56aaf500c64614c43342c9c3f3c89e577ed2386551996558f15caf000`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:05 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 11 Oct 2023 19:59:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:13 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:13 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5726819688860c7f93aa6f1d45e20cdb98e56e717eccc9c74e4a8602ed8929`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 4.4 MB (4418969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bd84476afe6fd96dc7cd71031753d7892ea0ce78f7c9e3605d3cb16a62760f`  
		Last Modified: Wed, 11 Oct 2023 20:00:17 GMT  
		Size: 33.2 MB (33239692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0d1452407272a49f6bf371b7a2c936fa5dffd31d98de67ff621b97dd4a26e`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018a72239f48ec52a2faad1f6559f359763e46bfc6f2728bb37185f81cf24009`  
		Last Modified: Wed, 11 Oct 2023 20:00:10 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d515cfa9cd89177129fb9538629a3b9a9f0aec0bcaecc5be1f34bd56dcfcf21`  
		Last Modified: Wed, 11 Oct 2023 20:00:09 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:8ec288d479d956964cf2b38c0d1097482155b7e59f03bf9aa520da4021537e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f42d647b759e8598c7026b23e0e716e40db12f047c2bd098f8f8e3d6e3d75c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23245400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ef4a9983e4104a0a81502341beb8408b00c6d95630b535907907f1924f7a7f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:30:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Mon, 07 Aug 2023 20:30:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:30:47 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:30:47 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:30:47 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:30:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9e0598146a04dd875c5c8bfd4fe65a6d787b5e7aa7eddd44d8b045688b51ea`  
		Last Modified: Mon, 07 Aug 2023 20:31:41 GMT  
		Size: 19.6 MB (19557185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f4683669de6527191a8edbd84f3ad92e3077b18991ccc9cdff51a926b9a77d`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20905209fe10e56722ee9a48ac5d6dab2f3a2b257f2a93433737c3caacafc08`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452d0b7e35169d35ff46f375d21430f2a3d707d684583398166b4f9d14ed215`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:94b9e110f0c14930db4527c41698109e84b5a565d5d3d1bab503bb23ff79db3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:bb7bcd13b3084a82d339d9ec2f73aaa17d0782cc16cf03220940817ecc78a44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71250941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e8711cc9a22b9881913d73f91750cba97c012a2687bcaf4196a3a63300b431f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:17 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 21:40:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:24 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:25 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93fc40bb2b1386409c2c3f485d878bce6cacbd60ec3df4688a4610ea4e31ff5`  
		Last Modified: Wed, 11 Oct 2023 21:41:28 GMT  
		Size: 34.6 MB (34580162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56d1bcc7e853acede482f10b8516f4451d3b1f85557c85ce20ab563a6457611`  
		Last Modified: Wed, 11 Oct 2023 21:41:23 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e27e248e464ba1dbdc435eabdd4edf0eef70aa5f27a1a6073e1ae731d18bdba`  
		Last Modified: Wed, 11 Oct 2023 21:41:24 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52d5c112f57139536bccadc3e9ae1e7b32668464b666e7eb31a50916ac3581a`  
		Last Modified: Wed, 11 Oct 2023 21:41:23 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:6db29f45c067626c3aed58d554882530fb5a3a00985c4056c4b874065ebc83d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63848525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd537b51729c9005991ebee879bfc36732d22a4490c5c1444693dc77d41d4c6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:08 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 18:19:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:16 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:16 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:17 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:17 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:17 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5f0e0be44fbc850734570b2d88fe881e3589617158faca0bf71d464d093286`  
		Last Modified: Wed, 11 Oct 2023 18:20:17 GMT  
		Size: 32.8 MB (32751558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63722eb8a739fa7459961de7f42b57977a0305867f5a4ac70b4ae2f7bd93343`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0c8af953b49ffddfed5b3133b59b99d7b8f4056232ee54742904508d4e8559`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598707cc254ec589a73e90d88c1b5da72e089626006cb16d4e4937f835ed5be9`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f0364c6d62a4eac81bf44d534a97ae90e6d4b862f71826ba2e3cfd9931f6a1bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67945046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8f34dbe5238b09af2b6d13fe96e4e735fb776295a9861889622f2379a076ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:25 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 19:59:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:31 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b87e56e22fae62a6f2d2e05772db53d0d4130764402cdfe4e10345bb94a788d`  
		Last Modified: Wed, 11 Oct 2023 20:00:30 GMT  
		Size: 32.6 MB (32645734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dedde53c034f276e80b746ff544cef9646146d9eda03355f3cc87e55a0b73b`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17c12000dee3c58684aad96a5e4b2d9a907f83dbf549bfd817a1bae05b2cf5`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8896a9bc0eea2fc1ee7bf39f1fe081d035f5e918780e6a2e04c262504b0ceb00`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:4771617f8fa2c2296e27512171386253c776bb1d8bf3702d2965825713d628b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2576064ee1f09de3f9e3b687a17733ef4662eb8da7197da6009c2ae42a8199b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22892402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84eb60f6ddc8c149a5eebfa12d2a90eb09b938314a28b3febd39a7dc96301311`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:30:53 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Mon, 07 Aug 2023 20:30:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:30:58 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:30:58 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:30:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:30:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a1130cb457feb5a433f526878959d2d8c95442694cc23263d04197b7dc3aac`  
		Last Modified: Mon, 07 Aug 2023 20:31:58 GMT  
		Size: 19.2 MB (19204185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bf18326d4c54af0954288f539ea2816a9a8955d007458ba9f0af65be63ab7d`  
		Last Modified: Mon, 07 Aug 2023 20:31:54 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75844cd43ff01471a619bb96232b117f34abcca16bdfe8771fb20792aff560d`  
		Last Modified: Mon, 07 Aug 2023 20:31:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49790f26ba7324b957d118bc6026e4ffb2e3d8ca2fd7a61462a9d19409d2f3a`  
		Last Modified: Mon, 07 Aug 2023 20:31:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:94b9e110f0c14930db4527c41698109e84b5a565d5d3d1bab503bb23ff79db3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:bb7bcd13b3084a82d339d9ec2f73aaa17d0782cc16cf03220940817ecc78a44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71250941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e8711cc9a22b9881913d73f91750cba97c012a2687bcaf4196a3a63300b431f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:17 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 21:40:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:24 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:25 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93fc40bb2b1386409c2c3f485d878bce6cacbd60ec3df4688a4610ea4e31ff5`  
		Last Modified: Wed, 11 Oct 2023 21:41:28 GMT  
		Size: 34.6 MB (34580162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56d1bcc7e853acede482f10b8516f4451d3b1f85557c85ce20ab563a6457611`  
		Last Modified: Wed, 11 Oct 2023 21:41:23 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e27e248e464ba1dbdc435eabdd4edf0eef70aa5f27a1a6073e1ae731d18bdba`  
		Last Modified: Wed, 11 Oct 2023 21:41:24 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52d5c112f57139536bccadc3e9ae1e7b32668464b666e7eb31a50916ac3581a`  
		Last Modified: Wed, 11 Oct 2023 21:41:23 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:6db29f45c067626c3aed58d554882530fb5a3a00985c4056c4b874065ebc83d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63848525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd537b51729c9005991ebee879bfc36732d22a4490c5c1444693dc77d41d4c6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:08 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 18:19:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:16 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:16 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:17 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:17 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:17 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5f0e0be44fbc850734570b2d88fe881e3589617158faca0bf71d464d093286`  
		Last Modified: Wed, 11 Oct 2023 18:20:17 GMT  
		Size: 32.8 MB (32751558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63722eb8a739fa7459961de7f42b57977a0305867f5a4ac70b4ae2f7bd93343`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0c8af953b49ffddfed5b3133b59b99d7b8f4056232ee54742904508d4e8559`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598707cc254ec589a73e90d88c1b5da72e089626006cb16d4e4937f835ed5be9`  
		Last Modified: Wed, 11 Oct 2023 18:20:11 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f0364c6d62a4eac81bf44d534a97ae90e6d4b862f71826ba2e3cfd9931f6a1bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67945046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8f34dbe5238b09af2b6d13fe96e4e735fb776295a9861889622f2379a076ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:25 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 11 Oct 2023 19:59:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:31 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b87e56e22fae62a6f2d2e05772db53d0d4130764402cdfe4e10345bb94a788d`  
		Last Modified: Wed, 11 Oct 2023 20:00:30 GMT  
		Size: 32.6 MB (32645734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dedde53c034f276e80b746ff544cef9646146d9eda03355f3cc87e55a0b73b`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17c12000dee3c58684aad96a5e4b2d9a907f83dbf549bfd817a1bae05b2cf5`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8896a9bc0eea2fc1ee7bf39f1fe081d035f5e918780e6a2e04c262504b0ceb00`  
		Last Modified: Wed, 11 Oct 2023 20:00:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:4771617f8fa2c2296e27512171386253c776bb1d8bf3702d2965825713d628b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2576064ee1f09de3f9e3b687a17733ef4662eb8da7197da6009c2ae42a8199b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22892402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84eb60f6ddc8c149a5eebfa12d2a90eb09b938314a28b3febd39a7dc96301311`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:30:53 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Mon, 07 Aug 2023 20:30:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:30:58 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:30:58 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:30:58 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:30:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:30:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a1130cb457feb5a433f526878959d2d8c95442694cc23263d04197b7dc3aac`  
		Last Modified: Mon, 07 Aug 2023 20:31:58 GMT  
		Size: 19.2 MB (19204185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bf18326d4c54af0954288f539ea2816a9a8955d007458ba9f0af65be63ab7d`  
		Last Modified: Mon, 07 Aug 2023 20:31:54 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75844cd43ff01471a619bb96232b117f34abcca16bdfe8771fb20792aff560d`  
		Last Modified: Mon, 07 Aug 2023 20:31:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49790f26ba7324b957d118bc6026e4ffb2e3d8ca2fd7a61462a9d19409d2f3a`  
		Last Modified: Mon, 07 Aug 2023 20:31:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:c7326a11e1baaa633f78fc3e494f6cb3d9a2d3d7ad8e589e5e7651ed7af5551b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:67a81f96eb95d4b842aa10b6a02e8323c49c0b0ab8b1a1d434f7bba258a43beb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71898580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afe7c9a215e7b904f7a5b78f3c4c887f816da8783e056a8a0d771bbe2fc619e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:32 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 21:40:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:40 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:40 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869696b91542152d40ee5c463b1c25ef9a7c713ef36a6c58bac22289bb24449b`  
		Last Modified: Wed, 11 Oct 2023 21:41:42 GMT  
		Size: 35.2 MB (35227803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187324a23854e688547b57db7db7206e222f34eaa76d803f18ec317f7facb1`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cefdd12c511b8d2d007e8a6e2db9a7c48f2b6c62936c1012564eda55c5fdc9`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b247d4a4398117d70a5677fe87283584608b64d17ba083b139dedf14767d11c2`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b53660fe1af5575ccecc242cdccee2faddf4ceae58cbf3dcb1bffc88911661e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64624643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa8ed8137a424e633ab2bf4dc99963f79893c8996bb7617060e7a79bbc70fa2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:21 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 18:19:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:29 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db89586125167b6f56f20b3a3586f9b109f66056caa6a96fd52348b2567cb3`  
		Last Modified: Wed, 11 Oct 2023 18:20:33 GMT  
		Size: 33.5 MB (33527682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4892e757f21d30309834fc54d0702acfe82e7aa79959d2089e88aa1f6e8f0f`  
		Last Modified: Wed, 11 Oct 2023 18:20:29 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa84064bbf2ccabc0739bbbe5f0cfeec5003a1e9c8e7b02490413c1909e9303`  
		Last Modified: Wed, 11 Oct 2023 18:20:28 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81a941aaadab250a92e70202471310fa150e9c3c428261213c0fdaeff2d29e0`  
		Last Modified: Wed, 11 Oct 2023 18:20:28 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:60022e10803e59c6c11c7aa7b5cc3434e63ef4feb6a3a3c4b82f9ee20ded4729
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68697413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d171ec2d92df7dc01689b48d5d241ee1e465d6a38ec89b37a13da8b605ba42a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:35 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 19:59:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:41 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:41 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8c09a18736d758e13723a9a6dd284dde367a888feaff1ddb381446e216e1`  
		Last Modified: Wed, 11 Oct 2023 20:00:43 GMT  
		Size: 33.4 MB (33398100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3473bfae7a2ab8e066ddb29d80f31c1d600ddb6f6abf38d3d37b45f9696460ba`  
		Last Modified: Wed, 11 Oct 2023 20:00:40 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89e22b9d4377cc3ee2878d8b1169c4401bf4bbaa39a28db6783eec95801721d`  
		Last Modified: Wed, 11 Oct 2023 20:00:39 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366b3e065f656cb4699d68fbb0ce7f675180ecd8be57a02a835647a5dc2a5190`  
		Last Modified: Wed, 11 Oct 2023 20:00:39 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:472d6631290df88eaa1b6eb34895c371e7948ef084c8151839b620a567612554
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:01f7f883eb77379b13b4d9e5d320a1ae0000d5026ac5d1b89b0d473d5b0f7552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23360370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1e7b4a78b4f81521acee66aab3a7c5efe4e38d0d129ad85a0ba4f79caba979`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:31:04 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Mon, 07 Aug 2023 20:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:31:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:31:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:31:08 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:31:08 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:31:09 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:31:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:31:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c216188631b318e1e2418de78df00f1f51089ba19ab2cf7e7a7c3ddc0e84b9`  
		Last Modified: Mon, 07 Aug 2023 20:32:11 GMT  
		Size: 19.7 MB (19672159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad8ee8024c011a7df9ebc5ad3cdb576eebfa52cd3d71d88dbeb778f32c7e475`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc679ad9a33c55210071b2f8ba46edf0faad22af48a591805882789a0199f5b`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b754b80d1168f3bcd58f914e6724e0a1f4b525005c87e788fa8419b9582ad58`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:c7326a11e1baaa633f78fc3e494f6cb3d9a2d3d7ad8e589e5e7651ed7af5551b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:67a81f96eb95d4b842aa10b6a02e8323c49c0b0ab8b1a1d434f7bba258a43beb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71898580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afe7c9a215e7b904f7a5b78f3c4c887f816da8783e056a8a0d771bbe2fc619e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:32 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 21:40:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:40 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:40 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:40 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869696b91542152d40ee5c463b1c25ef9a7c713ef36a6c58bac22289bb24449b`  
		Last Modified: Wed, 11 Oct 2023 21:41:42 GMT  
		Size: 35.2 MB (35227803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187324a23854e688547b57db7db7206e222f34eaa76d803f18ec317f7facb1`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cefdd12c511b8d2d007e8a6e2db9a7c48f2b6c62936c1012564eda55c5fdc9`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b247d4a4398117d70a5677fe87283584608b64d17ba083b139dedf14767d11c2`  
		Last Modified: Wed, 11 Oct 2023 21:41:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b53660fe1af5575ccecc242cdccee2faddf4ceae58cbf3dcb1bffc88911661e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64624643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa8ed8137a424e633ab2bf4dc99963f79893c8996bb7617060e7a79bbc70fa2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:21 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 18:19:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:29 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db89586125167b6f56f20b3a3586f9b109f66056caa6a96fd52348b2567cb3`  
		Last Modified: Wed, 11 Oct 2023 18:20:33 GMT  
		Size: 33.5 MB (33527682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4892e757f21d30309834fc54d0702acfe82e7aa79959d2089e88aa1f6e8f0f`  
		Last Modified: Wed, 11 Oct 2023 18:20:29 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa84064bbf2ccabc0739bbbe5f0cfeec5003a1e9c8e7b02490413c1909e9303`  
		Last Modified: Wed, 11 Oct 2023 18:20:28 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81a941aaadab250a92e70202471310fa150e9c3c428261213c0fdaeff2d29e0`  
		Last Modified: Wed, 11 Oct 2023 18:20:28 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:60022e10803e59c6c11c7aa7b5cc3434e63ef4feb6a3a3c4b82f9ee20ded4729
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68697413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d171ec2d92df7dc01689b48d5d241ee1e465d6a38ec89b37a13da8b605ba42a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:35 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 11 Oct 2023 19:59:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:41 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:41 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8c09a18736d758e13723a9a6dd284dde367a888feaff1ddb381446e216e1`  
		Last Modified: Wed, 11 Oct 2023 20:00:43 GMT  
		Size: 33.4 MB (33398100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3473bfae7a2ab8e066ddb29d80f31c1d600ddb6f6abf38d3d37b45f9696460ba`  
		Last Modified: Wed, 11 Oct 2023 20:00:40 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89e22b9d4377cc3ee2878d8b1169c4401bf4bbaa39a28db6783eec95801721d`  
		Last Modified: Wed, 11 Oct 2023 20:00:39 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366b3e065f656cb4699d68fbb0ce7f675180ecd8be57a02a835647a5dc2a5190`  
		Last Modified: Wed, 11 Oct 2023 20:00:39 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:472d6631290df88eaa1b6eb34895c371e7948ef084c8151839b620a567612554
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:01f7f883eb77379b13b4d9e5d320a1ae0000d5026ac5d1b89b0d473d5b0f7552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23360370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1e7b4a78b4f81521acee66aab3a7c5efe4e38d0d129ad85a0ba4f79caba979`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:31:04 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Mon, 07 Aug 2023 20:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:31:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:31:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:31:08 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:31:08 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:31:09 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:31:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:31:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c216188631b318e1e2418de78df00f1f51089ba19ab2cf7e7a7c3ddc0e84b9`  
		Last Modified: Mon, 07 Aug 2023 20:32:11 GMT  
		Size: 19.7 MB (19672159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad8ee8024c011a7df9ebc5ad3cdb576eebfa52cd3d71d88dbeb778f32c7e475`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc679ad9a33c55210071b2f8ba46edf0faad22af48a591805882789a0199f5b`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b754b80d1168f3bcd58f914e6724e0a1f4b525005c87e788fa8419b9582ad58`  
		Last Modified: Mon, 07 Aug 2023 20:32:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:295a5326cfe15ce099810d75e7e5783b14714901e075aefad634509771aa0a44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:bf8dcd958a130af2edac25ec90a1f6cc3171c755cf4b71ee58bf4ba2b3f7a8f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31475375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102b6042d5b4368888ad4486202556ca79b95d4e264498f1d23aa7258596fd06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:30:42 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Aug 2023 20:31:14 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Mon, 07 Aug 2023 20:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Aug 2023 20:31:19 GMT
EXPOSE 8888
# Mon, 07 Aug 2023 20:31:19 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Aug 2023 20:31:19 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:31:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:31:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90abcbb30a629c57e0b08df7b8082f6e402abc4cf708c553237cb0424fa9c4`  
		Last Modified: Mon, 07 Aug 2023 20:31:37 GMT  
		Size: 284.9 KB (284927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0716291e97dd3aa9b4ac1e505f495e39980163e703e70b7b3879a5300c9ca61`  
		Last Modified: Mon, 07 Aug 2023 20:32:24 GMT  
		Size: 27.8 MB (27787164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b966dde18c834e300e92baee365b79921f6533d96965a14c81a571d2e2fbf8`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 12.3 KB (12261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d98ce7134d836d5477458e108616a2cf46af05b192c50a53572ffb050be98`  
		Last Modified: Mon, 07 Aug 2023 20:32:19 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578856a072c164ed8ec025c2e31ea1756d1109b02b8a38c11b74fb67040848b8`  
		Last Modified: Mon, 07 Aug 2023 20:32:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:17fbcca51ffab90339d6159af4e49f02876dbcf764d8a490609bc24efacadc6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:dd3e274c70d1e918d7557a5a22bc263f9520955e9cafbd2e6e406e842aa81e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82813614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dcffc85b1020b6c1349e8b0d85e42504a37d00f7a47189283e6faca134b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 21:40:45 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 21:40:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 21:40:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 21:40:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 21:40:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 21:40:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 21:40:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd152c4c221fe5100d71352016a9d1f0c9dcd0612280c0c5d47c1d02548291e`  
		Last Modified: Wed, 11 Oct 2023 21:41:25 GMT  
		Size: 5.2 MB (5228528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86698d89d6c3dde0460cdb05177c837c89fb32c0bb80ff6b841b818c184ce61`  
		Last Modified: Wed, 11 Oct 2023 21:41:58 GMT  
		Size: 46.1 MB (46142829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab43b91776800fa352500eda229e6b786a23d001ff3fbf26a76fcc72ebd6143`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7fc16fd35f70d4a5bd24d31a620cfc14bb8d54818676a025e8906eb1cdb057`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4b880b9b33aeeecdc6875caa8802679f7b16c998298031d92c7f5c4260dd10`  
		Last Modified: Wed, 11 Oct 2023 21:41:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:461e52b9a754b47bf7423f5da79f85ed8d895d260ff598d5360aee448b4a0a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74948076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32762b89fcd01dc9ea5e327fd5f52aef474186557c319888ce70065e6cec46ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 18:19:32 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 18:19:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 18:19:42 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 18:19:42 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 18:19:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 18:19:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9796c0695f7c556cf6e46458a58316bc4e6ffab4671c0fa4471842995e378a`  
		Last Modified: Wed, 11 Oct 2023 18:20:12 GMT  
		Size: 4.5 MB (4493561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e03b1faee778a4bd70f37e75c2fbeec637f5d6e639512b5bcb3c531e678db0`  
		Last Modified: Wed, 11 Oct 2023 18:20:51 GMT  
		Size: 43.9 MB (43851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2dd9421ed768dd2da50dadee4f34805cfd1fe9406e5ade502e9f240d0330ee`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1f392246c4168d72ea94c6e02aa5e271b7ca97b2bf6a756213105872d701dc`  
		Last Modified: Wed, 11 Oct 2023 18:20:42 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52df86b9601d2fb3ba46a6c7139bb5808332b8eb4e3e5ce28a31ec1fd85d5d0f`  
		Last Modified: Wed, 11 Oct 2023 18:20:43 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9bb0443c77efdcb1c1fb5f2232117b4fbad7fb708779459820c2c62be7f1f2b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79156374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2dedae1902d8d47d6c06105acf40fc49e9194e3705c02adeffa9dc5a48ba1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:59:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 Oct 2023 19:59:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 11 Oct 2023 19:59:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 11 Oct 2023 19:59:52 GMT
EXPOSE 8888
# Wed, 11 Oct 2023 19:59:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 11 Oct 2023 19:59:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 11 Oct 2023 19:59:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 19:59:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4fe693d9f3cceb1c1b06884788e739020d0f333835b047254ec0b586f9f24`  
		Last Modified: Wed, 11 Oct 2023 20:00:27 GMT  
		Size: 5.2 MB (5210827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f0f1b8216870ec4fc89ea90b2d5842eb84769dbba516acbe398af3d7b5c469`  
		Last Modified: Wed, 11 Oct 2023 20:00:57 GMT  
		Size: 43.9 MB (43857074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c31842fe067310fe37b74a4fe28b1f8a8d9eea8389d1f7857116578c293fe4`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a049891bb7d4ac39a241baccdd9aed47a3ebf939187dcd9b2191cd0ffb96e41`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc1099f9669e66d9357f64008a0489a072a72a8b1e6893c443992530ccb1d16`  
		Last Modified: Wed, 11 Oct 2023 20:00:52 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
