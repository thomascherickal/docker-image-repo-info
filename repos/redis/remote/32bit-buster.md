## `redis:32bit-buster`

```console
$ docker pull redis@sha256:13c716e84115f92f4394ed73575211f9c064581b0e451accc7f980c855fbf1d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:32bit-buster` - linux; amd64

```console
$ docker pull redis@sha256:c2f2971a1b0af017a9e856e5567485763582f75633a201dbc145a5fb3e3b0632
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c232b9390b07694edea5489efab33721244dc6025b02e6fbcefbd19ca63ba59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:53:59 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 20:53:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 20:54:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 20 Apr 2020 18:34:56 GMT
ENV REDIS_VERSION=5.0.9
# Mon, 20 Apr 2020 18:34:56 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Mon, 20 Apr 2020 18:34:56 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Mon, 20 Apr 2020 18:37:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:37:36 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:37:36 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:37:37 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:37:37 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:37:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:37:38 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:37:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2edbd6a658e04d559c1bec36d838006bbdcb39d8fb9033ed43d2014ac497774`  
		Last Modified: Thu, 16 Apr 2020 21:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66960bede47c1a193710cf8bfa7bf5f50bc46374260923df1db1c423b52153ac`  
		Last Modified: Thu, 16 Apr 2020 21:01:17 GMT  
		Size: 1.4 MB (1417708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7219d5ce53476cfbbf65dde53db3412640f42a5bb7296653554bd7f63d993a3`  
		Last Modified: Mon, 20 Apr 2020 18:40:11 GMT  
		Size: 12.1 MB (12058716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd99af16cdb23d8383d8a25a8aebbb281cc710f2051637f5d045bbce9f786b`  
		Last Modified: Mon, 20 Apr 2020 18:40:09 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d7ff0575ff0c891bf00497177ffcaf92a9a2dd8b683e95e13196cb97ace6f`  
		Last Modified: Mon, 20 Apr 2020 18:40:09 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
