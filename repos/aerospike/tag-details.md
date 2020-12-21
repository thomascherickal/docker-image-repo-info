<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.1.0.20`](#aerospike51020)
-	[`aerospike:5.2.0.12`](#aerospike52012)
-	[`aerospike:5.3.0.3`](#aerospike5303)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.1.0.20`

**does not exist** (yet?)

## `aerospike:5.2.0.12`

**does not exist** (yet?)

## `aerospike:5.3.0.3`

**does not exist** (yet?)

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:4a36344ad0aa5558bfb3075cc701db689831237d743c95bef69b48024ef013c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:628d718c901663c18229fd02b28e06ac7038db074c62b8ee4cd9f9757f4a5c59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74704557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b35556ab7f65ccf44d05b5164530c45f3f1f92204f6cd4b98267c8b8d56465e`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Mon, 14 Dec 2020 20:20:57 GMT
ENV AEROSPIKE_VERSION=5.3.0.2
# Mon, 14 Dec 2020 20:20:57 GMT
ENV AEROSPIKE_SHA256=11f33419443e486821608e74bf7db318e184686503043cc1a3e7e07ab90eb059
# Mon, 14 Dec 2020 20:21:19 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 14 Dec 2020 20:21:20 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 14 Dec 2020 20:21:20 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 14 Dec 2020 20:21:20 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 14 Dec 2020 20:21:20 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 14 Dec 2020 20:21:20 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb9b2d282ca24425006dc718f434682c165c652fac20fedec88636754776c0e`  
		Last Modified: Mon, 14 Dec 2020 20:22:08 GMT  
		Size: 52.2 MB (52174645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60db2f7caae59bd95d73fe74c26a6fa7767cc9387d671039aad5b81f18e2226d`  
		Last Modified: Mon, 14 Dec 2020 20:21:59 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9324f2aa3ee701db23764111a044c3a0e027a103763a695d8b54b26e1d956e`  
		Last Modified: Mon, 14 Dec 2020 20:21:59 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
