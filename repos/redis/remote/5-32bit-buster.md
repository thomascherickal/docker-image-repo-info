## `redis:5-32bit-buster`

```console
$ docker pull redis@sha256:39048496a4d6637785b4d511bfe232f382693c976e66d21ae7511de9e03693db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5-32bit-buster` - linux; amd64

```console
$ docker pull redis@sha256:a74dcf2629f0d193dce895766ff01411668fb4e7e2a16ad7d26a757035f5f7fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40509166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9ba9112ac2887abbc1bb7c6546338443a08538862eadb67d9449cf26ed075c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:05:10 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 20:05:10 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 20:05:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Mar 2020 20:20:12 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 20:20:12 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 20:20:12 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 20:22:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 20:22:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 20:22:17 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 20:22:18 GMT
WORKDIR /data
# Fri, 13 Mar 2020 20:22:18 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 13 Mar 2020 20:22:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 20:22:18 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 20:22:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecc253967df63c91c05c830bac2fe70ca6310473427da326667b44fdec3374f`  
		Last Modified: Wed, 26 Feb 2020 20:11:48 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765957bf98d45a3c48bc1565d2cbddfbae12a480404e11a2ad43e0e5c1513a64`  
		Last Modified: Wed, 26 Feb 2020 20:11:49 GMT  
		Size: 1.4 MB (1357665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ad484c6224ddbd8d2917808deb623788fa507484fc4aa96fe0421a2850c136`  
		Last Modified: Fri, 13 Mar 2020 20:24:08 GMT  
		Size: 12.1 MB (12057442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5245b1acda1e394ffff751fb8c685f502f9402f8a77904d14bc15ffe4549a4a4`  
		Last Modified: Fri, 13 Mar 2020 20:24:06 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1452be907218aab38e998ee6fbfd9a58cd3cfedb3f71b6a6298ed95c12170fa4`  
		Last Modified: Fri, 13 Mar 2020 20:24:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
