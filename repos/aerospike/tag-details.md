<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-5.7.0.10`](#aerospikece-57010)
-	[`aerospike:ee-5.7.0.10`](#aerospikeee-57010)

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

## `aerospike:ee-5.7.0.10`

```console
$ docker pull aerospike@sha256:5aec8028c82964bc18d27c8d1e590bc1c5b8daa8c88f025711ba4a215055cc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-5.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:d79e49a11f169bde0449c5c3caf206798d034007a7fe5f1975b2de8e009e755d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83906055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59be685cc3338d3553ca293b25888096364acba8ed2ee1f7187c4d933705e9f9`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:21:32 GMT
ENV AEROSPIKE_VERSION=5.7.0.10
# Tue, 01 Mar 2022 06:21:32 GMT
ENV AEROSPIKE_SHA256=736bc5779412088d72a76d95192bfa34e3332fc33357cb5c413a71fbb7ee634c
# Tue, 01 Mar 2022 06:21:32 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Tue, 01 Mar 2022 06:21:57 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian10" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 01 Mar 2022 06:21:57 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Tue, 01 Mar 2022 06:21:58 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Tue, 01 Mar 2022 06:21:58 GMT
EXPOSE 3000 3001 3002
# Tue, 01 Mar 2022 06:21:58 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Tue, 01 Mar 2022 06:21:58 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1edf31ed141e2f8d89220177b0019e39a8e42dc7f52237c9999bc7c71c7bb82`  
		Last Modified: Tue, 01 Mar 2022 06:23:11 GMT  
		Size: 56.8 MB (56750235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac487bfab721d47ba4f987a65aa9e25ab14ff54150aee5cd7060e94191c496f`  
		Last Modified: Tue, 01 Mar 2022 06:23:02 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a2c4771477591292de240c1ddd6370345ad1fc7a87be1eb19c33a0ccf13d8c`  
		Last Modified: Tue, 01 Mar 2022 06:23:02 GMT  
		Size: 908.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
