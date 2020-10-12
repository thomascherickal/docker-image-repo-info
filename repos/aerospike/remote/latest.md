## `aerospike:latest`

```console
$ docker pull aerospike@sha256:1a49b9be06cad6f6697c5b85213f472c3fd861e1bb3f7b8590ce63f5cc6ee3c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:7c128ef363d571e0ce87995b1976919e82ecfa99aee79bc552ae428fabf7263f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65942736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e73ffe21fd483cb346eda54db898c693f8b6aa8c7682eb93cc486d93f268585`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_VERSION=5.2.0.2
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_SHA256=a60799791567b845d20aeaf73adf96ed2285d08145b3c5cac6746cc4e1f1f0d5
# Mon, 12 Oct 2020 22:20:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 12 Oct 2020 22:20:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 12 Oct 2020 22:20:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 12 Oct 2020 22:20:49 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 12 Oct 2020 22:20:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 22:20:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf44dc2eafa63b194b5fd385f0eab57742501c25734d94c8bfade2b582b7f9`  
		Last Modified: Mon, 12 Oct 2020 22:21:27 GMT  
		Size: 43.4 MB (43418408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b5373c93f52309e7458a527d4ce1d98b91214d1df5982e3e61a2541f7f3678`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eb3fe7f39a630629cb932430d66b74231aa66eb8b9b618fb027847b07f3c89`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
