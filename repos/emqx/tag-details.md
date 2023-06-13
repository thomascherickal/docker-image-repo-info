<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.18`](#emqx4418)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:45edad31732db122b4f8e35415a6781ad5d3da0cc028bbf3b6f2f91551198894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:2b2cf3af1e1fdc946d0400e6ef8bc3f2754ddb861f739c78360c3d39cb253746
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8154d287a0cd41ae6f26959af0d5aa9adf0e765d9f5940eae3fde58c3aab944`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 04:05:14 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 04:05:14 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 04:05:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 04:05:19 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:19 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:19 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 04:05:19 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11ad7fd953a334956026fc08b55abb1625fbaad5c2540a1d531ed566da6f031`  
		Last Modified: Tue, 13 Jun 2023 04:05:47 GMT  
		Size: 2.6 MB (2569638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6105da9fef63b5bef345d47ed904190ccb2362f38449341ce80b93b5b72941db`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f883bad9be8bf6dd4cc27edca3cca8ee64f80b3afadab702283823b30d8b01`  
		Last Modified: Tue, 13 Jun 2023 04:05:51 GMT  
		Size: 47.3 MB (47298222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45046c6a3a747679abb1bffe6cd4755e04900a76a30a5369f1ef54700f63440e`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3e063e691e7483fad65596bff459c5569a6c3fa562fe82d04d03936e41121981
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4b9057d01f5c22302deaba4afcac7de0aa1b60ae88596506afe78a4b29fe08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:13:46 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 03:13:46 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 03:13:46 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 03:13:50 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 03:13:50 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:13:51 GMT
USER emqx
# Tue, 13 Jun 2023 03:13:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:13:51 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 03:13:51 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 03:13:51 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:13:51 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a02187add624aa9fe23926c5bdf6318dabc18061ab217d54f5375202fd6d19`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 2.6 MB (2559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e8c2968dd5f6078c0a14359c292527f47afaeb256bda3d5da2f744e0a2f5b`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f66126cdd9932196fc8ec131abf7a6cc64b67c0a43e035f5b06db81967413e`  
		Last Modified: Tue, 13 Jun 2023 03:14:19 GMT  
		Size: 40.1 MB (40079893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7fdccebf1e79e89be1179ea0eae21d96342ecb81d3ad4a7e379982fa2d2b1d`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:45edad31732db122b4f8e35415a6781ad5d3da0cc028bbf3b6f2f91551198894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:2b2cf3af1e1fdc946d0400e6ef8bc3f2754ddb861f739c78360c3d39cb253746
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8154d287a0cd41ae6f26959af0d5aa9adf0e765d9f5940eae3fde58c3aab944`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 04:05:14 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 04:05:14 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 04:05:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 04:05:19 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:19 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:19 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 04:05:19 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11ad7fd953a334956026fc08b55abb1625fbaad5c2540a1d531ed566da6f031`  
		Last Modified: Tue, 13 Jun 2023 04:05:47 GMT  
		Size: 2.6 MB (2569638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6105da9fef63b5bef345d47ed904190ccb2362f38449341ce80b93b5b72941db`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f883bad9be8bf6dd4cc27edca3cca8ee64f80b3afadab702283823b30d8b01`  
		Last Modified: Tue, 13 Jun 2023 04:05:51 GMT  
		Size: 47.3 MB (47298222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45046c6a3a747679abb1bffe6cd4755e04900a76a30a5369f1ef54700f63440e`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3e063e691e7483fad65596bff459c5569a6c3fa562fe82d04d03936e41121981
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4b9057d01f5c22302deaba4afcac7de0aa1b60ae88596506afe78a4b29fe08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:13:46 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 03:13:46 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 03:13:46 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 03:13:50 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 03:13:50 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:13:51 GMT
USER emqx
# Tue, 13 Jun 2023 03:13:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:13:51 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 03:13:51 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 03:13:51 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:13:51 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a02187add624aa9fe23926c5bdf6318dabc18061ab217d54f5375202fd6d19`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 2.6 MB (2559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e8c2968dd5f6078c0a14359c292527f47afaeb256bda3d5da2f744e0a2f5b`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f66126cdd9932196fc8ec131abf7a6cc64b67c0a43e035f5b06db81967413e`  
		Last Modified: Tue, 13 Jun 2023 03:14:19 GMT  
		Size: 40.1 MB (40079893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7fdccebf1e79e89be1179ea0eae21d96342ecb81d3ad4a7e379982fa2d2b1d`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.18`

```console
$ docker pull emqx@sha256:45edad31732db122b4f8e35415a6781ad5d3da0cc028bbf3b6f2f91551198894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.18` - linux; amd64

```console
$ docker pull emqx@sha256:2b2cf3af1e1fdc946d0400e6ef8bc3f2754ddb861f739c78360c3d39cb253746
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8154d287a0cd41ae6f26959af0d5aa9adf0e765d9f5940eae3fde58c3aab944`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 04:05:14 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 04:05:14 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 04:05:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 04:05:19 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:19 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:19 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 04:05:19 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11ad7fd953a334956026fc08b55abb1625fbaad5c2540a1d531ed566da6f031`  
		Last Modified: Tue, 13 Jun 2023 04:05:47 GMT  
		Size: 2.6 MB (2569638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6105da9fef63b5bef345d47ed904190ccb2362f38449341ce80b93b5b72941db`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f883bad9be8bf6dd4cc27edca3cca8ee64f80b3afadab702283823b30d8b01`  
		Last Modified: Tue, 13 Jun 2023 04:05:51 GMT  
		Size: 47.3 MB (47298222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45046c6a3a747679abb1bffe6cd4755e04900a76a30a5369f1ef54700f63440e`  
		Last Modified: Tue, 13 Jun 2023 04:05:46 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.18` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3e063e691e7483fad65596bff459c5569a6c3fa562fe82d04d03936e41121981
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4b9057d01f5c22302deaba4afcac7de0aa1b60ae88596506afe78a4b29fe08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:13:46 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 13 Jun 2023 03:13:46 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 13 Jun 2023 03:13:46 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 13 Jun 2023 03:13:50 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 13 Jun 2023 03:13:50 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:13:51 GMT
USER emqx
# Tue, 13 Jun 2023 03:13:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:13:51 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 13 Jun 2023 03:13:51 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 13 Jun 2023 03:13:51 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:13:51 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a02187add624aa9fe23926c5bdf6318dabc18061ab217d54f5375202fd6d19`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 2.6 MB (2559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e8c2968dd5f6078c0a14359c292527f47afaeb256bda3d5da2f744e0a2f5b`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f66126cdd9932196fc8ec131abf7a6cc64b67c0a43e035f5b06db81967413e`  
		Last Modified: Tue, 13 Jun 2023 03:14:19 GMT  
		Size: 40.1 MB (40079893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7fdccebf1e79e89be1179ea0eae21d96342ecb81d3ad4a7e379982fa2d2b1d`  
		Last Modified: Tue, 13 Jun 2023 03:14:15 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:3b13d25121c260a24ef98fc7f4fd59e41040623d2a0d06a0f48b891f849a88f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:4c35e0bc1118239811e974dd383eaf13b5c30b80153e0e25ee31aa2d31ead0c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681380b29d8df286b720c20311cc02e83da157bb835b04c42dcda0fd19a43678`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:28 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 04:05:28 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 04:05:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 04:05:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 04:05:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 04:05:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 04:05:36 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:36 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:36 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 04:05:36 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:36 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9455449c3836673343cfe4a251856a028b9edb7faf316b905d1414568c13634c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 3.0 MB (2987797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e966bf28b5d866b8ef51054ae90093f7819a1ed717f5918ae5fbcbfd8b16a4c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297da6d562816a699128e55188d4be62568f5c6d786f78ff6b3241b7338f53cb`  
		Last Modified: Tue, 13 Jun 2023 04:06:08 GMT  
		Size: 67.6 MB (67571866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e7afe3bef593b419b59bbbaff2dabe2a6302a3dc415f0c9599c0e5ec731dee`  
		Last Modified: Tue, 13 Jun 2023 04:06:00 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:513baab0e22cec2f23a8b2321610d01fa457ce6ee7f4b7a2bfb11a73b9c30b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f216c71b739662bb1a7257a2eee995e859dd0981b0832ba2d9128f2411b73ff4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:14:00 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 03:14:00 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 03:14:00 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 03:14:00 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 03:14:00 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 03:14:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 03:14:06 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:14:06 GMT
USER emqx
# Tue, 13 Jun 2023 03:14:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:14:06 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 03:14:06 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 03:14:06 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:14:06 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3480a0a0634abda4389ecea698ff01416185e3895e0fa62cac52013ac872e753`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 3.0 MB (3003016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82abf033b86734fc9c4b2ea4fa863229647ac1f67f9803d628b3152b358d6638`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c65686f0b11cd44966222dc907536bbdbb14fa62a9bcfecf2c6561d050b751`  
		Last Modified: Tue, 13 Jun 2023 03:14:33 GMT  
		Size: 60.0 MB (59989375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89881a95f2d4b4f77b8b61349968773c6843a3225add5afec107595502beb1bd`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:3b13d25121c260a24ef98fc7f4fd59e41040623d2a0d06a0f48b891f849a88f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:4c35e0bc1118239811e974dd383eaf13b5c30b80153e0e25ee31aa2d31ead0c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681380b29d8df286b720c20311cc02e83da157bb835b04c42dcda0fd19a43678`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:28 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 04:05:28 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 04:05:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 04:05:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 04:05:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 04:05:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 04:05:36 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:36 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:36 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 04:05:36 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:36 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9455449c3836673343cfe4a251856a028b9edb7faf316b905d1414568c13634c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 3.0 MB (2987797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e966bf28b5d866b8ef51054ae90093f7819a1ed717f5918ae5fbcbfd8b16a4c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297da6d562816a699128e55188d4be62568f5c6d786f78ff6b3241b7338f53cb`  
		Last Modified: Tue, 13 Jun 2023 04:06:08 GMT  
		Size: 67.6 MB (67571866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e7afe3bef593b419b59bbbaff2dabe2a6302a3dc415f0c9599c0e5ec731dee`  
		Last Modified: Tue, 13 Jun 2023 04:06:00 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:513baab0e22cec2f23a8b2321610d01fa457ce6ee7f4b7a2bfb11a73b9c30b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f216c71b739662bb1a7257a2eee995e859dd0981b0832ba2d9128f2411b73ff4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:14:00 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 03:14:00 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 03:14:00 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 03:14:00 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 03:14:00 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 03:14:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 03:14:06 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:14:06 GMT
USER emqx
# Tue, 13 Jun 2023 03:14:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:14:06 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 03:14:06 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 03:14:06 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:14:06 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3480a0a0634abda4389ecea698ff01416185e3895e0fa62cac52013ac872e753`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 3.0 MB (3003016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82abf033b86734fc9c4b2ea4fa863229647ac1f67f9803d628b3152b358d6638`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c65686f0b11cd44966222dc907536bbdbb14fa62a9bcfecf2c6561d050b751`  
		Last Modified: Tue, 13 Jun 2023 03:14:33 GMT  
		Size: 60.0 MB (59989375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89881a95f2d4b4f77b8b61349968773c6843a3225add5afec107595502beb1bd`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:3b13d25121c260a24ef98fc7f4fd59e41040623d2a0d06a0f48b891f849a88f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:4c35e0bc1118239811e974dd383eaf13b5c30b80153e0e25ee31aa2d31ead0c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681380b29d8df286b720c20311cc02e83da157bb835b04c42dcda0fd19a43678`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:28 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 04:05:28 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 04:05:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 04:05:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 04:05:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 04:05:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 04:05:36 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:36 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:36 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 04:05:36 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:36 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9455449c3836673343cfe4a251856a028b9edb7faf316b905d1414568c13634c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 3.0 MB (2987797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e966bf28b5d866b8ef51054ae90093f7819a1ed717f5918ae5fbcbfd8b16a4c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297da6d562816a699128e55188d4be62568f5c6d786f78ff6b3241b7338f53cb`  
		Last Modified: Tue, 13 Jun 2023 04:06:08 GMT  
		Size: 67.6 MB (67571866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e7afe3bef593b419b59bbbaff2dabe2a6302a3dc415f0c9599c0e5ec731dee`  
		Last Modified: Tue, 13 Jun 2023 04:06:00 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:513baab0e22cec2f23a8b2321610d01fa457ce6ee7f4b7a2bfb11a73b9c30b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f216c71b739662bb1a7257a2eee995e859dd0981b0832ba2d9128f2411b73ff4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:14:00 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 03:14:00 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 03:14:00 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 03:14:00 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 03:14:00 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 03:14:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 03:14:06 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:14:06 GMT
USER emqx
# Tue, 13 Jun 2023 03:14:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:14:06 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 03:14:06 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 03:14:06 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:14:06 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3480a0a0634abda4389ecea698ff01416185e3895e0fa62cac52013ac872e753`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 3.0 MB (3003016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82abf033b86734fc9c4b2ea4fa863229647ac1f67f9803d628b3152b358d6638`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c65686f0b11cd44966222dc907536bbdbb14fa62a9bcfecf2c6561d050b751`  
		Last Modified: Tue, 13 Jun 2023 03:14:33 GMT  
		Size: 60.0 MB (59989375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89881a95f2d4b4f77b8b61349968773c6843a3225add5afec107595502beb1bd`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:3b13d25121c260a24ef98fc7f4fd59e41040623d2a0d06a0f48b891f849a88f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:4c35e0bc1118239811e974dd383eaf13b5c30b80153e0e25ee31aa2d31ead0c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681380b29d8df286b720c20311cc02e83da157bb835b04c42dcda0fd19a43678`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:05:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:05:28 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 04:05:28 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 04:05:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 04:05:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 04:05:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 04:05:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 04:05:36 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 04:05:36 GMT
USER emqx
# Tue, 13 Jun 2023 04:05:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 04:05:36 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 04:05:36 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 04:05:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:05:36 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9455449c3836673343cfe4a251856a028b9edb7faf316b905d1414568c13634c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 3.0 MB (2987797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e966bf28b5d866b8ef51054ae90093f7819a1ed717f5918ae5fbcbfd8b16a4c`  
		Last Modified: Tue, 13 Jun 2023 04:06:01 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297da6d562816a699128e55188d4be62568f5c6d786f78ff6b3241b7338f53cb`  
		Last Modified: Tue, 13 Jun 2023 04:06:08 GMT  
		Size: 67.6 MB (67571866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e7afe3bef593b419b59bbbaff2dabe2a6302a3dc415f0c9599c0e5ec731dee`  
		Last Modified: Tue, 13 Jun 2023 04:06:00 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:513baab0e22cec2f23a8b2321610d01fa457ce6ee7f4b7a2bfb11a73b9c30b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f216c71b739662bb1a7257a2eee995e859dd0981b0832ba2d9128f2411b73ff4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:13:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:14:00 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 13 Jun 2023 03:14:00 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 13 Jun 2023 03:14:00 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 13 Jun 2023 03:14:00 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 13 Jun 2023 03:14:00 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 13 Jun 2023 03:14:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 13 Jun 2023 03:14:06 GMT
WORKDIR /opt/emqx
# Tue, 13 Jun 2023 03:14:06 GMT
USER emqx
# Tue, 13 Jun 2023 03:14:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 13 Jun 2023 03:14:06 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 13 Jun 2023 03:14:06 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 13 Jun 2023 03:14:06 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:14:06 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3480a0a0634abda4389ecea698ff01416185e3895e0fa62cac52013ac872e753`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 3.0 MB (3003016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82abf033b86734fc9c4b2ea4fa863229647ac1f67f9803d628b3152b358d6638`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c65686f0b11cd44966222dc907536bbdbb14fa62a9bcfecf2c6561d050b751`  
		Last Modified: Tue, 13 Jun 2023 03:14:33 GMT  
		Size: 60.0 MB (59989375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89881a95f2d4b4f77b8b61349968773c6843a3225add5afec107595502beb1bd`  
		Last Modified: Tue, 13 Jun 2023 03:14:28 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
