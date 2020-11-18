## `aerospike:latest`

```console
$ docker pull aerospike@sha256:4ee617950476bce828e148d231cb3e209c0c0bf906a269ba617095ecd0dfc840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:c9633e8c0d4c3054f5099b26758fe32ba94e8cf39206e06980dcc8ebb91fbf1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f0c9a663d11a966448619daceaafcd8165ea4a1223087f64651f448364e9a9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_VERSION=5.2.0.7
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_SHA256=5f64b516be56f16a708991785d9525c18dc16f73418070738c3e5dd3dcae7ea8
# Wed, 18 Nov 2020 05:59:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 18 Nov 2020 05:59:11 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 18 Nov 2020 05:59:12 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 18 Nov 2020 05:59:12 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 18 Nov 2020 05:59:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 18 Nov 2020 05:59:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee4ca5131e1d8f81e18c4b04103695bcb8ee63af05cc2731a08b4dbae020b06`  
		Last Modified: Wed, 18 Nov 2020 06:00:04 GMT  
		Size: 44.6 MB (44604172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2abbd6b8920677d4e83288e4af49a3c36d796c8ec4d96518f44cb6e8a34143c`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2728479151082ff2e2d8897461f0f1b095e417dcad03ee2c68d1086ce915c799`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
