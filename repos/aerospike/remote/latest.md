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
