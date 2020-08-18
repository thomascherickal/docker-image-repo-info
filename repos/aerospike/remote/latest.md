## `aerospike:latest`

```console
$ docker pull aerospike@sha256:065cbb8d3d7a9f4b34178d50a73c5f5d7fafcfb71314a61d2a354ac664699c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:88f1191ca783e74355000bc1e247c62a0ad3277bee025daafaed8504570192dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66011213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46bdce9abaaa743f1020ff9e923c022f1dae46b3301d6419ea39765a826e378c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 18 Aug 2020 20:19:30 GMT
ENV AEROSPIKE_VERSION=5.1.0.6
# Tue, 18 Aug 2020 20:19:31 GMT
ENV AEROSPIKE_SHA256=64d39a81286de648592add8a4de3037c4141d55a135dfeddfa4b3c6534c297e7
# Tue, 18 Aug 2020 20:19:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 18 Aug 2020 20:19:49 GMT
VOLUME [/opt/aerospike/data]
# Tue, 18 Aug 2020 20:19:49 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 18 Aug 2020 20:19:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 18 Aug 2020 20:19:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c09823ef0005ce5ed526e2f1922828405cba3952c6d38fc5df9d3a1047f90`  
		Last Modified: Tue, 18 Aug 2020 20:20:07 GMT  
		Size: 43.5 MB (43486883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08e522e5e9db03b0e3787896455e01fc38b8b7f3333c7fba70c70273e2a33c`  
		Last Modified: Tue, 18 Aug 2020 20:20:01 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb7643131170ce42d78dc6001424b3b0e73bd4630e34458a18319dcab4a9e5d`  
		Last Modified: Tue, 18 Aug 2020 20:20:00 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
