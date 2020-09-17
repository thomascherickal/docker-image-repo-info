## `rabbitmq:management`

```console
$ docker pull rabbitmq@sha256:f2e271a2584ffb6a3f69d27e6b67a8bfc8892c78e459f511d02db36a0fc4a991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:1b0b9f733413e4941e810085f9918d0c325245abc991d0aef039dbf342a87b10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86377096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7bf54fe5f510e7c989beded9132b0b1cc2da197442b34c9c57d80f60d4a4d66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:21:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 16 Sep 2020 23:21:25 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Wed, 16 Sep 2020 23:21:26 GMT
ENV OPENSSL_VERSION=1.1.1g
# Wed, 16 Sep 2020 23:21:26 GMT
ENV OPENSSL_SOURCE_SHA256=ddb04774f1e32f0c49751e21b67216ac87852ceb056b75209af2443400636d46
# Wed, 16 Sep 2020 23:21:26 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 16 Sep 2020 23:21:26 GMT
ENV OTP_VERSION=23.0.4
# Wed, 16 Sep 2020 23:21:26 GMT
ENV OTP_SOURCE_SHA256=29e92db80229ec7903f93e5b152c7ca721cc44b58519199ea60b8e0d583faf93
# Wed, 16 Sep 2020 23:30:01 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 16 Sep 2020 23:30:02 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:30:03 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 16 Sep 2020 23:30:03 GMT
ENV RABBITMQ_VERSION=3.8.8
# Wed, 16 Sep 2020 23:30:03 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 16 Sep 2020 23:30:03 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 16 Sep 2020 23:30:03 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=-
# Wed, 16 Sep 2020 23:30:21 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 16 Sep 2020 23:30:23 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:30:24 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 16 Sep 2020 23:30:24 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:30:24 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 16 Sep 2020 23:30:24 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:30:24 GMT
COPY file:f5769ccac78dc9dd6aa3f4dc79e96ef3f91886952a4f45c81a1451ab514cee12 in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:30:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 23:30:25 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 16 Sep 2020 23:30:25 GMT
CMD ["rabbitmq-server"]
# Wed, 16 Sep 2020 23:30:42 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Wed, 16 Sep 2020 23:30:43 GMT
RUN rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:30:57 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; apt-get install -y --no-install-recommends python3; rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 16 Sep 2020 23:30:57 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d691f0af2920353f77679379f91e433e19d2b85f9523007de095207ba108620d`  
		Last Modified: Wed, 16 Sep 2020 23:31:19 GMT  
		Size: 780.0 KB (780031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada79c49f00ddf44afabdacab1dbc1da37d7bd66083f968550730f26751cc8b`  
		Last Modified: Wed, 16 Sep 2020 23:31:24 GMT  
		Size: 32.4 MB (32438479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba904e1a0464f2efe9e80d529591be64410a347cc02274d1e51103085b8a21`  
		Last Modified: Wed, 16 Sep 2020 23:31:18 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ec323f45c9b1f856b6285f444e3d4ab8c366ba55d89957a952a86af039f09d`  
		Last Modified: Wed, 16 Sep 2020 23:31:19 GMT  
		Size: 15.7 MB (15666497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f017e554649ae0dd8676f88c40a1bad5e44e20981c4945f46438758ea11654`  
		Last Modified: Wed, 16 Sep 2020 23:31:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8c2e17052cde9685bc5457af0906fe00baa5176ced0c99bc3a92bdbe3816ea`  
		Last Modified: Wed, 16 Sep 2020 23:31:18 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a973f4e913ea80c3f59ca0a5ab5eff39e82d7e05061d9472528c00a46f7c40`  
		Last Modified: Wed, 16 Sep 2020 23:31:19 GMT  
		Size: 4.7 KB (4687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25c33bba0ae2df865ee666a4cf85282d4ff5ce00c651ccaed01f0677ffd265e`  
		Last Modified: Wed, 16 Sep 2020 23:31:30 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d012b6a4c6f6b73e09f38612efcade7cacd5804f0757ef51fbe0d625b4f039`  
		Last Modified: Wed, 16 Sep 2020 23:31:30 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e848ee187a441692715a8eb5ec27e47520dac98a840d44afa397f1936526eca`  
		Last Modified: Wed, 16 Sep 2020 23:31:33 GMT  
		Size: 10.8 MB (10783898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c4d13e63375b4d6cfe07be14d9f4c67837b58143b5c22a1a86c0d32e666ef2f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79867022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7409d53a303ec2418f4a9e23d8800aad0de950834d344ba38ac516b658eba6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 19 Aug 2020 21:45:03 GMT
ADD file:8369fef9339cb0f1b2b9660d860a6cbf4a5cd6c5e173fbb8cdf8b9485e56aaf4 in / 
# Wed, 19 Aug 2020 21:45:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:45:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:45:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:45:12 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 19 Aug 2020 22:21:07 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Wed, 19 Aug 2020 22:21:08 GMT
ENV OPENSSL_VERSION=1.1.1g
# Wed, 19 Aug 2020 22:21:09 GMT
ENV OPENSSL_SOURCE_SHA256=ddb04774f1e32f0c49751e21b67216ac87852ceb056b75209af2443400636d46
# Wed, 19 Aug 2020 22:21:10 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 11 Sep 2020 23:28:27 GMT
ENV OTP_VERSION=23.0.4
# Fri, 11 Sep 2020 23:28:33 GMT
ENV OTP_SOURCE_SHA256=29e92db80229ec7903f93e5b152c7ca721cc44b58519199ea60b8e0d583faf93
# Fri, 11 Sep 2020 23:33:58 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 11 Sep 2020 23:34:09 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 11 Sep 2020 23:34:41 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 11 Sep 2020 23:34:47 GMT
ENV RABBITMQ_VERSION=3.8.8
# Fri, 11 Sep 2020 23:34:55 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 11 Sep 2020 23:35:02 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 11 Sep 2020 23:35:08 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=-
# Fri, 11 Sep 2020 23:36:11 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 11 Sep 2020 23:36:42 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 11 Sep 2020 23:37:13 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 11 Sep 2020 23:37:20 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 11 Sep 2020 23:37:26 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 11 Sep 2020 23:37:33 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 11 Sep 2020 23:37:45 GMT
COPY file:f5769ccac78dc9dd6aa3f4dc79e96ef3f91886952a4f45c81a1451ab514cee12 in /usr/local/bin/ 
# Fri, 11 Sep 2020 23:37:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 23:37:58 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 11 Sep 2020 23:38:04 GMT
CMD ["rabbitmq-server"]
# Fri, 11 Sep 2020 23:38:52 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 11 Sep 2020 23:39:23 GMT
RUN rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 11 Sep 2020 23:40:13 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; apt-get install -y --no-install-recommends python3; rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Fri, 11 Sep 2020 23:40:20 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:854ab59e811f2c269687884c4899a5de08a5f65b6489dffdb58754086f21e5fc`  
		Last Modified: Mon, 10 Aug 2020 14:29:24 GMT  
		Size: 22.3 MB (22278969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996b7ca18b137080bed3caae4f18c24a2ae9b41a0bd9279d21fe013600e6dbf6`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 35.5 KB (35458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a08dcf8afcac65e6356d202299b593954a299f9ebdb2db237496025225c8f2`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34a2e7cb38ebbe96765deedfead50764f5a482a67ca440de7e9e660db464be7`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593701df30b6b9b3f0d2484426c3ea23481a015c39f451cafbdcd359a31941b7`  
		Last Modified: Wed, 19 Aug 2020 22:28:18 GMT  
		Size: 687.1 KB (687118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030c2f3628adaa3e7d3ff111e552b30b0df721a1eda4a5de69e3c7b7d5e064d9`  
		Last Modified: Fri, 11 Sep 2020 23:52:18 GMT  
		Size: 31.4 MB (31445556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad381249c52264cba158a5e116e7688ead66be3e668fc64254b9213fbbbcb11b`  
		Last Modified: Fri, 11 Sep 2020 23:52:08 GMT  
		Size: 2.2 KB (2163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577e81d7995c69793304cf6945972919bf7db9262b29bd1572d4df818bb526b2`  
		Last Modified: Fri, 11 Sep 2020 23:52:11 GMT  
		Size: 15.7 MB (15666741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54080d86cca909d2b7d04b8b7ec06ecc315400336844250df8bd4d2923e65df`  
		Last Modified: Fri, 11 Sep 2020 23:52:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733ca7770b9499fd478fdc6a255e315b46d1646519b781db21fdc9b29868db4`  
		Last Modified: Fri, 11 Sep 2020 23:52:07 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08f278275c39aa8a700365b5df80821b15903c4e6b277fa0a642aca1c93c63c`  
		Last Modified: Fri, 11 Sep 2020 23:52:08 GMT  
		Size: 4.7 KB (4685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f09e774af81afbc8992158cf82a607fce973e4e0194e2e7e06e3216036fece`  
		Last Modified: Fri, 11 Sep 2020 23:52:37 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b7f2fc950bb999889ce010102ebe5e6c3e2aa3ff6e35704d1fed6c77399cc`  
		Last Modified: Fri, 11 Sep 2020 23:52:37 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93da642e6c0bd42f0e2b0664d1c432f51999aaadbed991ef8b7e4853980dd545`  
		Last Modified: Fri, 11 Sep 2020 23:52:39 GMT  
		Size: 9.7 MB (9744490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:6b6792665170d592396005a9e6973b045ceead5e135811559e531ad8c66fedcf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82292481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adae0dfb4480e82a8129f317cb3905fba563e1d368d8274021145c0287e60d42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:40:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 19 Aug 2020 22:40:59 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Wed, 19 Aug 2020 22:41:00 GMT
ENV OPENSSL_VERSION=1.1.1g
# Wed, 19 Aug 2020 22:41:01 GMT
ENV OPENSSL_SOURCE_SHA256=ddb04774f1e32f0c49751e21b67216ac87852ceb056b75209af2443400636d46
# Wed, 19 Aug 2020 22:41:02 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 11 Sep 2020 22:45:06 GMT
ENV OTP_VERSION=23.0.4
# Fri, 11 Sep 2020 22:45:08 GMT
ENV OTP_SOURCE_SHA256=29e92db80229ec7903f93e5b152c7ca721cc44b58519199ea60b8e0d583faf93
# Fri, 11 Sep 2020 22:50:43 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 11 Sep 2020 22:50:49 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 11 Sep 2020 22:51:08 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 11 Sep 2020 22:51:14 GMT
ENV RABBITMQ_VERSION=3.8.8
# Fri, 11 Sep 2020 22:51:16 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 11 Sep 2020 22:51:17 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 11 Sep 2020 22:51:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=-
# Fri, 11 Sep 2020 22:52:19 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 11 Sep 2020 22:52:38 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 11 Sep 2020 22:52:52 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 11 Sep 2020 22:52:59 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 11 Sep 2020 22:53:08 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 11 Sep 2020 22:53:10 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 11 Sep 2020 22:53:11 GMT
COPY file:f5769ccac78dc9dd6aa3f4dc79e96ef3f91886952a4f45c81a1451ab514cee12 in /usr/local/bin/ 
# Fri, 11 Sep 2020 22:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:53:12 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 11 Sep 2020 22:53:13 GMT
CMD ["rabbitmq-server"]
# Fri, 11 Sep 2020 22:53:46 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 11 Sep 2020 22:53:49 GMT
RUN rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 11 Sep 2020 22:54:22 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; apt-get install -y --no-install-recommends python3; rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Fri, 11 Sep 2020 22:54:29 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ae036ec60f2971711b5ca39695f9d77f433d0d44349b824e2818ac61b0bc1`  
		Last Modified: Wed, 19 Aug 2020 22:48:05 GMT  
		Size: 677.2 KB (677222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff86d35c94b9cc8f9e3fe6a168c2fbcff9caa4b81fea6b85cca8239aaa0a0fce`  
		Last Modified: Fri, 11 Sep 2020 23:02:16 GMT  
		Size: 32.0 MB (32032503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40013ad6f746e9fdc62f640044e024d8ddf878a4be6e701bc8856df69b49a4a5`  
		Last Modified: Fri, 11 Sep 2020 23:02:06 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124a1263b72b798079f6450f37b46506295e5fa00ed9a4fa6cfaaf8bf91aadf8`  
		Last Modified: Fri, 11 Sep 2020 23:02:07 GMT  
		Size: 15.7 MB (15666724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac83d7a2701f96e27e2ac4cba4f5ecfe13be2a25fe702fb4b8dcaef7dde329`  
		Last Modified: Fri, 11 Sep 2020 23:02:06 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550725fb208d8f225d89df558b232ae3ca1e859da1c0fd66b4b298ed73740b22`  
		Last Modified: Fri, 11 Sep 2020 23:02:06 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405f912267c9e3aab485ef9f10628ff71b2ae65fb624c58dc57e2212461e64f3`  
		Last Modified: Fri, 11 Sep 2020 23:02:06 GMT  
		Size: 4.7 KB (4683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c3385358d0ba982cf1a78793d4679499458eb5d47ac7e284633dee3c3938a9`  
		Last Modified: Fri, 11 Sep 2020 23:02:25 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d203b74df77d427c1623beacfb738999db8a6aae1ff2a16ba1abbdc7c8b9044`  
		Last Modified: Fri, 11 Sep 2020 23:02:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0ea771601f428b67c093abcc7ee116ab0e50b5c2c8379c025f5a84224629b1`  
		Last Modified: Fri, 11 Sep 2020 23:02:29 GMT  
		Size: 10.2 MB (10150325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; 386

```console
$ docker pull rabbitmq@sha256:686316689aebbfe5dfaa6a3ea25e2f87a3a9d718aa30cc87a8fbdfc4a73bfe55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86704527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3200b90d069499d903b05e30c33824876a1971b012f736583567dacb1dc14c53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:45:07 GMT
ADD file:ac1c1e51281ff4affbb38dd497cfd5918bc164f9b5239b2273c523c869d19a6f in / 
# Wed, 16 Sep 2020 22:45:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:45:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:45:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:45:09 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 16 Sep 2020 23:16:46 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Wed, 16 Sep 2020 23:16:46 GMT
ENV OPENSSL_VERSION=1.1.1g
# Wed, 16 Sep 2020 23:16:46 GMT
ENV OPENSSL_SOURCE_SHA256=ddb04774f1e32f0c49751e21b67216ac87852ceb056b75209af2443400636d46
# Wed, 16 Sep 2020 23:16:46 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 16 Sep 2020 23:16:46 GMT
ENV OTP_VERSION=23.0.4
# Wed, 16 Sep 2020 23:16:47 GMT
ENV OTP_SOURCE_SHA256=29e92db80229ec7903f93e5b152c7ca721cc44b58519199ea60b8e0d583faf93
# Wed, 16 Sep 2020 23:26:11 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 16 Sep 2020 23:26:11 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:26:13 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 16 Sep 2020 23:26:13 GMT
ENV RABBITMQ_VERSION=3.8.8
# Wed, 16 Sep 2020 23:26:14 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 16 Sep 2020 23:26:14 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 16 Sep 2020 23:26:15 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=-
# Wed, 16 Sep 2020 23:26:38 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 16 Sep 2020 23:26:40 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:26:41 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 16 Sep 2020 23:26:41 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:26:41 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 16 Sep 2020 23:26:41 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:26:42 GMT
COPY file:f5769ccac78dc9dd6aa3f4dc79e96ef3f91886952a4f45c81a1451ab514cee12 in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:26:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 23:26:42 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 16 Sep 2020 23:26:42 GMT
CMD ["rabbitmq-server"]
# Wed, 16 Sep 2020 23:26:55 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Wed, 16 Sep 2020 23:26:56 GMT
RUN rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:27:12 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; apt-get install -y --no-install-recommends python3; rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 16 Sep 2020 23:27:13 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:c064321cb7faf77d51d828e13cc9567067c4029cbdd0466f7859807600975b60`  
		Last Modified: Mon, 07 Sep 2020 15:50:23 GMT  
		Size: 27.1 MB (27124630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03be3b2ff776d52c17b5ff364b55809fc4508b7181d41134e8590bd24cd0beb8`  
		Last Modified: Wed, 16 Sep 2020 22:45:55 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb9e8aa804f2f11311452b78b4d269bd07b41637989332956f1edf1fab7c64d`  
		Last Modified: Wed, 16 Sep 2020 22:45:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5026b6db9cb277cb89143c0c44679fd1f94a8920de2f7065ef14f534e095940f`  
		Last Modified: Wed, 16 Sep 2020 23:27:40 GMT  
		Size: 690.0 KB (689989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0d123029b53d16acc5642ad17790ea646253e8a7a938bcc54bc5e9bf8702f7`  
		Last Modified: Wed, 16 Sep 2020 23:27:50 GMT  
		Size: 32.4 MB (32363015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302b7982198740e51068077f609f3304a2075dc285aa7520fc6cfa4910ce02b`  
		Last Modified: Wed, 16 Sep 2020 23:27:38 GMT  
		Size: 2.1 KB (2090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ea8dd246a176a3c37613922dbfeacf20c30a2b56d9638a52d7f97794797704`  
		Last Modified: Wed, 16 Sep 2020 23:27:42 GMT  
		Size: 15.7 MB (15665913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21abfbf9ee6e00f228109c52dc1c4c39664664f884f1ea912cde13357387725c`  
		Last Modified: Wed, 16 Sep 2020 23:27:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db7948a4c9f0b467916cf1219b703005b29ae8c04ec709c6e81f22ed3c1a616`  
		Last Modified: Wed, 16 Sep 2020 23:27:38 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb41e8b3e91924a961115d269edb94e321706e558c2974ce3aec56ae241a1e8`  
		Last Modified: Wed, 16 Sep 2020 23:27:38 GMT  
		Size: 4.7 KB (4688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce1a128d8ecbd468be0e362b4387c69b8071860805a1102d648d54938f87c0`  
		Last Modified: Wed, 16 Sep 2020 23:27:57 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd4c38e05601cba5528403493791a54c77d7d6719cc774a6d38f5a7634948bf`  
		Last Modified: Wed, 16 Sep 2020 23:27:57 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce019785a1cfad0cbb04ab593a178ab9fa9fac71f0135ac2c0675aa87fe79ad`  
		Last Modified: Wed, 16 Sep 2020 23:28:00 GMT  
		Size: 10.9 MB (10852393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:6fd4fb7f4246d0f0ac6bf1cd4c694230cf0667f0f2f4414cf54f9d832b306f81
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71566538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef043526f9a696cc8e75889cdf1d93d109abdf7057e625d73a19e58894a7d592`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 16 Oct 2018 08:22:25 GMT
ADD file:b1fa1d0ffa2b206311dfd95642d74c3312565a1ec2e6e3a2197bfd2a4b3de6c6 in / 
# Tue, 16 Oct 2018 08:22:30 GMT
CMD ["bash"]
# Tue, 16 Oct 2018 13:26:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 Oct 2018 13:27:02 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 16 Oct 2018 13:27:04 GMT
ENV GOSU_VERSION=1.10
# Tue, 16 Oct 2018 13:27:42 GMT
RUN set -eux; 		fetchDeps=' 		ca-certificates 		wget 	'; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 16 Oct 2018 13:27:45 GMT
RUN set -eux; 	sed 's/stretch/buster/g' /etc/apt/sources.list 		| tee /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster*'; 		echo 'Pin-Priority: 1'; 		echo; 		echo 'Package: erlang*'; 		echo 'Pin: release n=buster*'; 		echo 'Pin-Priority: 999'; 		echo; 		echo 'Package: erlang*'; 		echo 'Pin: release n=stretch*'; 		echo 'Pin-Priority: -10'; 	} | tee /etc/apt/preferences.d/buster-erlang
# Tue, 16 Oct 2018 13:28:55 GMT
RUN set -eux; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 Oct 2018 13:28:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 16 Oct 2018 13:29:01 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Oct 2018 13:29:03 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 16 Oct 2018 13:29:04 GMT
ENV RABBITMQ_VERSION=3.7.8
# Tue, 16 Oct 2018 13:29:05 GMT
ENV RABBITMQ_GITHUB_TAG=v3.7.8
# Tue, 16 Oct 2018 13:29:06 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.7.8-1
# Tue, 16 Oct 2018 13:29:52 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 16 Oct 2018 13:29:53 GMT
ENV LANG=C.UTF-8
# Tue, 16 Oct 2018 13:29:54 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 30 Oct 2018 10:14:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq /var/log/rabbitmq /tmp/rabbitmq-ssl 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq /var/log/rabbitmq /tmp/rabbitmq-ssl 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq /var/log/rabbitmq /tmp/rabbitmq-ssl
# Tue, 30 Oct 2018 10:14:08 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 30 Oct 2018 10:14:12 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 30 Oct 2018 10:14:15 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Tue, 30 Oct 2018 10:14:16 GMT
COPY file:e34e867160294a2e05bd38fa5d336df66261a0ae77ee6f859e1875ee8e4da556 in /usr/local/bin/ 
# Tue, 30 Oct 2018 10:14:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Oct 2018 10:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Oct 2018 10:14:23 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Tue, 30 Oct 2018 10:14:24 GMT
CMD ["rabbitmq-server"]
# Tue, 30 Oct 2018 10:15:21 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 30 Oct 2018 10:16:03 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; 	apt-get install -y --no-install-recommends python; 	rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Tue, 30 Oct 2018 10:16:06 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:202f659db3e53c01ac947538d8b37251e9fa16c4a6a699dc6c2a8910afcdfed4`  
		Last Modified: Tue, 16 Oct 2018 08:30:59 GMT  
		Size: 22.7 MB (22740583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecb3827380c4f397cd4889f00fc5544837c98a7021894868639ba977cbc9cd`  
		Last Modified: Tue, 16 Oct 2018 13:35:10 GMT  
		Size: 4.4 MB (4360630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af645453998bbb42a5f24dda8519eca988db31e4ff438c5a797298be84450c21`  
		Last Modified: Tue, 16 Oct 2018 13:35:05 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3ab92767ce3070fcb1317990449216a04b91ef3519a13e41ded4867395fb94`  
		Last Modified: Tue, 16 Oct 2018 13:35:05 GMT  
		Size: 920.6 KB (920625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d66cc37afb7cef45ce6cb12857ebdb72e8b8e9cd969b5c85ef6c20fa1ef8ed`  
		Last Modified: Tue, 16 Oct 2018 13:35:04 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7d12e7388f7429cba69f06fd908a72406843b8e51fedfb17cf68a8f524d77`  
		Last Modified: Tue, 16 Oct 2018 13:35:10 GMT  
		Size: 25.4 MB (25378958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6ce610a7a885d06cfdfca9023bafacec3fbe9f9f7473eb56511de4e4ce9df`  
		Last Modified: Tue, 16 Oct 2018 13:35:07 GMT  
		Size: 10.3 MB (10325923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad73571d848148413b6db267b9f02ed24336604026203013d6b0aab4d0059175`  
		Last Modified: Tue, 30 Oct 2018 10:35:53 GMT  
		Size: 2.4 KB (2373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a7b4ac678f4aa6a5c7e4f7517f8c4402074e081ca9be28d06efa8efedc0ed`  
		Last Modified: Tue, 30 Oct 2018 10:35:50 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018a18fa6662ba8882872117fa871fc7fc11f513e902ee4fe4664f54977be13`  
		Last Modified: Tue, 30 Oct 2018 10:35:50 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981c275e3b7cf152da90f9338fa01c4beb392f01d3bf9282be36c0ca5fc25147`  
		Last Modified: Tue, 30 Oct 2018 10:35:32 GMT  
		Size: 4.4 KB (4423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a054ca0d6af281273e00f8def7f369fca9589b2910d84dfce500a53796fe9c`  
		Last Modified: Tue, 30 Oct 2018 10:35:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939a666217f05bc14dd985091f06978738deb3731d0047d402c2bf6dabaf5f3d`  
		Last Modified: Tue, 30 Oct 2018 10:36:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2756ea1a7ae9135b42290a148c941fdc0d66a7a14c84eb91c43ba3caa8e62b`  
		Last Modified: Tue, 30 Oct 2018 10:36:45 GMT  
		Size: 7.8 MB (7827964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:00f68c5f4f2ded77698745ca9a8b0aaa396010accf05b3d01445549dcc8e6d04
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84345759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a90991123b0eb158668a72483de8ea663f2b089c34f2866aa183f49dc9f0eaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:51:22 GMT
ADD file:835d62b9e8aa5985cb778cef4129baec4d3688713202ad55a1fa54bb9daf136e in / 
# Wed, 16 Sep 2020 22:51:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:51:25 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:51:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:51:26 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:08:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*; 	gosu nobody true
# Wed, 16 Sep 2020 23:08:32 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Wed, 16 Sep 2020 23:08:32 GMT
ENV OPENSSL_VERSION=1.1.1g
# Wed, 16 Sep 2020 23:08:33 GMT
ENV OPENSSL_SOURCE_SHA256=ddb04774f1e32f0c49751e21b67216ac87852ceb056b75209af2443400636d46
# Wed, 16 Sep 2020 23:08:33 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Wed, 16 Sep 2020 23:08:33 GMT
ENV OTP_VERSION=23.0.4
# Wed, 16 Sep 2020 23:08:33 GMT
ENV OTP_SOURCE_SHA256=29e92db80229ec7903f93e5b152c7ca721cc44b58519199ea60b8e0d583faf93
# Wed, 16 Sep 2020 23:11:32 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		autoconf 		ca-certificates 		dpkg-dev 		gcc 		gnupg 		libncurses5-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum --check --strict -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	debMultiarch="$(dpkg-architecture --query DEB_HOST_MULTIARCH)"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		--libdir="lib/$debMultiarch" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	ldconfig; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --progress dot:giga --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum --check --strict -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; export CFLAGS; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Wed, 16 Sep 2020 23:11:33 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:11:34 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 16 Sep 2020 23:11:34 GMT
ENV RABBITMQ_VERSION=3.8.8
# Wed, 16 Sep 2020 23:11:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 16 Sep 2020 23:11:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 16 Sep 2020 23:11:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=-
# Wed, 16 Sep 2020 23:11:49 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 16 Sep 2020 23:11:50 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:11:51 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 16 Sep 2020 23:11:51 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 16 Sep 2020 23:11:51 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 16 Sep 2020 23:11:52 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:11:52 GMT
COPY file:f5769ccac78dc9dd6aa3f4dc79e96ef3f91886952a4f45c81a1451ab514cee12 in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 23:11:52 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 16 Sep 2020 23:11:52 GMT
CMD ["rabbitmq-server"]
# Wed, 16 Sep 2020 23:12:03 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Wed, 16 Sep 2020 23:12:04 GMT
RUN rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 16 Sep 2020 23:12:13 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apt-get update; apt-get install -y --no-install-recommends python3; rm -rf /var/lib/apt/lists/*; 	rabbitmqadmin --version
# Wed, 16 Sep 2020 23:12:14 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:cedb15d27487fa2e085bee049ff12636f8ba01e63c3bbdc094088e8bb7d8b641`  
		Last Modified: Mon, 07 Sep 2020 15:51:50 GMT  
		Size: 25.4 MB (25370945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4002d8c6f20fd20eb7aa7e91bfa01443724872a214bb07ad9cf86a810c86ed`  
		Last Modified: Wed, 16 Sep 2020 22:52:22 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b15c73b5f07d5d69927632e5a59fb80805da20bc1fabc30f973b5b2ff5805`  
		Last Modified: Wed, 16 Sep 2020 22:52:22 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f69c39c75db1d4580ec7e55396ea6c888a2b3fdf02923e7c2c040ca5a783c1`  
		Last Modified: Wed, 16 Sep 2020 23:12:37 GMT  
		Size: 780.4 KB (780406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373eb10ce704b2b51903e00c983de93365280e9b67b9e4137d7045d50684c9d1`  
		Last Modified: Wed, 16 Sep 2020 23:12:41 GMT  
		Size: 32.1 MB (32109619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aec2b4c37b474b9c1323c5222221c4b2e12601da8c423bbc0f786a8d76c43f2`  
		Last Modified: Wed, 16 Sep 2020 23:12:35 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c851d319aab5582dcaa1cc7d9c756b4da911a32212bda3b90519d9af5c5d55bc`  
		Last Modified: Wed, 16 Sep 2020 23:12:36 GMT  
		Size: 15.7 MB (15665366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1c84671352e6213b9c25478f0e0714ece2a39c5027a4195513e98bac4e63aa`  
		Last Modified: Wed, 16 Sep 2020 23:12:36 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ad7540c84e49a6029b4ed72c39a3fb6dd4eff92b346a5be12d9f21ea2e7b55`  
		Last Modified: Wed, 16 Sep 2020 23:12:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cc078ff775b75f7c9dcf1fe498ec0d9f595c92b94b646a472e26a4cd3b7c1b`  
		Last Modified: Wed, 16 Sep 2020 23:12:35 GMT  
		Size: 4.7 KB (4685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6690e653219cd3d9577b6d65ccb8359254f1e9e65ebd6d42f05f45c7dde1871f`  
		Last Modified: Wed, 16 Sep 2020 23:12:49 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e46b3710d25fabf2fdca75aa5d10b6ad4e182b94a0b10f559564191bc0f9c5`  
		Last Modified: Wed, 16 Sep 2020 23:12:49 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a445373dca69696b4ab6aeed7c5800aea9ec123836d5968eb09c9143d9e5298c`  
		Last Modified: Wed, 16 Sep 2020 23:12:51 GMT  
		Size: 10.4 MB (10410727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
