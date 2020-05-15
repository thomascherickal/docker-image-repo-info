<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.8.0.9`](#aerospike4809)
-	[`aerospike:4.9.0.7`](#aerospike4907)
-	[`aerospike:5.0.0.3`](#aerospike5003)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.8.0.9`

```console
$ docker pull aerospike@sha256:6e1b75dfc2895f2d42c1f558b3a1bba7d46ac3ee24f42eeb7ba75d108044c854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:ad867f1ba41904a4e2e9934d0ca3c603450490928106ae32b48198f60782ee83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51852804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724739865e3319f782c68b7865a381fdee53f9a8c9862bed94a7bca2452edb15`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:02:39 GMT
ENV AEROSPIKE_VERSION=4.8.0.9
# Fri, 15 May 2020 18:02:39 GMT
ENV AEROSPIKE_SHA256=3af1b8c97d73d05054582c8941d435bea55b7ead9b04d2df42f1e9990ab7e0c3
# Fri, 15 May 2020 18:02:56 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 15 May 2020 18:02:56 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 15 May 2020 18:02:56 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 15 May 2020 18:02:56 GMT
VOLUME [/opt/aerospike/data]
# Fri, 15 May 2020 18:02:56 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 15 May 2020 18:02:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 18:02:57 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54c9e0a0eb0f37ea0c57e87fa793ee69cbf6aa0e017305c081aa56f5d711aca`  
		Last Modified: Fri, 15 May 2020 18:03:44 GMT  
		Size: 29.3 MB (29330866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132a4a8b95ea20303011bf6a6de40a791f949ec168cdbe700b7a863d31e6a6b`  
		Last Modified: Fri, 15 May 2020 18:03:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7662a0f44eac7d054f02f0fdb0fd60a55478e5b0e47c9575897e3a076732e8`  
		Last Modified: Fri, 15 May 2020 18:03:38 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.9.0.7`

```console
$ docker pull aerospike@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `aerospike:5.0.0.3`

```console
$ docker pull aerospike@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:b4be51e0c63adafd744a9d826391dddf4705159195c66ea475c2c823357fe0e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:6bef016b10bfa9216b20e10d4ca8d98165e80d9750a833047e3093d99b81fc9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53192493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8f8e8103b496c4e3bfa9fac77a24f88b8cd517e0a835fef10867c8e61e4dbc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:03:01 GMT
ENV AEROSPIKE_VERSION=4.9.0.5
# Fri, 15 May 2020 18:03:01 GMT
ENV AEROSPIKE_SHA256=7e9b345020e987d1a4d1c91034a8054c97fd80a0c917a8da04d4aad9127e8fe2
# Fri, 15 May 2020 18:03:21 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 15 May 2020 18:03:21 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 15 May 2020 18:03:21 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 15 May 2020 18:03:21 GMT
VOLUME [/opt/aerospike/data]
# Fri, 15 May 2020 18:03:21 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 15 May 2020 18:03:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 18:03:22 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6635c0da64586c2b1e638a90a0d5d4eb2891e583df9b880bbf2b9daa1df326`  
		Last Modified: Fri, 15 May 2020 18:03:52 GMT  
		Size: 30.7 MB (30670552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f716638cb00ac61513ec0028c54231b2bb38c0e9e18a45c81b696154aff450b`  
		Last Modified: Fri, 15 May 2020 18:03:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f8805626f93e98e174a35b13b71a3ea96f8c2f53de4784d641cec349b861c9`  
		Last Modified: Fri, 15 May 2020 18:03:47 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
