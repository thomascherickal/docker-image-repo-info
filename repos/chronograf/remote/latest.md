## `chronograf:latest`

```console
$ docker pull chronograf@sha256:f259092060d63db29b0356e00c46318f22925fda8dcb4aee19791945d22c31b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:1c756313c8a69c63c4619b304680984fb192f141091ee91b982c5291c5bd7878
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66880708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b64196243eeaa705a9b19fbfdf53545f9fc911c50bd186ec1813ea64aa3aeed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:38 GMT
ADD file:2868c3af63afe6b8aadac07b8776e5468a3ed135fd84ad22df15e48f0610c7ba in / 
# Wed, 17 Nov 2021 02:22:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:29:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 03:30:32 GMT
ENV CHRONOGRAF_VERSION=1.9.1
# Wed, 17 Nov 2021 03:30:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 03:30:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 17 Nov 2021 03:30:49 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 17 Nov 2021 03:30:49 GMT
EXPOSE 8888
# Wed, 17 Nov 2021 03:30:49 GMT
VOLUME [/var/lib/chronograf]
# Wed, 17 Nov 2021 03:30:50 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 17 Nov 2021 03:30:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 03:30:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:89166b5eeae47d8c878cb88f20cc67eda2a550a697f4be317c7b7abea566b76f`  
		Last Modified: Wed, 17 Nov 2021 02:29:32 GMT  
		Size: 22.5 MB (22527686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b0c653853f0c227451646f1798091111a9aeb0fe078403aba9be7a17190af3`  
		Last Modified: Wed, 17 Nov 2021 03:31:26 GMT  
		Size: 6.8 MB (6760168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf8ae8281e08985606cb7abf89f98cb72d55c08529e9c77919dfd3b6789569`  
		Last Modified: Wed, 17 Nov 2021 03:32:26 GMT  
		Size: 37.6 MB (37568457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6aa5f8deb98458848497329dea15711ddbc2dd4e0157f5f36e036213ebaba`  
		Last Modified: Wed, 17 Nov 2021 03:32:14 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7602ba9bfd91b93fe288c1faf3948841b287a0d30aa9eadb36d730754602fd`  
		Last Modified: Wed, 17 Nov 2021 03:32:14 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e453e78de5a17c1bb9a9e70a98bf3e39e8888eec13fefd51d5ef3d07cb671937`  
		Last Modified: Wed, 17 Nov 2021 03:32:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3fb18999dd46d064947de88c86f049f7ce677b11db15a4d4cf87c15b8b0d1321
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60400450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4aa55eda148d3b9748e46d3bc19063b771b86359c6f629fe806c3e5afb1bb58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:42 GMT
ADD file:9bfcfd0aaac802b902b0e842e040a6599c461c90b73579bcacc2fbdda7ec39cb in / 
# Tue, 12 Oct 2021 01:34:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 19:38:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 15 Oct 2021 22:58:13 GMT
ENV CHRONOGRAF_VERSION=1.9.1
# Fri, 15 Oct 2021 22:58:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 15 Oct 2021 22:58:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 15 Oct 2021 22:58:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 15 Oct 2021 22:58:35 GMT
EXPOSE 8888
# Fri, 15 Oct 2021 22:58:35 GMT
VOLUME [/var/lib/chronograf]
# Fri, 15 Oct 2021 22:58:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 15 Oct 2021 22:58:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Oct 2021 22:58:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a1a3620b17011bd36d6f64dfcc8fd7c4cb3da78d19a59efb1b35afcadaf3f6a8`  
		Last Modified: Tue, 12 Oct 2021 01:51:59 GMT  
		Size: 19.3 MB (19316474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdc2f2b4d96b348e56cf5179e6a1d2f89538251124d2659dcb521c5c19e51bb`  
		Last Modified: Tue, 12 Oct 2021 19:42:36 GMT  
		Size: 5.8 MB (5780488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb66a9a95b28e3a240c450633d5421211135b4312de046bce206afbb0f30edf9`  
		Last Modified: Fri, 15 Oct 2021 22:59:56 GMT  
		Size: 35.3 MB (35279095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec2c2711c3377ce218bad44c96856e245d745faa65f1687a85c49b1f8a56538`  
		Last Modified: Fri, 15 Oct 2021 22:59:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e65825543156a066468a039c1e306c2c2db19fc435de2dcd52973ad8a56f97d`  
		Last Modified: Fri, 15 Oct 2021 22:59:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291978c4564a4ffcbd216ab5bc6155061ae9c2b94b78ea4b685708808d67891`  
		Last Modified: Fri, 15 Oct 2021 22:59:37 GMT  
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
