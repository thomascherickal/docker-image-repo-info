## `aerospike:latest`

```console
$ docker pull aerospike@sha256:3d0a36179a4ea9e094d81178f823a0004f9300e3e3a2689de479974e7f093282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:e380b2dd6336569997e67529cf8f4f20345d8d11159aa7f05edba5111d3961a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74727848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaa94543ff0a9da69fac4946010c2175285da30e9c5f08aba02363dc78dfe5a`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_VERSION=5.4.0.2
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_SHA256=f1fa3b73e5de572b1ff927b25ff43b5eef734a6f6854c34eb2fe01d886170e33
# Mon, 25 Jan 2021 20:21:37 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:21:38 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:21:38 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:21:39 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce9980d8f8f9d90196c6648ee5a42e22dc89f8b05792d6107a0a127d50c363c`  
		Last Modified: Mon, 25 Jan 2021 20:22:46 GMT  
		Size: 52.2 MB (52197187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaad568b5e18c0eddd0a51d525d4bba7ef57cbc0decceaff76aa298ab353ec2`  
		Last Modified: Mon, 25 Jan 2021 20:22:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d860f6c3d9c8b0418028639ab766c3dd1a5e22089ace86110dcddd92c1d74d30`  
		Last Modified: Mon, 25 Jan 2021 20:22:36 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
