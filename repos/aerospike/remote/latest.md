## `aerospike:latest`

```console
$ docker pull aerospike@sha256:d05f574e415f7d932361602c9488f9e97bc4c6610d42417787cf42113f85b542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:fd54b49b20cefbb08a806336c430ee1be782250c1e17c43d3ef585ad5ce129af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51855618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d73b5d3b4d88e188409426736af3ca352e328318ce5af8b796f93c8c6b17de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 02:19:28 GMT
ENV AEROSPIKE_VERSION=4.8.0.1
# Tue, 17 Dec 2019 02:19:28 GMT
ENV AEROSPIKE_SHA256=143aa9bbecf8d2516d5b69f6e559be926f86c7c2dd7d77723a53ded403acb626
# Tue, 17 Dec 2019 02:19:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 17 Dec 2019 02:19:48 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Tue, 17 Dec 2019 02:19:49 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Tue, 17 Dec 2019 02:19:49 GMT
VOLUME [/opt/aerospike/data]
# Tue, 17 Dec 2019 02:19:49 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 17 Dec 2019 02:19:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Dec 2019 02:19:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb98ee112091d68470dba9370e0cb4e99357a79c0798638f3826bc5f6b4e7ca`  
		Last Modified: Tue, 17 Dec 2019 02:20:04 GMT  
		Size: 29.3 MB (29329026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36551a0907f2c163bf7abf2cf101cb1557ae0b716f6ebbeac84a63426ed0d7d9`  
		Last Modified: Tue, 17 Dec 2019 02:19:59 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012968d8f734586006cd193edfce30abcdbf6f367a3680aa4457ea37fe8fd5c8`  
		Last Modified: Tue, 17 Dec 2019 02:19:59 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
