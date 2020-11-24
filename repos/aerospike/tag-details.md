<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.20`](#aerospike50020)
-	[`aerospike:5.1.0.17`](#aerospike51017)
-	[`aerospike:5.2.0.9`](#aerospike5209)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.20`

```console
$ docker pull aerospike@sha256:b866b29dad2e589861cd5485bd00d6d441fcb9e290d872bce52dd46f0122101b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.20` - linux; amd64

```console
$ docker pull aerospike@sha256:e97f974f65f094b9d0e248f189de95ea119311f2e22f9e93f1f7d249680cc5ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59782785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e583b53d9fad1f21d85c6960d332f63f4d2c0d762dadf7196c6efdd70ed318`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:19:41 GMT
ENV AEROSPIKE_VERSION=5.0.0.20
# Mon, 23 Nov 2020 23:19:41 GMT
ENV AEROSPIKE_SHA256=f60a9ed480ccc1773d7b94f9171a12221db324eb965714c82c7d9e833a35eb1c
# Mon, 23 Nov 2020 23:19:59 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 23 Nov 2020 23:19:59 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 23 Nov 2020 23:20:00 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 23 Nov 2020 23:20:00 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 23 Nov 2020 23:20:00 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 23 Nov 2020 23:20:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f737a814bdbeb4038141fa627fbaa42edc49c16d92baa400f578f1831b285a8b`  
		Last Modified: Mon, 23 Nov 2020 23:21:07 GMT  
		Size: 37.3 MB (37253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b0170781d5191e653ae4e6b8c2d38d7d7069df6f540b635b97907751a751c8`  
		Last Modified: Mon, 23 Nov 2020 23:21:00 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1f7f6c66bed259d3251da816ed81ea1e2c437c15a2a624ce0ba3b6a6a86f67`  
		Last Modified: Mon, 23 Nov 2020 23:21:00 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.17`

```console
$ docker pull aerospike@sha256:63399046704ad5e2ae92a3d2f16c9a79805f9b4d5f6c18ddf8cb1973d738fe2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.17` - linux; amd64

```console
$ docker pull aerospike@sha256:5a8759aeca554b972f1363cd7c9f08fbb56accf53b194d599e9ed9ea2035c252
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67217198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca90e2a3b494ea4448ca8573f91a9bebce4f727f8dcc832814e988c5c4acc194`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:20:06 GMT
ENV AEROSPIKE_VERSION=5.1.0.17
# Mon, 23 Nov 2020 23:20:06 GMT
ENV AEROSPIKE_SHA256=6bcf6a8b35f7b87fe40d1ede346b908159d665e9955051f07913cd6bf8dfd4d6
# Mon, 23 Nov 2020 23:20:25 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 23 Nov 2020 23:20:25 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 23 Nov 2020 23:20:25 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 23 Nov 2020 23:20:25 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 23 Nov 2020 23:20:25 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 23 Nov 2020 23:20:26 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b631894c72bde0cd9951e9891638c33acfdb74832b192f81519d3c2897d108`  
		Last Modified: Mon, 23 Nov 2020 23:21:19 GMT  
		Size: 44.7 MB (44687482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedb72da8776200b0d3e683da9ac5ec630be9acb891c421cea422b3d26081fc`  
		Last Modified: Mon, 23 Nov 2020 23:21:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15eba573c33e8a1a25b5a0a4a3ce07e31eac863ab488aaeeed5f324310b16e1`  
		Last Modified: Mon, 23 Nov 2020 23:21:12 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.9`

```console
$ docker pull aerospike@sha256:cf6706ac53a0c52ebafbe8c1dadfae757f2ea804ec7c38a5b4359d1262e43bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:732da30fe8f16379470c30cee15e4a13c9f77b7029a67097a8300c256f52b492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67135082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffbbf26e5900190d6db5cf2e1166117d7f121ad39e38ef40e02508add25dfbe`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:20:31 GMT
ENV AEROSPIKE_VERSION=5.2.0.9
# Mon, 23 Nov 2020 23:20:32 GMT
ENV AEROSPIKE_SHA256=fe51e62a03b082ab781717b19c526e63d006663a03441fafdf6fdd930599ea5a
# Mon, 23 Nov 2020 23:20:50 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 23 Nov 2020 23:20:50 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 23 Nov 2020 23:20:50 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 23 Nov 2020 23:20:50 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 23 Nov 2020 23:20:51 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 23 Nov 2020 23:20:51 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d917d0215824e00212bcf81f2ac7f1de185dd9f8523dcada89e972476531a8be`  
		Last Modified: Mon, 23 Nov 2020 23:21:30 GMT  
		Size: 44.6 MB (44605365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93595821d48697bb162218e620ecf70f9ae34f492bb37d0d072d52938e160b6b`  
		Last Modified: Mon, 23 Nov 2020 23:21:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c4c03f33fb05381824e2790fb5e8ef422f0bf305750c645b6d74718076f42`  
		Last Modified: Mon, 23 Nov 2020 23:21:24 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:cf6706ac53a0c52ebafbe8c1dadfae757f2ea804ec7c38a5b4359d1262e43bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:732da30fe8f16379470c30cee15e4a13c9f77b7029a67097a8300c256f52b492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67135082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffbbf26e5900190d6db5cf2e1166117d7f121ad39e38ef40e02508add25dfbe`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:20:31 GMT
ENV AEROSPIKE_VERSION=5.2.0.9
# Mon, 23 Nov 2020 23:20:32 GMT
ENV AEROSPIKE_SHA256=fe51e62a03b082ab781717b19c526e63d006663a03441fafdf6fdd930599ea5a
# Mon, 23 Nov 2020 23:20:50 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 23 Nov 2020 23:20:50 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 23 Nov 2020 23:20:50 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 23 Nov 2020 23:20:50 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 23 Nov 2020 23:20:51 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 23 Nov 2020 23:20:51 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d917d0215824e00212bcf81f2ac7f1de185dd9f8523dcada89e972476531a8be`  
		Last Modified: Mon, 23 Nov 2020 23:21:30 GMT  
		Size: 44.6 MB (44605365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93595821d48697bb162218e620ecf70f9ae34f492bb37d0d072d52938e160b6b`  
		Last Modified: Mon, 23 Nov 2020 23:21:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c4c03f33fb05381824e2790fb5e8ef422f0bf305750c645b6d74718076f42`  
		Last Modified: Mon, 23 Nov 2020 23:21:24 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
