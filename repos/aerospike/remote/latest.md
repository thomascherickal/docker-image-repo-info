## `aerospike:latest`

```console
$ docker pull aerospike@sha256:26759c52a200abe764651368d9b30dc964523ab352742d778b1a16d9126bb7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:6e6a85e72a887f20e643544cbd3797d2b98ade556f54dbf80cdbe81d35c4682d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53095260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92eec4e66e5d02ab57382696dec20617cf0d95d28c3bcc9f0bb7b89e14b7423`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 04:15:54 GMT
ENV AEROSPIKE_VERSION=5.0.0.10
# Wed, 05 Aug 2020 04:15:54 GMT
ENV AEROSPIKE_SHA256=cf56e1dfabf73508491c669a9eaf32b97ddb91863e4bd78cd0cec64bc53fd0ca
# Wed, 05 Aug 2020 04:16:10 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 05 Aug 2020 04:16:10 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 05 Aug 2020 04:16:10 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 05 Aug 2020 04:16:10 GMT
VOLUME [/opt/aerospike/data]
# Wed, 05 Aug 2020 04:16:11 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 05 Aug 2020 04:16:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 04:16:11 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f19d15d65be8f8207093d3b509ec816b41339ac8e8a756b758fb487981bf8b`  
		Last Modified: Wed, 05 Aug 2020 04:16:40 GMT  
		Size: 30.6 MB (30570933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302dea7e17b42295c0cc21dffb520d1c7fb5f4737a70edc61620cbdb0992907`  
		Last Modified: Wed, 05 Aug 2020 04:16:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377de189516cee7a19da3e7538f7e612667702aa252a855ae33461f570993de8`  
		Last Modified: Wed, 05 Aug 2020 04:16:35 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
