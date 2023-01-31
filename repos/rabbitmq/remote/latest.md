## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:8501c659bd79d2be95b108749bde471209f754d32b24772f08a7a2b99bd2f754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `rabbitmq:latest` - linux; amd64

```console
$ docker pull rabbitmq@sha256:b542092a88c107f199c71c6c34b41ff0185902e6172fe8446726cd996a24e50a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101591696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cb9635d301defa5cafbbc09a3e41c41c4aa6730a906c14a4de67d5dc672f15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:49:00 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 20:49:00 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 31 Jan 2023 20:49:01 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 31 Jan 2023 20:49:02 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Jan 2023 20:49:02 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Tue, 31 Jan 2023 20:49:02 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 31 Jan 2023 20:49:02 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Jan 2023 20:49:02 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Jan 2023 20:49:02 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:49:22 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 31 Jan 2023 20:49:23 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 31 Jan 2023 20:49:24 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Jan 2023 20:49:24 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Jan 2023 20:49:24 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Jan 2023 20:49:24 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 20:49:24 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Jan 2023 20:49:24 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 20:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 20:49:24 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Jan 2023 20:49:24 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1280b213aef7cc80e73940a617b0e5fac4acbe4142832c510783b0eaf6dd6621`  
		Last Modified: Tue, 31 Jan 2023 20:51:56 GMT  
		Size: 334.5 KB (334481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3710248cc06487708c6d60c5aef649f035b670c5b518f5aed9b31957647dff8`  
		Last Modified: Tue, 31 Jan 2023 20:51:56 GMT  
		Size: 8.9 KB (8921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e81be32de605ae487c6e04edc9fe355bd6cafb3c18f670ea79e2893b564b6b5`  
		Last Modified: Tue, 31 Jan 2023 20:52:03 GMT  
		Size: 51.1 MB (51108549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6610e44d931fe606a8e2efe2375a845cdc6531ed30deff5aff8daac655bca5dc`  
		Last Modified: Tue, 31 Jan 2023 20:51:56 GMT  
		Size: 5.2 KB (5213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8682ddf02c09027a6510837a7087ef4a9da15de952bca1629422062ef3fbc0c6`  
		Last Modified: Tue, 31 Jan 2023 20:51:57 GMT  
		Size: 21.6 MB (21554935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d592636c2e45f00cf8722b195400be5fec618504f5ac4482867d82150df4e7`  
		Last Modified: Tue, 31 Jan 2023 20:51:54 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81638db5918e47519d6d1112954a0b3f2474396c36048ef1960ed6170a4ff6d`  
		Last Modified: Tue, 31 Jan 2023 20:51:54 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163d89fff8cfd51b97557be461eab292eb9cb8c200e386971435851898c7c560`  
		Last Modified: Tue, 31 Jan 2023 20:51:54 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8776120650a7488d4e1fd5068d423776b6e8fa49559aad7e5e6e9f75c7f858e`  
		Last Modified: Tue, 31 Jan 2023 20:51:54 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:23fd2e49d9650e8f34b06356a6a041f00b9fae7d55c70f93c039b597d94c6cb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86834568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22b5647485275575cf01ef5e57441637a6f839729ce7bf4649d6d19d648bb46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 26 Jan 2023 13:35:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:35:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:35:48 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Thu, 26 Jan 2023 13:35:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:13 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 17:40:13 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 31 Jan 2023 17:40:14 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 31 Jan 2023 17:40:16 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Jan 2023 17:40:16 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Tue, 31 Jan 2023 17:40:16 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 31 Jan 2023 17:40:16 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Jan 2023 17:40:16 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Jan 2023 17:40:16 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:40:36 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 31 Jan 2023 17:40:38 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Jan 2023 17:40:38 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Jan 2023 17:40:38 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Jan 2023 17:40:38 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 17:40:38 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Jan 2023 17:40:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 17:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 17:40:38 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Jan 2023 17:40:38 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830e0a51c17abe28772ee3880ed7dfd375fdad26f43638a2253747c46bba03a1`  
		Last Modified: Tue, 31 Jan 2023 17:44:53 GMT  
		Size: 304.5 KB (304501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60d97f47940cc1aacccb078c229b10facefcd1b746d500b7b3be60843404cad`  
		Last Modified: Tue, 31 Jan 2023 17:44:53 GMT  
		Size: 8.9 KB (8895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a6d9a433eceb02b6f2fb369142a69442ec997c9150bf417a477ec4401733e4`  
		Last Modified: Tue, 31 Jan 2023 17:44:59 GMT  
		Size: 40.8 MB (40796078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6b3f68a01a3ce505e2840b0700b3bdbde554b23d5c5466453f08b4cece895`  
		Last Modified: Tue, 31 Jan 2023 17:44:53 GMT  
		Size: 5.1 KB (5062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8273bc99f7478dfd3dbb66f4d7260b386948d65913c9c8183e366a34d4c9dd05`  
		Last Modified: Tue, 31 Jan 2023 17:44:54 GMT  
		Size: 21.1 MB (21132000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9077fde7f692b24ab18cfb873d4227021052bdc7138b93550a8c5cfaf8cc1cf`  
		Last Modified: Tue, 31 Jan 2023 17:44:51 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7200fd1ef11bd241808ba41b7dd7f48debcf2f75822273b412673e502460f084`  
		Last Modified: Tue, 31 Jan 2023 17:44:51 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523914ec2a99b99984fd0f86b2a3f91ab36afebc1adbd0dafdc3c21654117fa`  
		Last Modified: Tue, 31 Jan 2023 17:44:51 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb7b90fbb81d662549eda18874704b65117c565e68874ff9f0ddd4ce2686f47`  
		Last Modified: Tue, 31 Jan 2023 17:44:51 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4c8aebf04784f034804a2d77f2e02213854a47b173f9080e83750f2fa9bdeb22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98115169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7760997d7932e569a42de67288ecb6eadaf03c1ed1f868e6635893c1c85afb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:10:55 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 20:10:55 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 31 Jan 2023 20:10:55 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 31 Jan 2023 20:10:57 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Jan 2023 20:10:57 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Tue, 31 Jan 2023 20:10:57 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 31 Jan 2023 20:10:57 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Jan 2023 20:10:57 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Jan 2023 20:10:57 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:11:15 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 31 Jan 2023 20:11:16 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 31 Jan 2023 20:11:17 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Jan 2023 20:11:17 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Jan 2023 20:11:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Jan 2023 20:11:17 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 20:11:17 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Jan 2023 20:11:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 20:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 20:11:17 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Jan 2023 20:11:17 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5916593a14ba30637713ca05aabc29add9c80ecd95ed4e91db363ce7c153e4a`  
		Last Modified: Tue, 31 Jan 2023 20:13:32 GMT  
		Size: 324.5 KB (324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96f7edbadcd39fdd6383f9719f0830c18147f3d0a3c4f95e7b8d63245d27c1`  
		Last Modified: Tue, 31 Jan 2023 20:13:32 GMT  
		Size: 8.9 KB (8922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa2a58b4c812e0a7be98ceb9d25b7b65899357281baa6d68413527f458010f`  
		Last Modified: Tue, 31 Jan 2023 20:13:37 GMT  
		Size: 49.2 MB (49203897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be84ba3a134b406a501ea87a07c6c5b9ffffb3143b1955fadf6c39788644fbde`  
		Last Modified: Tue, 31 Jan 2023 20:13:32 GMT  
		Size: 5.2 KB (5198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1efef554ffb1c8e37c65792d347e99caccaac4c8b6c91073243bef6d461bc9d`  
		Last Modified: Tue, 31 Jan 2023 20:13:32 GMT  
		Size: 21.4 MB (21377212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24197715c1ad1b92d8bd24ff531357defd13263c4fe7148915071e00740572c`  
		Last Modified: Tue, 31 Jan 2023 20:13:30 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d1bfd1594aa9ed3a1e50c726deabb61cf43b513e09dbb972dc63cb63d8820d`  
		Last Modified: Tue, 31 Jan 2023 20:13:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1a44efcb3244178c22d6124a6553aacdf7938157da67c1fa408b48d8a27778`  
		Last Modified: Tue, 31 Jan 2023 20:13:30 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213b6b87d6c52ead4cd1039e4bec3ff15fe721f2f9c836e48ff1cf6ad6f92d89`  
		Last Modified: Tue, 31 Jan 2023 20:13:30 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:5601a0aaa2b9f02faa5168332bebfc8701f668664fad5b25c6ae67f8c876be9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.6 MB (98629099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cb79e63334be3925a702265109e7e98459bc057e6ec7b671b25d60c8c2ca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 26 Jan 2023 13:47:16 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:47:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:47:20 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Thu, 26 Jan 2023 13:47:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:33:27 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 19:33:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 31 Jan 2023 19:33:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 31 Jan 2023 19:33:33 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Jan 2023 19:33:33 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Tue, 31 Jan 2023 19:33:33 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 31 Jan 2023 19:33:33 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Jan 2023 19:33:33 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Jan 2023 19:33:33 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 19:34:15 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 31 Jan 2023 19:34:17 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 31 Jan 2023 19:34:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Jan 2023 19:34:18 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Jan 2023 19:34:18 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Jan 2023 19:34:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:34:18 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Jan 2023 19:34:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 19:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 19:34:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Jan 2023 19:34:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5966288f9e48b8f2ddb7447413e5ca78e9cbfd31ebbe23480cbea2d12e9506`  
		Last Modified: Tue, 31 Jan 2023 19:39:41 GMT  
		Size: 357.0 KB (357043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53521fb462ac0dfbb2e549fcd433b1eb2b97309ff75aedae209fb0ce5aaa99b7`  
		Last Modified: Tue, 31 Jan 2023 19:39:41 GMT  
		Size: 8.9 KB (8923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17181d5310b0a75d2527116abcc2f71ceb1de7cf0c5fe3e1d97959bfbf71337`  
		Last Modified: Tue, 31 Jan 2023 19:39:50 GMT  
		Size: 43.3 MB (43256967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252e5aa4f1d4c284f053335d2ddbfbf4bb5be1aeacb07437c7ded1816c426e7b`  
		Last Modified: Tue, 31 Jan 2023 19:39:40 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b1046b22769a95ec349173a9ca86ef52231a1f97c01c17669830f50e3952b`  
		Last Modified: Tue, 31 Jan 2023 19:39:42 GMT  
		Size: 21.7 MB (21698948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fc2de78b030af1d50b4c45fa492206d5be305973c1d880e04941af8d6e04df`  
		Last Modified: Tue, 31 Jan 2023 19:39:39 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223eb5a27f3ec7b9c2e68f24d665383f431da60122f08332a13838ba8801df2`  
		Last Modified: Tue, 31 Jan 2023 19:39:38 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21e311ff30131e0410472d27f4a80a2ac15e5878a4e97aade51c026f42cac5`  
		Last Modified: Tue, 31 Jan 2023 19:39:38 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f81809d10736e9ad5609fa6804e799e5e0d3ab3858e2e443a6f7fb148832385`  
		Last Modified: Tue, 31 Jan 2023 19:39:38 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; riscv64

```console
$ docker pull rabbitmq@sha256:5c1fefaa7078cb17e02045f9ed0a273839d1b62ea38478f5345298d932f87731
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87639678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19d316715ead7ba180d515785e57970f560e2e55901f93743cafabe1b6b0ebf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:10:28 GMT
ADD file:50c1d21a50d57d99470bd427f2ee427504ad0602a5046dbc6a04680574d27f39 in / 
# Fri, 09 Dec 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 08:09:15 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 22 Dec 2022 08:09:15 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Wed, 18 Jan 2023 23:34:27 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Wed, 18 Jan 2023 23:34:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 18 Jan 2023 23:34:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Wed, 18 Jan 2023 23:34:31 GMT
ENV RABBITMQ_VERSION=3.11.7
# Wed, 18 Jan 2023 23:34:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 18 Jan 2023 23:34:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 18 Jan 2023 23:34:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 23:36:24 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Wed, 18 Jan 2023 23:36:32 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Wed, 18 Jan 2023 23:36:33 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 18 Jan 2023 23:36:33 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 18 Jan 2023 23:36:33 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 18 Jan 2023 23:36:33 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 18 Jan 2023 23:36:33 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 18 Jan 2023 23:36:33 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Jan 2023 23:36:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Jan 2023 23:36:33 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 18 Jan 2023 23:36:33 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1bf57572b326faac5012873a6b3ea48eee0fe2649c47d425e34e149459c96c29`  
		Last Modified: Fri, 09 Dec 2022 01:32:24 GMT  
		Size: 24.2 MB (24245212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56afbc2ed5ac23b93e6a2008b4f0dafa0b39ed9884603fc2788ababf4caf3f66`  
		Last Modified: Thu, 22 Dec 2022 08:21:01 GMT  
		Size: 294.7 KB (294716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f7beea575a8ba2d9afc2603d7e4be54a9133e2a090c214eb0d101239d563f`  
		Last Modified: Thu, 22 Dec 2022 08:21:00 GMT  
		Size: 8.9 KB (8893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4d7b6d0755bb5e0b9f8a7f1b34bbbf1462bcf408c5a334b4047f72a97e255c`  
		Last Modified: Wed, 18 Jan 2023 23:46:51 GMT  
		Size: 42.0 MB (41979956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f1db64e0212f0c02c56824a12e739fc634ddfb0d65c308b388428fafa06a94`  
		Last Modified: Wed, 18 Jan 2023 23:46:06 GMT  
		Size: 5.1 KB (5104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a963cd3718f99cb6baacbb9aa924547397ea826b5a96cfdd8089b0632b2c60b7`  
		Last Modified: Wed, 18 Jan 2023 23:46:23 GMT  
		Size: 21.1 MB (21104077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4dacccd121a7c9c7efd21ba4e0493bf252dddc9cc47cadc183c544dfaff010`  
		Last Modified: Wed, 18 Jan 2023 23:46:04 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401f295b8fbfb6c6b2590cd93ea02405d14b9c92b92db5bde4403c314e2745db`  
		Last Modified: Wed, 18 Jan 2023 23:46:04 GMT  
		Size: 105.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdaecd640bbaa37ddfd1a684525c72cec2de01e119227863da0ca5e76481af5`  
		Last Modified: Wed, 18 Jan 2023 23:46:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba59ff57a6571fef033ab1966e1b2742c5650c21a3221ba03a37f4febc510fb`  
		Last Modified: Wed, 18 Jan 2023 23:46:04 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:7ec890f3159beae920da507671d02b3b9efff7fa7d8a874be9dafe3d99b55aea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89901340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6fe98c1f9b93e53b117db73b83da748750417d5ba411ff3b215e161938ef3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 26 Jan 2023 13:21:27 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:21:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:21:29 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Thu, 26 Jan 2023 13:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:33:10 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 18:33:10 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 31 Jan 2023 18:33:12 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 31 Jan 2023 18:33:13 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Jan 2023 18:33:13 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Tue, 31 Jan 2023 18:33:13 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 31 Jan 2023 18:33:13 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Jan 2023 18:33:13 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Jan 2023 18:33:13 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 18:33:27 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 31 Jan 2023 18:33:28 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 31 Jan 2023 18:33:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Jan 2023 18:33:28 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Jan 2023 18:33:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Jan 2023 18:33:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:33:29 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Jan 2023 18:33:29 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Jan 2023 18:33:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 18:33:29 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Jan 2023 18:33:29 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af06a19f51a0814bb90823a394f495b423e4c37c0ee1d431decf6334abc92c1e`  
		Last Modified: Tue, 31 Jan 2023 18:36:52 GMT  
		Size: 337.4 KB (337377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646847f4a9af63d22a0aef18e59e8179122d50f39eb9f73a2b68410be5190f1`  
		Last Modified: Tue, 31 Jan 2023 18:36:52 GMT  
		Size: 8.9 KB (8924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8a600b7ac9a069a9f1cb0716706e52fe0d3479b30e5a80f7e016793f7b5092`  
		Last Modified: Tue, 31 Jan 2023 18:36:57 GMT  
		Size: 41.3 MB (41282388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a6ea6e2f6b11140d0dc0bb0b1da7d9d7fc3850386921c1defc0364ae8481e`  
		Last Modified: Tue, 31 Jan 2023 18:36:52 GMT  
		Size: 5.2 KB (5216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50f3305ba9bf1505f652f1a174cc05577e8ffbd9b7ad703b9e407ffd3194755`  
		Last Modified: Tue, 31 Jan 2023 18:36:52 GMT  
		Size: 21.2 MB (21249592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0259e8ed91f1abc105e2d02f4d86e44eda1c70357612f4d72284656c3e0a34`  
		Last Modified: Tue, 31 Jan 2023 18:36:51 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f83a60d4bba3881a1368b551589172093697d07df1bc5dfd99bbbf545906fbc`  
		Last Modified: Tue, 31 Jan 2023 18:36:50 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30100d717fdc5e850779d47c1024730530aa1fa6c09be26fd5cedf3377803e31`  
		Last Modified: Tue, 31 Jan 2023 18:36:51 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b72a5fd8d95702ffff38707da7c07eec81e7843e6f770e8e5949d7cfd10f8`  
		Last Modified: Tue, 31 Jan 2023 18:36:50 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
