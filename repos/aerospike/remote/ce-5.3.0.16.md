## `aerospike:ce-5.3.0.16`

```console
$ docker pull aerospike@sha256:31d0b435f604314e813d3c1c358cfaeb975e63f1d75877a9d350a1189d1b00fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.3.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:54ba99197625876811032132491f124cdbd88fe689e6235d6835d9142fb507c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374ba444a1b3ec957ee2608e5985d6292add7085c6ae0b61ce0a65624d75b12d`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:19:28 GMT
ENV AEROSPIKE_VERSION=5.3.0.16
# Thu, 15 Apr 2021 18:19:28 GMT
ENV AEROSPIKE_SHA256=9bcda09cf0c1570747a6d97e3de8a550b31ff6cd74700200a75539323229055d
# Thu, 15 Apr 2021 18:19:47 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:19:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:19:48 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 15 Apr 2021 18:19:48 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 15 Apr 2021 18:19:48 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:19:48 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bb83ed23bcfdefed052088c8db7e6cbd6387821567064ae65f7f3e4413e971`  
		Last Modified: Thu, 15 Apr 2021 18:21:22 GMT  
		Size: 52.2 MB (52179721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757c3c868f609ab9eec1cff3d0914ca3bcd62fc81a769aa361354790fc74cb98`  
		Last Modified: Thu, 15 Apr 2021 18:21:12 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436545266fab697fa5d2dd629f9425e5512d85a9a5c51f94c0e7666e181e264`  
		Last Modified: Thu, 15 Apr 2021 18:21:13 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
