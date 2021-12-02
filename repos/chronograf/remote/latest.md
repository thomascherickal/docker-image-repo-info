## `chronograf:latest`

```console
$ docker pull chronograf@sha256:75dadb7b039c8330e3d6fe6f122ad7887dc173ec300d803b43480dac4bd5f268
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:bfae11ebcaa2800e109ad78a1a88af5b50277ae3c0221128144cb3bbd5fc00c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66882260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e5397d827b44902881f17bf6a9ed6a1afbc2985ff5166a4fa3af80b35613bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:30 GMT
ADD file:8177796e1ceff490318ed6eb46346bef21c5bcf01b1b396567475a1333d77174 in / 
# Thu, 02 Dec 2021 02:50:30 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:55:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 02 Dec 2021 03:56:27 GMT
ENV CHRONOGRAF_VERSION=1.9.1
# Thu, 02 Dec 2021 03:56:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 03:56:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 02 Dec 2021 03:56:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 02 Dec 2021 03:56:39 GMT
EXPOSE 8888
# Thu, 02 Dec 2021 03:56:40 GMT
VOLUME [/var/lib/chronograf]
# Thu, 02 Dec 2021 03:56:40 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 02 Dec 2021 03:56:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Dec 2021 03:56:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b4f470726ddc3d7ee51215c25ddc9d02185d04304b081eb283cbeb217964b939`  
		Last Modified: Thu, 02 Dec 2021 02:57:41 GMT  
		Size: 22.5 MB (22529080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f7ac851948306ff0cad2418221cb3d1b3db35a10c8d199e71d24da55c907a6`  
		Last Modified: Thu, 02 Dec 2021 03:57:15 GMT  
		Size: 6.8 MB (6760339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5ed1ec307de799c2029d41d8bacb529e10d73479eca5a9dca1a3fd3da18162`  
		Last Modified: Thu, 02 Dec 2021 03:58:09 GMT  
		Size: 37.6 MB (37568445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8fe35026ddf4aaad23ee8c405b9261a13c8a719fcf029de49bd8136385ada8`  
		Last Modified: Thu, 02 Dec 2021 03:58:03 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da80d378991097af18e84aba7c7faa9895e6576ee0d5e632c02968d8f818ab52`  
		Last Modified: Thu, 02 Dec 2021 03:58:03 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe4a8c5ba575ca7a33bb40b92586ea6b1faeea85fb763c811ec76c13d573d7`  
		Last Modified: Thu, 02 Dec 2021 03:58:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:520d3a3909ecf27f5bd76738c7ae3661378e80bdb276407ee8b0c86ecce365f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60400404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d24c71e37bcedb8afe7d03b17fe7cc1cb8473632ef5aac5b9c5945288c79f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 17 Nov 2021 02:05:31 GMT
ADD file:f28546ff6a3759d3a957c25d4310c3065e1367dff4ae304caae1cf1dc64d061d in / 
# Wed, 17 Nov 2021 02:05:32 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 10:09:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 10:11:26 GMT
ENV CHRONOGRAF_VERSION=1.9.1
# Thu, 18 Nov 2021 10:11:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 18 Nov 2021 10:11:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 18 Nov 2021 10:11:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 18 Nov 2021 10:11:47 GMT
EXPOSE 8888
# Thu, 18 Nov 2021 10:11:47 GMT
VOLUME [/var/lib/chronograf]
# Thu, 18 Nov 2021 10:11:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 18 Nov 2021 10:11:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 10:11:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:614e23553da11f1294dc969bcab416c9f981794bdbaee5641335a222730c63b2`  
		Last Modified: Wed, 17 Nov 2021 02:22:41 GMT  
		Size: 19.3 MB (19316397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc6970cd8a6794f987d0e1ad25e6b7939c3fae5fc7a07bd1663575e619fa7d1`  
		Last Modified: Thu, 18 Nov 2021 10:12:54 GMT  
		Size: 5.8 MB (5780548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff9dda975d6159188d2f407676bd8272c13717aac2a5ef206316905d703c167`  
		Last Modified: Thu, 18 Nov 2021 10:14:46 GMT  
		Size: 35.3 MB (35279067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b92df719c0958ade78e4af32da86f21bc0c5263682714a8a860a55d99a28584`  
		Last Modified: Thu, 18 Nov 2021 10:14:27 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3535a6d596ab8f15279796ac6ebe9743424a8695324fa404f096828f238077`  
		Last Modified: Thu, 18 Nov 2021 10:14:27 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbbf2041d51d6e1ea6451fc12e813ab7c9f871cdf24861ec2901142da1b9609`  
		Last Modified: Thu, 18 Nov 2021 10:14:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5bb5df3f78953956c726f924416d2334b1687c0308c6b5cec10f027d678aa62d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61623588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b2beef50d1860666391b725b2645fad75a362116a0244ce0f4e6e249f5557a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:48 GMT
ADD file:2adad5eee701d55a9f58c07f0706eb574d0ad6b74b0cc52a9e622f50639961c9 in / 
# Wed, 17 Nov 2021 02:42:48 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:09:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 03:10:33 GMT
ENV CHRONOGRAF_VERSION=1.9.1
# Wed, 17 Nov 2021 03:10:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 03:10:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 17 Nov 2021 03:10:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 17 Nov 2021 03:10:45 GMT
EXPOSE 8888
# Wed, 17 Nov 2021 03:10:46 GMT
VOLUME [/var/lib/chronograf]
# Wed, 17 Nov 2021 03:10:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 17 Nov 2021 03:10:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 03:10:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:34b92b588f0f390db0d125ab0ee4c85510c52367371c4bcf5af80a6ab18f0a9b`  
		Last Modified: Wed, 17 Nov 2021 02:51:38 GMT  
		Size: 20.4 MB (20389442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f831632bd5d7229d4f28100c7422a4a6f9c307486f2d34f3c228345f16c17763`  
		Last Modified: Wed, 17 Nov 2021 03:11:17 GMT  
		Size: 6.0 MB (6046825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9de71372b0298f8cb73e233c351a5b7a82d3652e0a94fcf9e07f25bc8903181`  
		Last Modified: Wed, 17 Nov 2021 03:12:08 GMT  
		Size: 35.2 MB (35162935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6523036e73c5ca508e28589fd9d15ff833fb2ed2546627da7407fd567430c`  
		Last Modified: Wed, 17 Nov 2021 03:12:03 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff93c2f1bff22e854375714715a163505a900b1cfff1dad118dd0b7a0e89d56`  
		Last Modified: Wed, 17 Nov 2021 03:12:03 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf845c6b55817c79ccede58e6e0be6a64696163cc63115477b3b1af46185a9d`  
		Last Modified: Wed, 17 Nov 2021 03:12:03 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
