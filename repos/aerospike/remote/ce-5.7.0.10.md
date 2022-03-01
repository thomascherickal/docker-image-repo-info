## `aerospike:ce-5.7.0.10`

```console
$ docker pull aerospike@sha256:c995b4230882fea4ad9e63645311be950343e74dddc3a8d9c4ff8e2b2ff279ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:fbc8c8cc17c658e54e6dbacc8f47df8d3dfac43f70c667dfa18a0d21ab5d6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81535968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a32924375e58763d0102a041d4d588b5c803f21a8ec3e4787f04431aad2fcc`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:21:32 GMT
ENV AEROSPIKE_VERSION=5.7.0.10
# Tue, 01 Mar 2022 06:22:05 GMT
ENV AEROSPIKE_SHA256=6c17caabf03094c284c28406145447165ce7c40b954427879b8bd38d2824902b
# Tue, 01 Mar 2022 06:22:44 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 01 Mar 2022 06:22:45 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Tue, 01 Mar 2022 06:22:45 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Tue, 01 Mar 2022 06:22:45 GMT
EXPOSE 3000 3001 3002
# Tue, 01 Mar 2022 06:22:45 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 01 Mar 2022 06:22:45 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e59221fc4245686b7910616b36beef839c92170309056c65e03db8d1463a0f`  
		Last Modified: Tue, 01 Mar 2022 06:23:28 GMT  
		Size: 54.4 MB (54380212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e5b54830df18e5ebaa32f7adb78ac43b23edc6211cb603ecaccf0453cc892`  
		Last Modified: Tue, 01 Mar 2022 06:23:18 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ef1e6af8b4775d962623c9157bf982f041be8a049cc1e8ecd9f08a282bef8`  
		Last Modified: Tue, 01 Mar 2022 06:23:18 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
