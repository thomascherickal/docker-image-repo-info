## `aerospike:ce-5.6.0.5`

```console
$ docker pull aerospike@sha256:9f7d3ecd4f8da75f486f7a2091bb1f6a5b32751a53abc9757a44a5b954a240f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.6.0.5` - linux; amd64

```console
$ docker pull aerospike@sha256:0fc358636dbbd979e4dee270d1bd0aff757fcb104701ff2aa95a18c0ef59fcc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80604734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd1bc969535f6bebccb2b765f58144465aea1990196e87f8083b64b9fd3cb06`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:52:44 GMT
ENV AEROSPIKE_VERSION=5.6.0.5
# Wed, 02 Jun 2021 19:53:14 GMT
ENV AEROSPIKE_SHA256=a173e5fabe9a0c6f51d717f0989b26fb22313f9de971de9ac296209123e654ef
# Wed, 02 Jun 2021 19:53:33 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 02 Jun 2021 19:53:34 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Jun 2021 19:53:34 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Wed, 02 Jun 2021 19:53:34 GMT
EXPOSE 3000 3001 3002
# Wed, 02 Jun 2021 19:53:35 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Jun 2021 19:53:35 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d481d571265aa158b6a3483b1a5d0fa102a543ac3bd6c377448d513ff489521`  
		Last Modified: Wed, 02 Jun 2021 19:54:10 GMT  
		Size: 53.5 MB (53456798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de1cd9b10ca3462a93c6f27a28cfcf8736c1dc66b276785110be494657c2e89`  
		Last Modified: Wed, 02 Jun 2021 19:54:02 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab7b072ddd82cd0d29a5e2e73f12df34039e7240f0a6fcf4b5d2cf66053198`  
		Last Modified: Wed, 02 Jun 2021 19:54:02 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
