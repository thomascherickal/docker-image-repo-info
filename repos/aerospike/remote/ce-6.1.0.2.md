## `aerospike:ce-6.1.0.2`

```console
$ docker pull aerospike@sha256:3561232d388e334483c14b00b59b2e312e3c22421e0399f99906c64c858c65c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-6.1.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:a905d0287431acf879baf7c5936ad604675633b0c628a66a998ace4cee834f2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121433313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b9c050fbc5eeabee736b08ffe3f32ac6a448cb364a448f38858206f1102d6a`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:45 GMT
ENV AEROSPIKE_VERSION=6.1.0.2
# Wed, 05 Oct 2022 00:50:26 GMT
ENV AEROSPIKE_SHA256=de37fb05085a0cc4183660bb5df9d9aab8c02039af2eb544102925b11c5c216e
# Wed, 05 Oct 2022 00:50:48 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && if [ -d '/opt/aerospike/bin/asadm' ];   then   mv /opt/aerospike/bin/asadm /usr/lib/;   ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f /usr/lib/asadm/asinfo ];     then     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;     fi   fi   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 05 Oct 2022 00:50:49 GMT
COPY file:f497c4c6974a190f79a562efd9c9c0d6b753efe43e62c3fcc2536f74ad08238d in /etc/aerospike/aerospike.template.conf 
# Wed, 05 Oct 2022 00:50:49 GMT
COPY file:fe302e12e47afe1731a34ed4ed29328c6901a3f2c9e32e307220e65cb76d53a2 in /entrypoint.sh 
# Wed, 05 Oct 2022 00:50:49 GMT
EXPOSE 3000 3001 3002
# Wed, 05 Oct 2022 00:50:49 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bc173a4e130acd734466309e8018f98eacedb26677e919891205bf31d08c81`  
		Last Modified: Wed, 05 Oct 2022 00:51:36 GMT  
		Size: 94.3 MB (94293439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805cf418698d07cefba5d4a4473c87b52d23e93bfb8332895528c7a29cfb19e2`  
		Last Modified: Wed, 05 Oct 2022 00:51:22 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923af1a72283ff2dd7d022bd41c174c7bb5d02a402da3cad73a0b8ccf71668d9`  
		Last Modified: Wed, 05 Oct 2022 00:51:22 GMT  
		Size: 812.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
