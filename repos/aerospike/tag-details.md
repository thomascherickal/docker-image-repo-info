<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.13`](#aerospike50013)
-	[`aerospike:5.1.0.10`](#aerospike51010)
-	[`aerospike:5.2.0.2`](#aerospike5202)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.13`

**does not exist** (yet?)

## `aerospike:5.1.0.10`

**does not exist** (yet?)

## `aerospike:5.2.0.2`

**does not exist** (yet?)

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:543645a77f4b53126e55f5a38188543e60bf993bbbbe6fa019132ed81852393a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:e973759b54ebb3499910e70f38b06ab1f46f848346bd2e50d5591b9dc1e1bbfc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66025934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a9db1ae18281a52e7266307b073444b1a8c8eaa5a256de66ccd4d59bda4376`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:55:29 GMT
ENV AEROSPIKE_VERSION=5.1.0.6
# Thu, 10 Sep 2020 00:55:30 GMT
ENV AEROSPIKE_SHA256=64d39a81286de648592add8a4de3037c4141d55a135dfeddfa4b3c6534c297e7
# Thu, 10 Sep 2020 00:55:59 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Thu, 10 Sep 2020 00:56:00 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 10 Sep 2020 00:56:00 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 10 Sep 2020 00:56:00 GMT
VOLUME [/opt/aerospike/data]
# Thu, 10 Sep 2020 00:56:00 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 10 Sep 2020 00:56:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Sep 2020 00:56:01 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53d3cfb98de2eeedb7ef1e1c02db6b0c4a44abe56802cd991a7709350d64b9b`  
		Last Modified: Thu, 10 Sep 2020 00:56:47 GMT  
		Size: 43.5 MB (43501605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5aa4529669138b39187a737ae7aeef35616058aafaa999645dc080a9c893031`  
		Last Modified: Thu, 10 Sep 2020 00:56:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988d9b724bf04e46082c36fc348a21ae566913d72065b2d70c5f5136da82f599`  
		Last Modified: Thu, 10 Sep 2020 00:56:40 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
