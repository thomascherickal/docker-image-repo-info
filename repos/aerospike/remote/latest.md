## `aerospike:latest`

```console
$ docker pull aerospike@sha256:b4be51e0c63adafd744a9d826391dddf4705159195c66ea475c2c823357fe0e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:6bef016b10bfa9216b20e10d4ca8d98165e80d9750a833047e3093d99b81fc9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53192493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8f8e8103b496c4e3bfa9fac77a24f88b8cd517e0a835fef10867c8e61e4dbc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:03:01 GMT
ENV AEROSPIKE_VERSION=4.9.0.5
# Fri, 15 May 2020 18:03:01 GMT
ENV AEROSPIKE_SHA256=7e9b345020e987d1a4d1c91034a8054c97fd80a0c917a8da04d4aad9127e8fe2
# Fri, 15 May 2020 18:03:21 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 15 May 2020 18:03:21 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 15 May 2020 18:03:21 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 15 May 2020 18:03:21 GMT
VOLUME [/opt/aerospike/data]
# Fri, 15 May 2020 18:03:21 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 15 May 2020 18:03:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 18:03:22 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6635c0da64586c2b1e638a90a0d5d4eb2891e583df9b880bbf2b9daa1df326`  
		Last Modified: Fri, 15 May 2020 18:03:52 GMT  
		Size: 30.7 MB (30670552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f716638cb00ac61513ec0028c54231b2bb38c0e9e18a45c81b696154aff450b`  
		Last Modified: Fri, 15 May 2020 18:03:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f8805626f93e98e174a35b13b71a3ea96f8c2f53de4784d641cec349b861c9`  
		Last Modified: Fri, 15 May 2020 18:03:47 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
