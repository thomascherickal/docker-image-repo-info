<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-5.3.0.16`](#aerospikece-53016)
-	[`aerospike:ce-5.4.0.11`](#aerospikece-54011)
-	[`aerospike:ce-5.5.0.9`](#aerospikece-5509)
-	[`aerospike:ee-5.3.0.16`](#aerospikeee-53016)
-	[`aerospike:ee-5.4.0.11`](#aerospikeee-54011)
-	[`aerospike:ee-5.5.0.9`](#aerospikeee-5509)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:ce-5.3.0.16`

```console
$ docker pull aerospike@sha256:28df49e8183f4f011926394c5ee8ba3d7c12c72580909266f326769a197a6a5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.3.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:8a3c9e3a4ab612f23fea8f76b9c2f64a0c740ccdabae02cb2e8c01e4b329db99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74702988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9cd6cbdef23ad0e52cadf54f236b1677087a52814b45868afba6fadfe060cb`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:47:27 GMT
ENV AEROSPIKE_VERSION=5.3.0.16
# Wed, 12 May 2021 01:50:27 GMT
ENV AEROSPIKE_SHA256=9bcda09cf0c1570747a6d97e3de8a550b31ff6cd74700200a75539323229055d
# Wed, 12 May 2021 01:50:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:50:59 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:50:59 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 12 May 2021 01:51:00 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 12 May 2021 01:51:00 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:51:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64da0b955129d47eeed4e821ef93bda4da335fe71b4ee163cce5c28bdf682d24`  
		Last Modified: Wed, 12 May 2021 01:53:15 GMT  
		Size: 52.2 MB (52172669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa37adff9a8c9b5d0e23e7040436ee3665e6115e3845110841802ee783e2c9e`  
		Last Modified: Wed, 12 May 2021 01:53:05 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bac70e286f23863205577436547d4decfc936b0ce44ab2a9f1a05c78f6bb84`  
		Last Modified: Wed, 12 May 2021 01:53:05 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ce-5.4.0.11`

```console
$ docker pull aerospike@sha256:91b8a389ed0b61318a0428674b71399de3679c911a920109ccf4a67cb3521c59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.4.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:203166448e747048708ea23997c878fc858da2c21f90edb68ed7fb1a4bf7e9ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74723752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9966e71ce43521461e5cd25d17060fb4d38f30205f476ff1f18652967f4749`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_VERSION=5.4.0.11
# Wed, 12 May 2021 01:49:51 GMT
ENV AEROSPIKE_SHA256=8ce655f36b18bf89f2f0c687c594d222371c2330ffaaa9509697051d7994ebc7
# Wed, 12 May 2021 01:50:20 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:50:20 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:50:20 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 12 May 2021 01:50:21 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 12 May 2021 01:50:21 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:50:21 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f9d8d34f6e7a63749b41787ca2cd60a1787ff6bf77c269c159fa67dc828d9f`  
		Last Modified: Wed, 12 May 2021 01:52:57 GMT  
		Size: 52.2 MB (52193432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a0021d5420968da43e64ad1f64ab8d4abaaa393384331bff93e2600a810f50`  
		Last Modified: Wed, 12 May 2021 01:52:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0648cc3934d5d791489c14346b0aa12354d4c6a6d196e7788ad71961fc80c5`  
		Last Modified: Wed, 12 May 2021 01:52:46 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ce-5.5.0.9`

```console
$ docker pull aerospike@sha256:2879252a6e61c02690153f84ddc32d2ae3e27c88604d46c721edfaf61d3a4e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:355793c3c1ca5eec8d240f757f4953800882ee4ae81cc508afc97115d86aea00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74778460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce4a9e712ba8b61e91b2d197e774f841592929c4e3e73a9c9fc67cfcc3ce06`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Wed, 12 May 2021 01:49:15 GMT
ENV AEROSPIKE_SHA256=3e4e8f35c4607a465781e8f6b662494ca16717300746064ae7a1c09fd3b5ac90
# Wed, 12 May 2021 01:49:42 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:49:43 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:49:43 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 12 May 2021 01:49:44 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 12 May 2021 01:49:44 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:49:44 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66ab9f4217ba78f5a9eccccd54ebb0db2f3a19d27f6a3759ce96c0e3fe23f44`  
		Last Modified: Wed, 12 May 2021 01:52:38 GMT  
		Size: 52.2 MB (52248142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d93535340e8edcb9723e5093337d696021202e6909bd270ac4ae431b50ba641`  
		Last Modified: Wed, 12 May 2021 01:52:27 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a209082495bc63d19471fb0b7ea36b0455fe981213a41d9f9ccf46c7d49527`  
		Last Modified: Wed, 12 May 2021 01:52:27 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-5.3.0.16`

```console
$ docker pull aerospike@sha256:f37216310815da5ac5eda503f4059395566ff57424edbc58c1a2f5dbed904418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.3.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:7e35adad5870b3b98090565d3da18c257630e5806aa236a3ebafba7713939854
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76373688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb9027947820abdd32c7c6b3d49f7a3fbfc9b736822c309b36756adffe4f574`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:47:27 GMT
ENV AEROSPIKE_VERSION=5.3.0.16
# Wed, 12 May 2021 01:47:27 GMT
ENV AEROSPIKE_SHA256=1408e186da1d5bb225a7296091ad32330b6c39c89dc3a45077c7e869c6e80edd
# Wed, 12 May 2021 01:47:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:47:59 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:47:59 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:47:59 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:47:59 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:48:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5bf363b6f6b1130c20e27caeb84120b5cbb10769d5b9853dbcd81538249f9c`  
		Last Modified: Wed, 12 May 2021 01:51:35 GMT  
		Size: 53.8 MB (53843305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf8975fd92a01ac4b97d36d596d800084d03dd8edd44288189af65278de94c7`  
		Last Modified: Wed, 12 May 2021 01:51:25 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d74e43830856a4badf30dc29823b4ae93d79d1fae5d3d15bb539cf2907ffe3`  
		Last Modified: Wed, 12 May 2021 01:51:25 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-5.4.0.11`

```console
$ docker pull aerospike@sha256:9df903be9751f4a7a536f76050b27367a2f2873e198862d8e216a294bb5894a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.4.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:da35b809db6387c977e197fe6c135cc1c575054198eaf4eae07040f37e0064f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76410761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3beabf17fb9124a5facc145a39f6fcb18cccdc02c31cab69faec704aa6ff2e`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_VERSION=5.4.0.11
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_SHA256=a23c586ae4fdd31f916b2dda5b7c9f86a4a529cc32b110f13fda6fa393e5be93
# Wed, 12 May 2021 01:48:32 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:48:33 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:48:33 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:48:33 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:48:34 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:48:34 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ff9e6860b0b1234399fe109db0458300a5743421671edcc167368c47ff1a4a`  
		Last Modified: Wed, 12 May 2021 01:51:54 GMT  
		Size: 53.9 MB (53880378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf9bc1765e06f99e7dbc3c3db66a2c46045018f2c5f54db03e404eab9cec96`  
		Last Modified: Wed, 12 May 2021 01:51:43 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef3ddd04f606550dd2b4dbcacdfc8415de7938e5c915932fed1213a506f1265`  
		Last Modified: Wed, 12 May 2021 01:51:43 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-5.5.0.9`

```console
$ docker pull aerospike@sha256:93dd21219b26ccc163f8732b22a595247ed86d4aeba8dd1988410f40dbc795e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:b728c6cc666c7eab45ef504b3a1820aa9ffbaa0c545391c381bee6aafa74e2c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76466660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd19df67e5de262814a0ea4d70c86d53de610ceb2f70b4385e10da98ea95eb6`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_SHA256=ae222dcb2e8deb10e1fe45b27d02f32749ec2259c62a292d253d176689b05a06
# Wed, 12 May 2021 01:49:07 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:49:08 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:49:08 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:49:08 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:49:09 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:49:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d28478b0d5758137f998e0932a9ba89d6a883cc3d2c1b2c8edd2fef497c88`  
		Last Modified: Wed, 12 May 2021 01:52:17 GMT  
		Size: 53.9 MB (53936277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5749258c6dd58e5600f83c6e45b1343ea458b9710770d987b745217f3ebc5`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f444a64949cb9febef2abc39735ef1b4f29e6f2518d32465948b021c10936`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:93dd21219b26ccc163f8732b22a595247ed86d4aeba8dd1988410f40dbc795e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:b728c6cc666c7eab45ef504b3a1820aa9ffbaa0c545391c381bee6aafa74e2c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76466660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd19df67e5de262814a0ea4d70c86d53de610ceb2f70b4385e10da98ea95eb6`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_SHA256=ae222dcb2e8deb10e1fe45b27d02f32749ec2259c62a292d253d176689b05a06
# Wed, 12 May 2021 01:49:07 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:49:08 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:49:08 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:49:08 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:49:09 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:49:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d28478b0d5758137f998e0932a9ba89d6a883cc3d2c1b2c8edd2fef497c88`  
		Last Modified: Wed, 12 May 2021 01:52:17 GMT  
		Size: 53.9 MB (53936277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5749258c6dd58e5600f83c6e45b1343ea458b9710770d987b745217f3ebc5`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f444a64949cb9febef2abc39735ef1b4f29e6f2518d32465948b021c10936`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
