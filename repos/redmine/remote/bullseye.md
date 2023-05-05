## `redmine:bullseye`

```console
$ docker pull redmine@sha256:7ec3b436e8a70445a7b696e724f7f79e87756ead71e5c28051d7d389b2851557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:bullseye` - linux; amd64

```console
$ docker pull redmine@sha256:543d88dddd4677fa4efeb35efc8d60e9b4f671424e89768a13b3cf389aaab1c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240459155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e1bbde27d1808fca10a4ff2bd73b3bdf116b6dd64bf0dcf7a225d99ca4ca35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:08:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 19:08:49 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 19:19:16 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 19:19:17 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 19:19:17 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 19:21:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 19:21:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 19:21:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 19:21:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 19:21:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 19:21:35 GMT
CMD ["irb"]
# Thu, 04 May 2023 08:52:23 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 04 May 2023 08:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:52:59 GMT
ENV RAILS_ENV=production
# Thu, 04 May 2023 08:52:59 GMT
WORKDIR /usr/src/redmine
# Thu, 04 May 2023 08:52:59 GMT
ENV HOME=/home/redmine
# Thu, 04 May 2023 08:53:00 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 04 May 2023 08:53:00 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 04 May 2023 08:53:00 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 04 May 2023 08:53:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 04 May 2023 08:53:03 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 04 May 2023 08:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 May 2023 08:53:34 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 04 May 2023 08:53:34 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 04 May 2023 08:53:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 08:53:34 GMT
EXPOSE 3000
# Thu, 04 May 2023 08:53:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201ffa30101754210c7fbca23d2147904756a96e7f8d9754f6db4bc31580083c`  
		Last Modified: Wed, 03 May 2023 19:42:49 GMT  
		Size: 10.0 MB (10023164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaf5502212fbe68d4ac640762fb12d59af0868a4cd48fb88fd3e7612d79c165`  
		Last Modified: Wed, 03 May 2023 19:42:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5989aaa467739f805f59f49c0a3760fb8ce5823811aafed2047cd795702e85b`  
		Last Modified: Wed, 03 May 2023 19:44:01 GMT  
		Size: 32.6 MB (32626126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9217ac23b4ffb1f4c4f88d8e6ecf75f075baddf3d460235576adacd563695f`  
		Last Modified: Wed, 03 May 2023 19:43:59 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfff5d2555333adcf30d9ac46f9b53f66068d38493b07e0f22c96ae1454f91cd`  
		Last Modified: Thu, 04 May 2023 08:55:47 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d891fae24e2268b1d51f5f6f98541fb2ad0de0fa1500d1119e50095e5e6e86d`  
		Last Modified: Thu, 04 May 2023 08:56:01 GMT  
		Size: 102.0 MB (101950855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5088d0bb4d616b66757ce59f26a16d77ef5b3fd5cfd00c6cfb60b400ffdb7a`  
		Last Modified: Thu, 04 May 2023 08:55:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90fea341e9bed0799d84c9c55f33825c2dc1a70a0949af70e774290a8a37729`  
		Last Modified: Thu, 04 May 2023 08:55:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ad114b837f98f3ba0a20553d16fc74a59d17c394c2a2f9a812742d04c09b28`  
		Last Modified: Thu, 04 May 2023 08:55:45 GMT  
		Size: 3.1 MB (3144728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f47a6fb15a7eb6ddd2e9bb4c98eb4e9f1e6bd5ea2cee018d044183fbd8bf7`  
		Last Modified: Thu, 04 May 2023 08:55:51 GMT  
		Size: 61.3 MB (61306310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b5bfed32de3a1afc002603da871c0444b29cbbdb75d977c9e7462d48234f4`  
		Last Modified: Thu, 04 May 2023 08:55:45 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6d65b1d7f53948336a5893b8ef8faad540dd897fb48d3a62c669d1c88892eb3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.3 MB (239269880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199668d8b422c98b1c83ed8feaabd924a8b623b1a56f0244c17ee4543155e8b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:47:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:47:12 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:53:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:53:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:53:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:53:59 GMT
CMD ["irb"]
# Wed, 03 May 2023 14:11:42 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 03 May 2023 14:12:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:12:18 GMT
ENV RAILS_ENV=production
# Wed, 03 May 2023 14:12:18 GMT
WORKDIR /usr/src/redmine
# Wed, 03 May 2023 14:12:18 GMT
ENV HOME=/home/redmine
# Wed, 03 May 2023 14:12:18 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 03 May 2023 14:12:18 GMT
ENV REDMINE_VERSION=5.0.5
# Wed, 03 May 2023 14:12:18 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Wed, 03 May 2023 14:12:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Wed, 03 May 2023 14:12:22 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 03 May 2023 14:14:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 14:14:08 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 03 May 2023 14:14:09 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Wed, 03 May 2023 14:14:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 03 May 2023 14:14:09 GMT
EXPOSE 3000
# Wed, 03 May 2023 14:14:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520c96d75b8bbb8ca7b74094ff4ee8c41cf536df6bac998b01db4bd0935efe6`  
		Last Modified: Wed, 03 May 2023 12:03:22 GMT  
		Size: 8.6 MB (8634343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cb808d1e8f9d1f674dfe2463dc61ac8964cca0d926c771ef50a5b0d9a35ecb`  
		Last Modified: Wed, 03 May 2023 12:03:20 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4531177c93e28b694e7e317d2f2890bac6f942f7dee94878d6282471111f82f`  
		Last Modified: Wed, 03 May 2023 12:04:00 GMT  
		Size: 31.2 MB (31165955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa7d2bcae37a40150f43a34637125411cf26751d3b7f0b59fea5bf3e03df1d`  
		Last Modified: Wed, 03 May 2023 12:03:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e59205b583bf14edab14bd94ad1e93d8cbb74b3c0837f7b825c38c531d4ad8`  
		Last Modified: Wed, 03 May 2023 14:17:08 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bb8ed065dbb75a96668d33629a64a16659581935847be6f40fc3a361d736f3`  
		Last Modified: Wed, 03 May 2023 14:17:23 GMT  
		Size: 96.9 MB (96937260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535311ed61227a8bb3ccdf12354f3d70a0d0f16f96da0c349adc1cceed7032b0`  
		Last Modified: Wed, 03 May 2023 14:17:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d698c65b239db60f7cf57ad04d312e45a1ac5df3bd2a2c843cd270f9c2f65b`  
		Last Modified: Wed, 03 May 2023 14:17:05 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aec496dd633f6777932bee807a8f195de5e9e7681786bc07a26861c855ef2a`  
		Last Modified: Wed, 03 May 2023 14:17:06 GMT  
		Size: 3.1 MB (3144728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61002fb84b8dc1aca1a989165c20b3e22aaea3ec9a1302103b67d3c96499214`  
		Last Modified: Wed, 03 May 2023 14:17:13 GMT  
		Size: 70.5 MB (70479725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1094e56d025d2bb950772eb81685c223509e5199c2ef06d2d07a706f8fa7e`  
		Last Modified: Wed, 03 May 2023 14:17:05 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:f6a4e89fa7740867db8704d3078851ae53062933afb1078dfd16849586fa398e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232177907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1751b7090d34a84f721f391d6d5f86e57d76c0e32eb6b8e602edf020a8e3bf5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 15:04:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:04:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 15:04:30 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 15:13:08 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 15:13:08 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 15:13:08 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 15:15:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 15:15:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 15:15:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 15:15:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:15:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 15:15:07 GMT
CMD ["irb"]
# Thu, 04 May 2023 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 04 May 2023 06:58:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 06:58:36 GMT
ENV RAILS_ENV=production
# Thu, 04 May 2023 06:58:36 GMT
WORKDIR /usr/src/redmine
# Thu, 04 May 2023 06:58:36 GMT
ENV HOME=/home/redmine
# Thu, 04 May 2023 06:58:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 04 May 2023 06:58:37 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 04 May 2023 06:58:37 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 04 May 2023 06:58:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 04 May 2023 06:58:40 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 04 May 2023 07:00:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 May 2023 07:00:12 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 04 May 2023 07:00:12 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 04 May 2023 07:00:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:00:13 GMT
EXPOSE 3000
# Thu, 04 May 2023 07:00:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b4d9291c9933451d8b76290c3e6931085c6d07e8b924df3ca7adff5bf6c57e`  
		Last Modified: Wed, 03 May 2023 15:34:16 GMT  
		Size: 8.1 MB (8143782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fc957833ebe20d5c94e0eb971e265ab56116e4317427dea0623899524f1503`  
		Last Modified: Wed, 03 May 2023 15:34:15 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e920954585c8f9233efb5284e860208ca00352c22071b72b69d5f564b4906b`  
		Last Modified: Wed, 03 May 2023 15:35:28 GMT  
		Size: 31.0 MB (31035278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609dc7ec330e3e1ffdce32a37ffe03ad318e8066aa5d15aebc8e7ce4290010d6`  
		Last Modified: Wed, 03 May 2023 15:35:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ef55da5ec03ffb307aa1c65e8b8fc4c40b140f08d359cb20d84ba0e86930a3`  
		Last Modified: Thu, 04 May 2023 07:02:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07acf7f691d1088ecb99131d9366c3bb8a9dab496fbe50e16cdfa439e8b7659`  
		Last Modified: Thu, 04 May 2023 07:03:14 GMT  
		Size: 93.1 MB (93088761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0ff9740f14cbd9e7f857fbbe75253af24de704a0130f86b6f60c3f3495ac13`  
		Last Modified: Thu, 04 May 2023 07:02:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8872cc298ce1dc84e11ebe7226edaf19b0358097bf9c9282b708492fd549d251`  
		Last Modified: Thu, 04 May 2023 07:02:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cb58f058a7954d9b7d3fc5a961b4d4ddd5961db2819921792e6c58c5770a7c`  
		Last Modified: Thu, 04 May 2023 07:02:58 GMT  
		Size: 3.1 MB (3144730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c411bd904296035e4cb79956a7bf2d29bfd9243d85b0e336f523107d05e4cc`  
		Last Modified: Thu, 04 May 2023 07:03:05 GMT  
		Size: 70.2 MB (70196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f1201b89285b5ba4e250898ac7ef2f001c66ccc27a767e6452d488d1411c6d`  
		Last Modified: Thu, 04 May 2023 07:02:57 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:bcc02fe8b5392f3f21da6d3b64d0360d5ef1d0783d3b88711bdd0329b6a96dc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234943819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fb8e0c97192f45f30e3088f6bf20e7b223e660fb9c83f48c5b3af31c6fa732`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:33:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:33:36 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:43:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:43:29 GMT
CMD ["irb"]
# Thu, 04 May 2023 03:58:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 04 May 2023 03:59:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:59:22 GMT
ENV RAILS_ENV=production
# Thu, 04 May 2023 03:59:22 GMT
WORKDIR /usr/src/redmine
# Thu, 04 May 2023 03:59:22 GMT
ENV HOME=/home/redmine
# Thu, 04 May 2023 03:59:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 04 May 2023 03:59:22 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 04 May 2023 03:59:22 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 04 May 2023 03:59:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 04 May 2023 03:59:25 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 04 May 2023 03:59:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 May 2023 03:59:50 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 04 May 2023 03:59:50 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 04 May 2023 03:59:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:59:50 GMT
EXPOSE 3000
# Thu, 04 May 2023 03:59:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1531f71db6b0a18949b875d88c4e89771d1f342242ace07be465eaf823657`  
		Last Modified: Wed, 03 May 2023 12:00:18 GMT  
		Size: 9.2 MB (9243388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09062a3cd32c5e4b240a84c6d1b7286f252e13dd31c44688b8ef1fc66feb47ed`  
		Last Modified: Wed, 03 May 2023 12:00:15 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae0e0c21b62b4bd50e21055fb4282e3349a1877e660140f5ad2406a00e97f1f`  
		Last Modified: Wed, 03 May 2023 12:01:25 GMT  
		Size: 32.0 MB (31987241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e53e9b73e036c9fdcc00931455984a0c2e31e51db93a901bd0fed695001f4`  
		Last Modified: Wed, 03 May 2023 12:01:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a762b8248238fa348d50e7f27fee248bbdbab684d60c6b098feb1ba9375036`  
		Last Modified: Thu, 04 May 2023 04:01:29 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f5b7c7fa8bbf7ab35714b2ba6b74299144de826be21efdb794fac40b41959`  
		Last Modified: Thu, 04 May 2023 04:01:39 GMT  
		Size: 99.7 MB (99729020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9ab98876fd4b7b70301adaac64951b1521ffadc52b20aeea628621a903c6d7`  
		Last Modified: Thu, 04 May 2023 04:01:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c5a0c0a727a98973d3fc62fe4c30034134327ab7760372e0d33c5043452518`  
		Last Modified: Thu, 04 May 2023 04:01:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24b1c544f595457a95487e0e902e02cd98be8b00232b2f910f1cf15990700d8`  
		Last Modified: Thu, 04 May 2023 04:01:27 GMT  
		Size: 3.1 MB (3144727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe40bf5a329cee6872384b501eb133304041838a7e3090fe30de276ea4123b5`  
		Last Modified: Thu, 04 May 2023 04:01:32 GMT  
		Size: 60.8 MB (60782249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d05d15cb6fd58da1bc73ca0f6fcbe45c3179eb28b607443e6b5f35f9508d8e1`  
		Last Modified: Thu, 04 May 2023 04:01:27 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; 386

```console
$ docker pull redmine@sha256:4e20069448b04f658e7ad134a1c2072a98aa4826c266046400ce4e6c4ea1ffbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242613928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f5125cb4e75212e2845dc7baef5a99f721e3fc113ba1759ca3141b9070672e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:18:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 18:18:59 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:33:36 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 18:33:36 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 18:33:36 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 18:37:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 18:37:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 18:37:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 18:37:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 18:37:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 18:37:16 GMT
CMD ["irb"]
# Thu, 04 May 2023 05:17:33 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 04 May 2023 05:18:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 05:18:13 GMT
ENV RAILS_ENV=production
# Thu, 04 May 2023 05:18:13 GMT
WORKDIR /usr/src/redmine
# Thu, 04 May 2023 05:18:13 GMT
ENV HOME=/home/redmine
# Thu, 04 May 2023 05:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 04 May 2023 05:18:14 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 04 May 2023 05:18:14 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 04 May 2023 05:18:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 04 May 2023 05:18:17 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 04 May 2023 05:19:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 May 2023 05:19:05 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 04 May 2023 05:19:06 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 04 May 2023 05:19:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 05:19:06 GMT
EXPOSE 3000
# Thu, 04 May 2023 05:19:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408abed653e613b07e8c84630724d9ad6141b392b7643c8a01047952c3693eb`  
		Last Modified: Wed, 03 May 2023 19:08:53 GMT  
		Size: 12.0 MB (11997391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d241d202694b05aab8780b8a505df93b608c713321dabfdf9a9262570d11837`  
		Last Modified: Wed, 03 May 2023 19:08:49 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6ea84121c8edf6918e58f9f25dd453d43d0caf47e7e2ae9f77e80b43d02f24`  
		Last Modified: Wed, 03 May 2023 19:10:09 GMT  
		Size: 31.2 MB (31181567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9315d30535983d554dff626b6603d336b3836b1882dc4e0a531edbefd6997778`  
		Last Modified: Wed, 03 May 2023 19:10:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56045e940e55b9bd90a8a3fcbced80ff6676fa9ff524ebd7be6b2ec8ebc4953`  
		Last Modified: Thu, 04 May 2023 05:21:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c91d3479dd15e6fca749897cc064faa9433b353f9dc934004ef1640dc9ebd`  
		Last Modified: Thu, 04 May 2023 05:21:28 GMT  
		Size: 103.3 MB (103279895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9e84867beb9fd5a5dd569e24833f38d5b63b7e3e7f7f3caaaf88c728f9b092`  
		Last Modified: Thu, 04 May 2023 05:21:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b1bd16b8b83dd3dcea6317860c27f62493593ffd0df9d5364d33f48e2cf66`  
		Last Modified: Thu, 04 May 2023 05:21:03 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b011a6682c722dd7b196435e2d59930d3325c2e94e1b3ccb9603e430b1f702e0`  
		Last Modified: Thu, 04 May 2023 05:21:04 GMT  
		Size: 3.1 MB (3144719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0609553a9474403a07d8ea0a7b00852088a241e7184a676cd8ee5f237c9cfd`  
		Last Modified: Thu, 04 May 2023 05:21:15 GMT  
		Size: 60.6 MB (60617700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afbf132a6b27e61f5d37a72a2707e6160f464d2b948f82ab98b3273229a4c53`  
		Last Modified: Thu, 04 May 2023 05:21:03 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:5838110a9662636caf59d367ccc3c07c6a9d497f8683cd8044f4bbc9167ba249
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.6 MB (262605044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339e63b5dc7dbdc6800dfbe33d1b3973d3e9fefff1fe0d236108dbc0099b3956`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 03 May 2023 00:31:50 GMT
ADD file:ee3b3c43add645e1a2078f2a6e8544d223abf2754eb8039cbbc2cbdb911b49bb in / 
# Wed, 03 May 2023 00:31:52 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:58:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 20:58:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 20:58:26 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:08:00 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 21:08:01 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 21:08:01 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 21:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 21:12:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 21:12:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 21:13:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:13:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 21:13:02 GMT
CMD ["irb"]
# Thu, 04 May 2023 16:44:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 04 May 2023 16:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 16:46:29 GMT
ENV RAILS_ENV=production
# Thu, 04 May 2023 16:46:29 GMT
WORKDIR /usr/src/redmine
# Thu, 04 May 2023 16:46:30 GMT
ENV HOME=/home/redmine
# Thu, 04 May 2023 16:46:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 04 May 2023 16:46:31 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 04 May 2023 16:46:32 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 04 May 2023 16:46:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 04 May 2023 16:46:37 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 04 May 2023 16:50:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 May 2023 16:50:09 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 04 May 2023 16:50:10 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 04 May 2023 16:50:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 16:50:10 GMT
EXPOSE 3000
# Thu, 04 May 2023 16:50:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e39c6de44f96d2720b144cbaa9e763eac60a69222a96279f3962e8a701fb17ac`  
		Last Modified: Wed, 03 May 2023 00:36:56 GMT  
		Size: 35.3 MB (35280910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444e3b940442c260a138ecf472498e2f3c2f056210fc4f8d1e2d4ff58387ab0e`  
		Last Modified: Wed, 03 May 2023 21:30:08 GMT  
		Size: 10.5 MB (10481292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6d7068324b787a6069c017c9e1e3b8f6a52905ee229daaed9490c3d2715698`  
		Last Modified: Wed, 03 May 2023 21:30:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3db922d54071aea0992b5cef91bb1646a917ee8665061063c60c66935a826db`  
		Last Modified: Wed, 03 May 2023 21:31:02 GMT  
		Size: 32.8 MB (32791808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5768d8ebfb37431c322ba8ac213ae02b4f33cdf75acc9010349343a987d3c3db`  
		Last Modified: Wed, 03 May 2023 21:30:56 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd2a81bee7d822c4329d20d0e878044d2184dc7bbbda61012b1a79ef924fe5`  
		Last Modified: Thu, 04 May 2023 16:56:06 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac227b32ee7bba661edefb0eb54cc3849bf86d4756f042ea3ee6001a0384a81f`  
		Last Modified: Thu, 04 May 2023 16:56:35 GMT  
		Size: 107.4 MB (107445307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f28da8c552a3378dbe2c40fb48054b5e08443dbae93d8db46a8c14d922bf6e9`  
		Last Modified: Thu, 04 May 2023 16:56:04 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc51cc04f317f9a2c3072ed3d625e299ef0d7b0458dcd329ac08a77c50172689`  
		Last Modified: Thu, 04 May 2023 16:56:04 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3830f3f5abe60a4d785bd612110587e094971e67aa0cffe365005ce6407b4d6`  
		Last Modified: Thu, 04 May 2023 16:56:06 GMT  
		Size: 3.1 MB (3144729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f8ef986c68a5595e5f7810ec4931bb0f2ae240fc28b395d441d558fa5695a5`  
		Last Modified: Thu, 04 May 2023 16:56:18 GMT  
		Size: 73.5 MB (73456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a70e0a603e7f45119c991add5c7ebd8ed1a1899397a9817870e75646e0932b`  
		Last Modified: Thu, 04 May 2023 16:56:04 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:ce2f9a8bba7cda3aa144886ee2239cfd1a2f84384e7a193ce5263f63f1f48a45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246275184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4358f4d4c81c2b989fa857fa3ea5796b04494246430e72d779a37611ee868379`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 03 May 2023 03:41:57 GMT
ADD file:7dcdb7d695d9510a1a7e1623776d63d56f7025bdd1702a13a3acd52af825b9c3 in / 
# Wed, 03 May 2023 03:41:59 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:41:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 21:41:40 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:50:49 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 21:50:49 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 21:50:50 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 21:52:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 21:52:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 21:52:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 21:52:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:52:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 21:52:53 GMT
CMD ["irb"]
# Fri, 05 May 2023 00:40:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 05 May 2023 00:40:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 00:40:45 GMT
ENV RAILS_ENV=production
# Fri, 05 May 2023 00:40:45 GMT
WORKDIR /usr/src/redmine
# Fri, 05 May 2023 00:40:45 GMT
ENV HOME=/home/redmine
# Fri, 05 May 2023 00:40:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 05 May 2023 00:40:46 GMT
ENV REDMINE_VERSION=5.0.5
# Fri, 05 May 2023 00:40:46 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Fri, 05 May 2023 00:40:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Fri, 05 May 2023 00:40:49 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 05 May 2023 00:42:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 05 May 2023 00:42:10 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 05 May 2023 00:42:10 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Fri, 05 May 2023 00:42:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 05 May 2023 00:42:11 GMT
EXPOSE 3000
# Fri, 05 May 2023 00:42:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8e4cb8eb5d7a86a02dfc1d3645e982def0fc1c20e1fd14d9c6736177d3887dfa`  
		Last Modified: Wed, 03 May 2023 03:44:59 GMT  
		Size: 29.6 MB (29642157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c85c36d736a741c38ab8f15dcfcc6ff4e3c646f366ca5f65e719909dfe9768`  
		Last Modified: Wed, 03 May 2023 22:09:45 GMT  
		Size: 8.9 MB (8864272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b9219b2994019ebc532bc44762bbf36886fb5c730fcafff35d5dfb0f7729d1`  
		Last Modified: Wed, 03 May 2023 22:09:43 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1329b46a7de8d57420aa0dfebc892de87417c6cc160ba0ddd470c91301f0a1`  
		Last Modified: Wed, 03 May 2023 22:10:32 GMT  
		Size: 32.4 MB (32445002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a973ba0b0831bb784dfb28bf6ec41e765fc02397564fe9e620c0dc53ef8b28`  
		Last Modified: Wed, 03 May 2023 22:10:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549364cdf15baecbf9a30aa3e1a216e443eb2bd02e5e84c2ad7eadc138395e3`  
		Last Modified: Fri, 05 May 2023 00:49:47 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bff09a12faf47175fd02a4c6b8ccb068c69392ea69476bc0f244090c9c2ad5e`  
		Last Modified: Fri, 05 May 2023 00:50:01 GMT  
		Size: 99.1 MB (99100192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdf15d9179c735efd6dfadf4f8ca91acfc01191d39ecd6598253ccd52952fc8`  
		Last Modified: Fri, 05 May 2023 00:49:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f0714a99caf5dcb1f3d634158fb925422c45935d08ec0424b03388b6d73005`  
		Last Modified: Fri, 05 May 2023 00:49:46 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34a2c6ddb27aca4fd572737fcadd412f4b594b3e98da3ac6f6dc90a128d0d8f`  
		Last Modified: Fri, 05 May 2023 00:49:47 GMT  
		Size: 3.1 MB (3144721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8766990f97006e1b54481c5f9e0b9889661d791de2d4505d3090cef44b6b236a`  
		Last Modified: Fri, 05 May 2023 00:49:53 GMT  
		Size: 73.1 MB (73074377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfee9e85dd2e33df803b3816617dbbda54384bbe69232491f0cbf373110823`  
		Last Modified: Fri, 05 May 2023 00:49:46 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
