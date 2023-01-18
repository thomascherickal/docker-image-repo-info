## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:9ead9c171fb462a5bc7e09f730453f5885138fb29d16bbd8b0a2b0e926051e51
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
$ docker pull rabbitmq@sha256:30408fde5a1bc0dc493ce3d509dc395caec33cd5f04e8a518acb663a91a9067f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101566729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d50e14e2eea9f972ebf8d51982cc113dbbe3906102c3d17d1159481a262f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Thu, 15 Dec 2022 01:40:56 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 15 Dec 2022 01:40:56 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 15 Dec 2022 01:40:57 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 15 Dec 2022 01:40:59 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 15 Dec 2022 01:40:59 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 15 Dec 2022 01:40:59 GMT
ENV RABBITMQ_VERSION=3.11.6
# Thu, 15 Dec 2022 01:40:59 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 15 Dec 2022 01:40:59 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 15 Dec 2022 01:40:59 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Jan 2023 18:51:24 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 06 Jan 2023 18:51:25 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Fri, 06 Jan 2023 18:51:26 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 06 Jan 2023 18:51:26 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 06 Jan 2023 18:51:26 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 06 Jan 2023 18:51:26 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 06 Jan 2023 18:51:26 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 06 Jan 2023 18:51:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 06 Jan 2023 18:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 18:51:26 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 06 Jan 2023 18:51:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03dea6b5e70e630bb5bf621528463788e46cf2571f98f3f591e10633f1b650d9`  
		Last Modified: Thu, 15 Dec 2022 01:47:28 GMT  
		Size: 334.5 KB (334487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae1c228689d2f294439828746d67d06536e5cf331393d0529e18ce4c8f222f8`  
		Last Modified: Thu, 15 Dec 2022 01:47:27 GMT  
		Size: 8.9 KB (8919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf939b446499c0937604d712f7e13340db9687e710d61c8b0b278700ba9e38`  
		Last Modified: Thu, 15 Dec 2022 01:47:34 GMT  
		Size: 51.1 MB (51095946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e035229b114a43bd976252b210632f191d41ae606b4eafaf029f0d06c0f454`  
		Last Modified: Thu, 15 Dec 2022 01:47:27 GMT  
		Size: 5.2 KB (5194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e103ef1475feb2f050483aa4216a95752e3c27c02404fcc0a815938da1c0ad`  
		Last Modified: Fri, 06 Jan 2023 18:53:09 GMT  
		Size: 21.5 MB (21543585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0926bc87948c9673fbbee4d4bff60af175dfae14be1b5b8e6a3d0c0037099ef`  
		Last Modified: Fri, 06 Jan 2023 18:53:07 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae105c01998d72f7a495f74a8674275001eb3ee74e232d458dce9091b2706c3`  
		Last Modified: Fri, 06 Jan 2023 18:53:07 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553e1f2f08f51bf343735e0e580955a4c851bd0ba8b2a2f0ed461538e37a15bb`  
		Last Modified: Fri, 06 Jan 2023 18:53:07 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f5869ee28d3f9a1362b44150f944d7f8ea10bb2be4a01f1c9ee635619af4be`  
		Last Modified: Fri, 06 Jan 2023 18:53:07 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:52b3bf5c54230baa00fe085439fd12d19271a31ea0420b8e94367483070fc105
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86824922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4b01f7c12351194d854b1f30dc1c69cbe0ffb83074fd7fdc77803b661cc232`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Thu, 15 Dec 2022 01:46:15 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 15 Dec 2022 01:46:15 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 15 Dec 2022 01:46:16 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 15 Dec 2022 01:46:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 15 Dec 2022 01:46:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 15 Dec 2022 01:46:18 GMT
ENV RABBITMQ_VERSION=3.11.6
# Thu, 15 Dec 2022 01:46:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 15 Dec 2022 01:46:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 15 Dec 2022 01:46:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Jan 2023 23:50:44 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 06 Jan 2023 23:50:45 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Fri, 06 Jan 2023 23:50:45 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 06 Jan 2023 23:50:45 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 06 Jan 2023 23:50:45 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 06 Jan 2023 23:50:45 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 06 Jan 2023 23:50:46 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 06 Jan 2023 23:50:46 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 06 Jan 2023 23:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 23:50:46 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 06 Jan 2023 23:50:46 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5108d8dbd5bda660a4d2c9616714aaf46e46b38bdb6a7959e67e03daf1b5b7`  
		Last Modified: Thu, 15 Dec 2022 01:54:51 GMT  
		Size: 304.5 KB (304499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94b75eed8fbf4ab5a7c1725b6c77b2dc5db3fab5ccb0ca4b4113af0c7c59bb5`  
		Last Modified: Thu, 15 Dec 2022 01:54:51 GMT  
		Size: 8.9 KB (8896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4eb18c6b8daf31ab3cbfb7d28611899c817539640bd3f523195870dad7a4540`  
		Last Modified: Thu, 15 Dec 2022 01:54:57 GMT  
		Size: 40.8 MB (40796610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c9ae9f66491966b6ea4faa6caee52e6ad508a9d29e23d6f5e6c78c777b907`  
		Last Modified: Thu, 15 Dec 2022 01:54:51 GMT  
		Size: 5.1 KB (5113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe78f510683996f7a6dba03f050653a05c50a393122abf47aa5e7034c29050f`  
		Last Modified: Fri, 06 Jan 2023 23:54:06 GMT  
		Size: 21.1 MB (21119087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bea6aef213b707c3658c0427c09fbcba7dd64ec7bcac541041dc998378cffe`  
		Last Modified: Fri, 06 Jan 2023 23:54:03 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d017d2baf0f403016de8a06a399a739c9ced2fcf9b9494b8d2951490039a82d9`  
		Last Modified: Fri, 06 Jan 2023 23:54:03 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7dd4f5087e1c3d2d3633defbb0b5c586bb7f539028d681221cca3980e29a84`  
		Last Modified: Fri, 06 Jan 2023 23:54:03 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c00320a1f32571cf308287caec598dc0ddec9416be7193674344b5bd47eddf3`  
		Last Modified: Fri, 06 Jan 2023 23:54:03 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:2f7b5b7839b68e6a46a3f990ab263bb4ecf8dddc04ae046d9e1ed1762ead65da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98101605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a090c74a4b1c5d1a80e3c98f91e72f9e5768d8eb57bbdfba7822b509e67da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Thu, 15 Dec 2022 00:49:39 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 15 Dec 2022 00:49:39 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 15 Dec 2022 00:49:39 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 15 Dec 2022 00:49:41 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 15 Dec 2022 00:49:41 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 15 Dec 2022 00:49:41 GMT
ENV RABBITMQ_VERSION=3.11.6
# Thu, 15 Dec 2022 00:49:41 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 15 Dec 2022 00:49:41 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 15 Dec 2022 00:49:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Jan 2023 21:02:45 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 06 Jan 2023 21:02:46 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Fri, 06 Jan 2023 21:02:46 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 06 Jan 2023 21:02:46 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 06 Jan 2023 21:02:46 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 06 Jan 2023 21:02:46 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 06 Jan 2023 21:02:46 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 06 Jan 2023 21:02:46 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 06 Jan 2023 21:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 21:02:46 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 06 Jan 2023 21:02:46 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d3908a4d8db89c8e5b3a40a7e124528b26044e788f2f78ce6d83ed2befe39`  
		Last Modified: Thu, 15 Dec 2022 00:55:03 GMT  
		Size: 324.5 KB (324487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11fe054472c647f1e263e236c691308a2b25ff50737252bba6375da38112ea`  
		Last Modified: Thu, 15 Dec 2022 00:55:02 GMT  
		Size: 8.9 KB (8918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb319727920fffa4c5edec118cc051f71ac52b30f93d04171fe4c4d5919691a`  
		Last Modified: Thu, 15 Dec 2022 00:55:08 GMT  
		Size: 49.2 MB (49202064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5988893227e2b5177f9bc07963a30331d3686eab1b8c2d0e5702e7b0c7a880`  
		Last Modified: Thu, 15 Dec 2022 00:55:02 GMT  
		Size: 5.2 KB (5188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc2f0d4c2eafd335ab37eb114fb4d65b16a88472df658a1a11ca1292ca514c`  
		Last Modified: Fri, 06 Jan 2023 21:04:30 GMT  
		Size: 21.4 MB (21366069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372f057fe9095f155ff05a4b96a7df37b8d679e808312a1660ba746d18cff54e`  
		Last Modified: Fri, 06 Jan 2023 21:04:28 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973befbda78fc021b1ac3cea240e11b39f5474306b553ebc68e9838af3c69b78`  
		Last Modified: Fri, 06 Jan 2023 21:04:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948e1a72872def38143533dba37e0f5c93647736cb3b789ea8e40bc76d51e80e`  
		Last Modified: Fri, 06 Jan 2023 21:04:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd23c344c8741e80bd10abcd13d9b0e2f6287c73598e9b05535b4d29e577b30f`  
		Last Modified: Fri, 06 Jan 2023 21:04:28 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:0892369cf67f306ef127b6d9ef57f80cf5aae7cb636f5872aa8a2697a052db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.6 MB (98613144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095471f673ae56566946cb1f58d857d84a961e7ba0b85dd4f6da3f385644c654`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 15 Dec 2022 01:53:24 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 15 Dec 2022 01:53:24 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 15 Dec 2022 01:53:26 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 15 Dec 2022 01:53:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 15 Dec 2022 01:53:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 15 Dec 2022 01:53:28 GMT
ENV RABBITMQ_VERSION=3.11.6
# Thu, 15 Dec 2022 01:53:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 15 Dec 2022 01:53:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 15 Dec 2022 01:53:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Jan 2023 21:02:58 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 06 Jan 2023 21:03:01 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Fri, 06 Jan 2023 21:03:01 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 06 Jan 2023 21:03:01 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 06 Jan 2023 21:03:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 06 Jan 2023 21:03:01 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 06 Jan 2023 21:03:02 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 06 Jan 2023 21:03:02 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 06 Jan 2023 21:03:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 21:03:02 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 06 Jan 2023 21:03:02 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7aba749720c8d26ce56d5d4943541588f52a73dad782e2b4c9f724a2a488ed`  
		Last Modified: Thu, 15 Dec 2022 02:04:44 GMT  
		Size: 357.0 KB (357044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d9fa36507825661d84e2a797042a70dbbf142de18138a57ce494c1c73ab93`  
		Last Modified: Thu, 15 Dec 2022 02:04:44 GMT  
		Size: 8.9 KB (8920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9358c998c8615127db432d1a6881bb327dbe5dd0f32e8cd7d48baff43b2c1a`  
		Last Modified: Thu, 15 Dec 2022 02:04:53 GMT  
		Size: 43.3 MB (43254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e20ac7d2ebdabbb0c3a74a001bbb79a9e76ad47dd33da3f4d8a961a62a9ac0`  
		Last Modified: Thu, 15 Dec 2022 02:04:44 GMT  
		Size: 5.2 KB (5150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396534117edeed106db104e9dc0e084afe6bda72c3b46408d3fddeb1688e1ed8`  
		Last Modified: Fri, 06 Jan 2023 21:06:29 GMT  
		Size: 21.7 MB (21686669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e0d34677c3897c173b5602c25281d454a7c6e4e73d2c5ac4873462b15fd544`  
		Last Modified: Fri, 06 Jan 2023 21:06:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e055ddec4e24dc6e485071fdb943b4ea0e32190c82514ddf95f3b51af1ef19df`  
		Last Modified: Fri, 06 Jan 2023 21:06:25 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f273508d4efbf5f9cc10cc90ef79eb6a39ecda67efe64cf50a9172906dc2bbd`  
		Last Modified: Fri, 06 Jan 2023 21:06:25 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40087c0280cc64b870421374a9414c33d929c43f3dfb6d05c242ca137dda5cff`  
		Last Modified: Fri, 06 Jan 2023 21:06:25 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; riscv64

```console
$ docker pull rabbitmq@sha256:cae038b281dea0bebfe334f0445667c4dca6fa697bfb2b71edf8e1e605b80f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87634872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:214b15733532082c5f3a055d1934c36e28270fa86593061b0e2a3873274f4f0c`
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
# Thu, 22 Dec 2022 08:09:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 22 Dec 2022 08:09:22 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 22 Dec 2022 08:09:22 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 22 Dec 2022 08:09:22 GMT
ENV RABBITMQ_VERSION=3.11.7
# Thu, 22 Dec 2022 08:09:22 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 22 Dec 2022 08:09:22 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 22 Dec 2022 08:09:22 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Jan 2023 22:10:41 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 17 Jan 2023 22:10:49 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 17 Jan 2023 22:10:50 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 17 Jan 2023 22:10:50 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 17 Jan 2023 22:10:50 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 17 Jan 2023 22:10:50 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 17 Jan 2023 22:10:50 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 17 Jan 2023 22:10:50 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 17 Jan 2023 22:10:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 22:10:50 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 17 Jan 2023 22:10:50 GMT
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
	-	`sha256:979c7f6d4cab95a9242dba85e998de9b1a793289e5fa5f7644ed108e0c6139d0`  
		Last Modified: Thu, 22 Dec 2022 08:21:46 GMT  
		Size: 42.0 MB (41975083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80e1f0af775fc7b4a9e25d4a91a486fdbfd4c531a3575104843629b6ac6d948`  
		Last Modified: Thu, 22 Dec 2022 08:21:00 GMT  
		Size: 5.1 KB (5096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b1a729ee25ab91e47db7d527743dffde82a5f4dcbc6e928f324e2cf94d4743`  
		Last Modified: Tue, 17 Jan 2023 22:16:43 GMT  
		Size: 21.1 MB (21104154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cca80a66aa0176e8142c83e0586a018903194a116c3059315eb2a353a32a220`  
		Last Modified: Tue, 17 Jan 2023 22:16:27 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73483f2953215785fad998507eab05d70f1ecf2f3c846ce445e37b3c0a2ea60`  
		Last Modified: Tue, 17 Jan 2023 22:16:27 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e560640a6002b4501a799fdd835724a9e1c000a5934d7aaa6adb4ace09cea07`  
		Last Modified: Tue, 17 Jan 2023 22:16:27 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ff8e23bfe1a5e7bcc35cc40bff0c584ec1390c6a8b6434b3ef5a281566b572`  
		Last Modified: Tue, 17 Jan 2023 22:16:27 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:8608215be25508b145c927c57e27b5a909787949ff8b8496e85d46c3df75f62b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89898178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733ca650e74e55cbb1f26c1c3269f00806c31ad5202d276391e09ad75da93748`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:52:40 GMT
ADD file:3d26982d2188d52ed2423587d3d2597c1f8ff614c19408d892cadc91d3743deb in / 
# Fri, 09 Dec 2022 01:52:43 GMT
CMD ["bash"]
# Thu, 15 Dec 2022 00:48:27 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 15 Dec 2022 00:48:27 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 15 Dec 2022 00:48:33 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 15 Dec 2022 00:48:36 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 15 Dec 2022 00:48:36 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 15 Dec 2022 00:48:36 GMT
ENV RABBITMQ_VERSION=3.11.7
# Thu, 15 Dec 2022 00:48:36 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 15 Dec 2022 00:48:36 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 15 Dec 2022 00:48:36 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 01:41:54 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Wed, 18 Jan 2023 01:41:55 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Wed, 18 Jan 2023 01:41:55 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 18 Jan 2023 01:41:55 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 18 Jan 2023 01:41:55 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 18 Jan 2023 01:41:55 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 18 Jan 2023 01:41:55 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 18 Jan 2023 01:41:55 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Jan 2023 01:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Jan 2023 01:41:55 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 18 Jan 2023 01:41:55 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:5d330d9ae4f68425a719ebb93a3911994ee56b1328cf256fc3c44a4050de22ec`  
		Last Modified: Fri, 09 Dec 2022 01:54:57 GMT  
		Size: 27.0 MB (27016083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a529f1fbb4239c1804b3d39df9c5d1d872d7107f732c98c998abb750c41cd7`  
		Last Modified: Thu, 15 Dec 2022 01:04:41 GMT  
		Size: 337.4 KB (337377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cafd6a5f553fa7a2813fa7ad6527d38d8a14be41c722d434df353d3cd14185`  
		Last Modified: Thu, 15 Dec 2022 01:04:40 GMT  
		Size: 8.9 KB (8928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d5db3774691ca19ce69de07b636cca8c5a476b9891b8ee13a8f92270761984`  
		Last Modified: Thu, 15 Dec 2022 01:04:45 GMT  
		Size: 41.3 MB (41279140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98357a769f92735b9443b00f2effb7a06aa253f1445c921a7ab9e06774dfdbd7`  
		Last Modified: Thu, 15 Dec 2022 01:04:40 GMT  
		Size: 5.2 KB (5224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9deb1a493204921dc2df3ce321a81891bb3f653f83ea442a49f8e8b98efe306`  
		Last Modified: Wed, 18 Jan 2023 01:45:39 GMT  
		Size: 21.2 MB (21249715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c837830219d03b6c3850277300bd8577969d380030c0a058629e7ddd41d1058`  
		Last Modified: Wed, 18 Jan 2023 01:45:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760edea05b26375152fc5ae4ccc3cb65cbe1330febbf85be43a65b5149c756a3`  
		Last Modified: Wed, 18 Jan 2023 01:45:38 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3868fc1a09f85c2982c111ea61c9d31c902e467d85194b3c9b5df8a2c2e50e11`  
		Last Modified: Wed, 18 Jan 2023 01:45:37 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a00dea01631252a6a1580e4c1adf2824989fff13ede2fdcb01b141898ca59b`  
		Last Modified: Wed, 18 Jan 2023 01:45:38 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
