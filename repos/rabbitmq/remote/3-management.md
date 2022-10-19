## `rabbitmq:3-management`

```console
$ docker pull rabbitmq@sha256:651a75a973e2c1fcd8b52f6ca62c00a8a1eb16b3befcd6a2a5bd571518c19ddf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `rabbitmq:3-management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:72a686d14b4869a1c02fa8675a711a99b64ae894258b0f135b2d0e5bf7972985
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112296411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bf31c8c3a661976ecdd3e3d2afd2f41a3ac674ca6b4dbf395546654d513e0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 05 Oct 2022 18:12:50 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Wed, 05 Oct 2022 18:12:50 GMT
ENV OPENSSL_VERSION=1.1.1q
# Wed, 05 Oct 2022 18:12:50 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Wed, 05 Oct 2022 18:12:50 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 05 Oct 2022 18:12:50 GMT
ENV OTP_VERSION=25.1.1
# Wed, 05 Oct 2022 18:12:50 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Wed, 05 Oct 2022 18:15:37 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 05 Oct 2022 18:15:37 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 05 Oct 2022 18:15:38 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:43:25 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:43:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:43:26 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:43:26 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:43:58 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:43:59 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:44:00 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:44:00 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:44:00 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:44:00 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:44:00 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:44:00 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:44:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:44:01 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:44:01 GMT
CMD ["rabbitmq-server"]
# Wed, 19 Oct 2022 19:44:16 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 19 Oct 2022 19:44:17 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e2bc6e42dd8cae2e15fdc84b9a3e4426b6fd9676af58de6ae74cbeeb4c042`  
		Last Modified: Wed, 05 Oct 2022 18:18:18 GMT  
		Size: 1.8 MB (1835258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498446f2734401912c65f63cca1079f22fb3eb7df29200167087616db3b61903`  
		Last Modified: Wed, 05 Oct 2022 18:18:24 GMT  
		Size: 52.3 MB (52297797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2df5a4d5834deee0bdc7dd20a32106ac9468a9539d1b117129a822b64e02f18`  
		Last Modified: Wed, 05 Oct 2022 18:18:17 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f5c0e8e195b2a9feb5e7ec22ddd6794d48081e4431e864d4b0105721d9682c`  
		Last Modified: Wed, 19 Oct 2022 19:45:31 GMT  
		Size: 17.8 MB (17816327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db28f47907212919b4f44c78b45a336c639e0a2fb92105a679ba46cebe0db0fb`  
		Last Modified: Wed, 19 Oct 2022 19:45:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36717f610fb93cd871ef3a6d7873e46834aac6fd863cf3c601565d7ca1186715`  
		Last Modified: Wed, 19 Oct 2022 19:45:29 GMT  
		Size: 105.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f5e82aad6145c1b2354ddca76e926a846de4addbb50131e2366c5b6c1da4ca`  
		Last Modified: Wed, 19 Oct 2022 19:45:29 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b48fbb7f5e223aad61109a502b0a295aa471e1335f50635872898d40e03805`  
		Last Modified: Wed, 19 Oct 2022 19:45:30 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd909d5624be938a564ea696a77b504c65ffb8827849e98a78894f2de36ba6c`  
		Last Modified: Wed, 19 Oct 2022 19:45:49 GMT  
		Size: 11.8 MB (11768785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:24e3cbb5be6be401fb021206cd4fe5bdf67278bc7aeb8636ee4e24b42462890b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96809862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44aea54916f0639176b97fa37ce9ed299493e10bb29eb4a01820126e093c6a55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Thu, 06 Oct 2022 06:19:05 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Thu, 06 Oct 2022 06:19:05 GMT
ENV OPENSSL_VERSION=1.1.1q
# Thu, 06 Oct 2022 06:19:05 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Thu, 06 Oct 2022 06:19:05 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Thu, 06 Oct 2022 06:19:05 GMT
ENV OTP_VERSION=25.1.1
# Thu, 06 Oct 2022 06:19:05 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Thu, 06 Oct 2022 06:23:12 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Thu, 06 Oct 2022 06:23:12 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 06 Oct 2022 06:23:13 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:20:39 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:20:39 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:20:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:20:39 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:21:01 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:21:02 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:21:02 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:21:02 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:21:02 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:21:03 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:21:03 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:21:03 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:21:03 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:21:03 GMT
CMD ["rabbitmq-server"]
# Wed, 19 Oct 2022 20:21:21 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 19 Oct 2022 20:21:21 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45bf03615d76b91ebf489a4f939e61df06c5c598875ca91f0537b5bf03d8609`  
		Last Modified: Thu, 06 Oct 2022 06:27:47 GMT  
		Size: 1.8 MB (1802763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3551e0da5f4892df31b8fff3b46285c0a2fd5a29af2fd6c154d127c443c9a390`  
		Last Modified: Thu, 06 Oct 2022 06:27:53 GMT  
		Size: 42.0 MB (41962452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f69d56cbe26f0ec79ec43ecd67dc3aba0d81245f4b48392de31897a5997e20`  
		Last Modified: Thu, 06 Oct 2022 06:27:47 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833f09667428bd06f8f63dd8f89cca6058e9834340f2aeee19813a8324cf06f`  
		Last Modified: Wed, 19 Oct 2022 20:23:41 GMT  
		Size: 17.8 MB (17815914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c83b7b736749c2a5a7ef22afea3825c73d74f608eb49f75b8cf079512b094`  
		Last Modified: Wed, 19 Oct 2022 20:23:39 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eae828ab49f0e56646e1c242dcab3d2d0d8dfc93a9f7ba0f10f073c7c20e18c`  
		Last Modified: Wed, 19 Oct 2022 20:23:39 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1711b164c920c85b98a6fc42ed37bc79c4aa7e43d9726808646bcdc8ef82de2f`  
		Last Modified: Wed, 19 Oct 2022 20:23:39 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44578a8459e70f731f5262a3de00a38f18d081afe68a2c30dda37e1bd41bae1`  
		Last Modified: Wed, 19 Oct 2022 20:23:39 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b3133a4c79ff43027c4c7e59c7ce475d54f53d78610063e1cf21ac948e3e5`  
		Last Modified: Wed, 19 Oct 2022 20:24:02 GMT  
		Size: 10.6 MB (10634857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:b09f720b0f24b19e1f54783f0b19f763b0692567d0056f7b72896fc57b864471
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.9 MB (108936603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798727551589f668dd8bb279dfbbbcd5ab7d15c17b9907ddc9e79df2320556bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 05 Oct 2022 16:19:44 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Wed, 05 Oct 2022 16:19:45 GMT
ENV OPENSSL_VERSION=1.1.1q
# Wed, 05 Oct 2022 16:19:46 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Wed, 05 Oct 2022 16:19:47 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 05 Oct 2022 16:19:48 GMT
ENV OTP_VERSION=25.1.1
# Wed, 05 Oct 2022 16:19:49 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Wed, 05 Oct 2022 16:22:18 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 05 Oct 2022 16:22:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 05 Oct 2022 16:22:20 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:08:17 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:08:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:08:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:08:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:08:43 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:08:45 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:08:46 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:08:47 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:08:48 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:08:49 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:08:51 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:08:52 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:08:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:08:53 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:08:54 GMT
CMD ["rabbitmq-server"]
# Wed, 19 Oct 2022 20:09:12 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 19 Oct 2022 20:09:12 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce086b7568508612079145c1b835092b564b94d074e3f8bb09355f27ff54e57`  
		Last Modified: Wed, 05 Oct 2022 16:26:50 GMT  
		Size: 1.8 MB (1796166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6040e30044116ed2eedbcb6d8d22e7da6ca829b3fc8a6b140bb16ca168a7a622`  
		Last Modified: Wed, 05 Oct 2022 16:26:56 GMT  
		Size: 50.4 MB (50401788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925bd950d539b6864533c7331392b23376aee26b650b9cbbdb1ad6b679708c9`  
		Last Modified: Wed, 05 Oct 2022 16:26:49 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b88048f440317aeee3b91c5f0cc855c157ee7210db1300a3ccd94fb56260253`  
		Last Modified: Wed, 19 Oct 2022 20:11:30 GMT  
		Size: 17.8 MB (17815581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff53f5c6c8c0984703763b05dbcb98d5527b4b4c340d7ea8e200e1a2e8c2d53`  
		Last Modified: Wed, 19 Oct 2022 20:11:28 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18130a93ef608bd65ce1c9a4f522caabe2f615254c4f9d9745bb63f9bddb8e`  
		Last Modified: Wed, 19 Oct 2022 20:11:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364fe244b38075bb0afa9a8805da3b12b7aa3c05e352d41cb1699059ab1c4550`  
		Last Modified: Wed, 19 Oct 2022 20:11:28 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7e797bc984d65794b202ad97b993c2bf4924aab4243b080773771e2a152131`  
		Last Modified: Wed, 19 Oct 2022 20:11:28 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe99e03d1d18ce34fd65d5ca1b76713a89a8749dd461d789416d0b45b38cf5`  
		Last Modified: Wed, 19 Oct 2022 20:11:50 GMT  
		Size: 11.7 MB (11727767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:341c78ed528f268bcab35a864d464074a364052a4e2340d85eff5e6801370a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110085904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884efceac7c14537e7ef03e19c459b5af7db3bb9737a7e560bdb9324c6ad3f04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:08 GMT
ADD file:75224b75d955b3021df8214497d6835e1aff42b5ce83f96b779b63c4a8e15faf in / 
# Wed, 05 Oct 2022 10:52:10 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 20:19:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 05 Oct 2022 20:19:29 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Wed, 05 Oct 2022 20:19:30 GMT
ENV OPENSSL_VERSION=1.1.1q
# Wed, 05 Oct 2022 20:19:30 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Wed, 05 Oct 2022 20:19:30 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 05 Oct 2022 20:19:31 GMT
ENV OTP_VERSION=25.1.1
# Wed, 05 Oct 2022 20:19:31 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Wed, 05 Oct 2022 20:23:07 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 05 Oct 2022 20:23:09 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 05 Oct 2022 20:23:10 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:39:28 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:39:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:39:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:39:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:40:17 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:40:21 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:40:23 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:40:24 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:40:24 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:40:24 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:40:25 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:40:25 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:40:26 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:40:26 GMT
CMD ["rabbitmq-server"]
# Wed, 19 Oct 2022 19:41:00 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 19 Oct 2022 19:41:01 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:ecaa0fe591301d50850e37b61a6fac5429c04a3c39272da2f7b748eaed7f5c52`  
		Last Modified: Wed, 05 Oct 2022 10:54:26 GMT  
		Size: 33.3 MB (33296076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504edef3f0896a22a2bb8e7c27d6d025230afed12bb674b55b126f3521ec2bf6`  
		Last Modified: Wed, 05 Oct 2022 20:28:27 GMT  
		Size: 1.8 MB (1786819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab76214a26ee1bc948d210f5af359152520aec1a43592800001b03a3f8831bf`  
		Last Modified: Wed, 05 Oct 2022 20:28:36 GMT  
		Size: 44.5 MB (44471206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf915c9889d07c1f6432cd5b3ab02357f9029ae518818973c5bfb34d12e78ee`  
		Last Modified: Wed, 05 Oct 2022 20:28:27 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951eebd79214c3786f28efc89314a7f1f496ac00dee525cd64b7a678b571b1cb`  
		Last Modified: Wed, 19 Oct 2022 19:43:34 GMT  
		Size: 17.8 MB (17816874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c877ddf72b0010e8f9437904e3ebe73e206b82ddaccae592ddac5d5909abd00`  
		Last Modified: Wed, 19 Oct 2022 19:43:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4cb601b8887e7b4a3dab5459dd849e5e6c6d7eef5d34cae60b2682364a76bc`  
		Last Modified: Wed, 19 Oct 2022 19:43:32 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea066c11939684dfa18ac2187c59b5dc1e02b55ba6570682cba08e78ebb49c`  
		Last Modified: Wed, 19 Oct 2022 19:43:32 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e2c232bdeb113e9d6adda569aa5131b6359f4d0c5716ff57015b03ebf1d14`  
		Last Modified: Wed, 19 Oct 2022 19:43:32 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fe17878204cc67d4be392acde2fd35449f40c1d6d7b5afa16b0ee13c23c941`  
		Last Modified: Wed, 19 Oct 2022 19:43:57 GMT  
		Size: 12.7 MB (12711131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; riscv64

```console
$ docker pull rabbitmq@sha256:46eb453ec768b5f1f35ce07a6087cd1b35224ee097ad31fd9674a6245aab46c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97430275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1808993c8d3f1fc8fdce6dd01a53a5723c424d50c08ae41d33e6159134fcd2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:13 GMT
ADD file:8c408c11e1eeed71fdd784404ddf9ac52b700161e6187e2313c2751d756e3442 in / 
# Wed, 05 Oct 2022 00:12:14 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 05 Oct 2022 01:09:13 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Wed, 05 Oct 2022 01:09:13 GMT
ENV OPENSSL_VERSION=1.1.1q
# Wed, 05 Oct 2022 01:09:14 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Wed, 05 Oct 2022 01:09:14 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 05 Oct 2022 01:09:15 GMT
ENV OTP_VERSION=25.1.1
# Wed, 05 Oct 2022 01:09:15 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Wed, 05 Oct 2022 01:35:08 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 05 Oct 2022 01:35:10 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 05 Oct 2022 01:35:12 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Thu, 13 Oct 2022 21:12:15 GMT
ENV RABBITMQ_VERSION=3.11.1
# Thu, 13 Oct 2022 21:12:16 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 13 Oct 2022 21:12:16 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 13 Oct 2022 21:12:17 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Oct 2022 21:13:54 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Thu, 13 Oct 2022 21:14:04 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Thu, 13 Oct 2022 21:14:07 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Thu, 13 Oct 2022 21:14:07 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 13 Oct 2022 21:14:08 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 13 Oct 2022 21:14:08 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 13 Oct 2022 21:14:09 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Thu, 13 Oct 2022 21:14:10 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Thu, 13 Oct 2022 21:14:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 Oct 2022 21:14:11 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Thu, 13 Oct 2022 21:14:11 GMT
CMD ["rabbitmq-server"]
# Thu, 13 Oct 2022 21:17:39 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Thu, 13 Oct 2022 21:17:40 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:edcdeceb0859700b9f2e87516c30c0049092e29666696c30e6b862e0df3d4961`  
		Last Modified: Wed, 05 Oct 2022 00:29:16 GMT  
		Size: 24.2 MB (24242839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b3c1978e4e7c203421dddc0ea41f295d3b38c4d4e064894fbe0c8ffe96ed2b`  
		Last Modified: Wed, 05 Oct 2022 02:09:23 GMT  
		Size: 1.9 MB (1895001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2147c2bdad96f5daf46cd1ebfc2acdfc0733bea94a1ad74ec1470961dd29b`  
		Last Modified: Wed, 05 Oct 2022 02:10:17 GMT  
		Size: 43.1 MB (43134391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fcd08d874216563591cce56433571ed306be87bc6c8824de04eeaf6edc18c`  
		Last Modified: Wed, 05 Oct 2022 02:09:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8522a6062d8fc075066d65516f17f08b624018cf2680a09f8a001136ad896f67`  
		Last Modified: Thu, 13 Oct 2022 21:43:11 GMT  
		Size: 17.8 MB (17817668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453311d571c965108e487315fdfba38d677d0de9f3e0966b1c7b755d4a7af3f8`  
		Last Modified: Thu, 13 Oct 2022 21:42:55 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1485c0c2169f6787f2e59726d06fd8172148cb4c49e3066f1c9d1e590ce4ae`  
		Last Modified: Thu, 13 Oct 2022 21:42:55 GMT  
		Size: 105.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fb15a64604fbdd67eefdf8a12466a674f8f84c8e886cc16e0b1112751ceae0`  
		Last Modified: Thu, 13 Oct 2022 21:42:55 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd3e804832a04a730bd27b37a8a5bc48eedda9e456ced5e54e5df323ce17ccc`  
		Last Modified: Thu, 13 Oct 2022 21:42:55 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af30d1d6941f06c4e369d5c1307d557bb046aacda4e79cccaab19a13a909f3b`  
		Last Modified: Thu, 13 Oct 2022 21:45:54 GMT  
		Size: 10.3 MB (10336670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:4ad2b57e3b5ae88b93cc20b8dac78741c2424231ad2651333531691aad1f93c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100543176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41ec8bc30486809e3c31cb002da5128b1b4cd2b8a2133df7eb552695df64d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:44 GMT
ADD file:f82ae9ee8436728ac9abdb4af38412611ab80a6dc434a66f2acd4f531df16e41 in / 
# Tue, 04 Oct 2022 23:52:47 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:46:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 		tzdata 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 05 Oct 2022 07:46:23 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Wed, 05 Oct 2022 07:46:24 GMT
ENV OPENSSL_VERSION=1.1.1q
# Wed, 05 Oct 2022 07:46:24 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Wed, 05 Oct 2022 07:46:24 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 05 Oct 2022 07:46:24 GMT
ENV OTP_VERSION=25.1.1
# Wed, 05 Oct 2022 07:46:25 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Wed, 05 Oct 2022 07:49:21 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		g++ 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 05 Oct 2022 07:49:23 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 05 Oct 2022 07:49:23 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:15:54 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:15:55 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:15:55 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:15:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:16:49 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:16:51 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:16:52 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:16:52 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:16:52 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:16:52 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:16:52 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:16:52 GMT
COPY file:d7e54a3570407a262351dfa2e082aa1713b74883d564d1616d93787afcf4b8c0 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:16:53 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:16:53 GMT
CMD ["rabbitmq-server"]
# Wed, 19 Oct 2022 20:17:19 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python3; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 19 Oct 2022 20:17:21 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:55110f99e16edd33cca5c8eacd76396b8cd5660b1e57a10cbdea2b85f8c1dce5`  
		Last Modified: Tue, 04 Oct 2022 23:54:22 GMT  
		Size: 27.0 MB (27044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adfeb76e18e4e428227f942d271e05114e76e7c9abe347bea46e7b6b672d1d2`  
		Last Modified: Wed, 05 Oct 2022 07:53:19 GMT  
		Size: 1.8 MB (1825189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b00adbdda2e5e940eba2480aea56254457199cfab099781a817088fc9a65a`  
		Last Modified: Wed, 05 Oct 2022 07:53:24 GMT  
		Size: 42.5 MB (42476511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c372da9149fb6d4e183411344a49f4e95715475f2d3e27131296d5b7d23965d1`  
		Last Modified: Wed, 05 Oct 2022 07:53:19 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8806745cae0c0e872debf1d1725ae8dd2debdcf704449df59912074e546835f`  
		Last Modified: Wed, 19 Oct 2022 20:21:43 GMT  
		Size: 17.8 MB (17816272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd24e038479365bb9a4c0b4ce4f352e9360ef129f0c1111bad3b7af72e297158`  
		Last Modified: Wed, 19 Oct 2022 20:21:42 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432ea4cfc7d519ca0384683458a38acfbc3de0d8bad416be32a1c76de698f18a`  
		Last Modified: Wed, 19 Oct 2022 20:21:42 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ef5c0bbbef8374b7791374f80bf26bcbd488dbbc4b0d1556d358474e86e081`  
		Last Modified: Wed, 19 Oct 2022 20:21:42 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aea2c62049f6575792bd0f60f6a13046cb88256dc4cc3d6cd8dc8647b43feab`  
		Last Modified: Wed, 19 Oct 2022 20:21:42 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b604e1507aeda11dc7c25cc69acc01891e1fb3f05a1134585e5cf2cfb9f57ff`  
		Last Modified: Wed, 19 Oct 2022 20:22:00 GMT  
		Size: 11.4 MB (11376532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
