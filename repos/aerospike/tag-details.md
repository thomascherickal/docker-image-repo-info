<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.1.0.19`](#aerospike51019)
-	[`aerospike:5.2.0.11`](#aerospike52011)
-	[`aerospike:5.3.0.2`](#aerospike5302)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.1.0.19`

**does not exist** (yet?)

## `aerospike:5.2.0.11`

**does not exist** (yet?)

## `aerospike:5.3.0.2`

**does not exist** (yet?)

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:2cbe03563f44546bd5d6c70ed953a53224bc150c2a94fa2ec7e758d4d99f8ca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:ffcc6f82106da2bbb1db694e4bd98856590891fcecf1ab4e36fd1b32e03e2eb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b34a33e05549038c3f0a1a718d9bfe0065cabb66f9e4dc38472238c35ee36721`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:34:28 GMT
ENV AEROSPIKE_VERSION=5.2.0.10
# Fri, 11 Dec 2020 20:34:28 GMT
ENV AEROSPIKE_SHA256=7b765d77cc391d7ea3991c335801972b703e01ac19b9116d266b5c0b57f1ca8d
# Fri, 11 Dec 2020 20:34:47 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 11 Dec 2020 20:34:47 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 11 Dec 2020 20:34:47 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 11 Dec 2020 20:34:47 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 11 Dec 2020 20:34:47 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Fri, 11 Dec 2020 20:34:48 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeedefa0514d607e5223cd91ad9f0b67952f575d813658607cc6ad358c54bfa`  
		Last Modified: Fri, 11 Dec 2020 20:35:32 GMT  
		Size: 44.6 MB (44603713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d606ec9198a004ca6e9817da932a950b94a51b55d56ce40adf2a82fb910064d`  
		Last Modified: Fri, 11 Dec 2020 20:35:26 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfca89a6d881e487ac78fd1a560c3936efe35a5c68cb9dfb2e7dfc7d84c82e3`  
		Last Modified: Fri, 11 Dec 2020 20:35:25 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
