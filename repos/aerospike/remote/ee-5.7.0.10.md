## `aerospike:ee-5.7.0.10`

```console
$ docker pull aerospike@sha256:c0f957f4c1ef28e5236f8c45243e5e8761dd5efb22342e6f2d67a1d5e9000365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-5.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:965873c5d357fc9afdcf4fe44a065cad6485f91db633536eeca7b9e2dac64d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83903958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92d1ce5398509ae068d58d9269b2b62c0af4b264e28e6bf27800d06d7e1600e8`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 25 Jan 2022 20:19:22 GMT
ENV AEROSPIKE_VERSION=5.7.0.10
# Tue, 25 Jan 2022 20:19:22 GMT
ENV AEROSPIKE_SHA256=736bc5779412088d72a76d95192bfa34e3332fc33357cb5c413a71fbb7ee634c
# Tue, 25 Jan 2022 20:19:23 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Tue, 25 Jan 2022 20:19:45 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian10" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 25 Jan 2022 20:19:46 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Tue, 25 Jan 2022 20:19:46 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Tue, 25 Jan 2022 20:19:46 GMT
EXPOSE 3000 3001 3002
# Tue, 25 Jan 2022 20:19:47 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Tue, 25 Jan 2022 20:19:47 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a2f82829f08b9379ccbd304c8c48133d03e5a74b7265bdef3f441bec044c72`  
		Last Modified: Tue, 25 Jan 2022 20:20:27 GMT  
		Size: 56.7 MB (56748155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bd07a36fa2713cf512af2e84a8213f03017750a05787279e6265bcfffbb59f`  
		Last Modified: Tue, 25 Jan 2022 20:20:18 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476dd022ebc73a1d5d3e1378a7035fbcac206fd0e1527430f8d26880436b088`  
		Last Modified: Tue, 25 Jan 2022 20:20:18 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
