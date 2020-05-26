## `aerospike:latest`

```console
$ docker pull aerospike@sha256:f146a121e6ba6e75cb306b8ea37f2770539a8da9a14a71c46b1c01e6de3224dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:bc2286efde1b20515a901f7df1fef3831ca4b2a04bd830d78583f328b26c1875
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53090683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943526f108fcc376c7b5151a396f0a3330a41bb0362a0c4729deea8d761ef5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_VERSION=5.0.0.4
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_SHA256=30638676e17a5918fcc91a5e1b93eec95823a465d1c68bdf8574241d5e68ea61
# Tue, 26 May 2020 22:20:54 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 26 May 2020 22:20:54 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 26 May 2020 22:20:55 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 26 May 2020 22:20:55 GMT
VOLUME [/opt/aerospike/data]
# Tue, 26 May 2020 22:20:55 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 26 May 2020 22:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 22:20:56 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a14cf606a112b836e5f119002ec0b2334b0afd2d32323a3d72ee98ff25642f`  
		Last Modified: Tue, 26 May 2020 22:21:54 GMT  
		Size: 30.6 MB (30568742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72509580413e525dc37f23016b43051e3532005762c22361817ac601f5c24680`  
		Last Modified: Tue, 26 May 2020 22:21:30 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2d8a1c37f086f0bbbba02a8089f828ed0b7c0d2fb7ac179a1c4b5d6fb2013`  
		Last Modified: Tue, 26 May 2020 22:21:31 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
