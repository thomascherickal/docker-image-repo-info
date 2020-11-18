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
