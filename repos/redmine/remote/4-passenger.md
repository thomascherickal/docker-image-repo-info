## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:424e4987c0f49f25a2df24f161441ef7f2fc0b375af0665b8fd0a50377fa34c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:6a577274370f7bc1ff42bfc30d254f2c6e5aadff9c0fb037570f8298f0881943
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221561354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7345150dd10d55edaf970b808125f8bb3d857e72bf89404a49e2c1bdf38adb8d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:41:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 21:41:19 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 21:55:32 GMT
ENV RUBY_MAJOR=2.7
# Tue, 28 Sep 2021 21:55:32 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 28 Sep 2021 21:55:32 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 28 Sep 2021 21:58:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 21:58:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 21:58:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 21:58:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 21:58:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 21:58:27 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 16:08:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 29 Sep 2021 16:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 16:08:35 GMT
ENV RAILS_ENV=production
# Wed, 29 Sep 2021 16:08:35 GMT
WORKDIR /usr/src/redmine
# Wed, 29 Sep 2021 16:08:35 GMT
ENV HOME=/home/redmine
# Wed, 29 Sep 2021 16:08:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 29 Sep 2021 16:08:36 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 29 Sep 2021 16:08:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 29 Sep 2021 16:08:40 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 29 Sep 2021 16:09:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 29 Sep 2021 16:09:23 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 29 Sep 2021 16:09:23 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 29 Sep 2021 16:09:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:09:24 GMT
EXPOSE 3000
# Wed, 29 Sep 2021 16:09:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 05 Oct 2021 22:30:11 GMT
ENV PASSENGER_VERSION=6.0.11
# Tue, 05 Oct 2021 22:30:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 22:30:29 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 05 Oct 2021 22:30:29 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 05 Oct 2021 22:30:29 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ffc2b068dcf8bed3fb22144e2af726eae3099dfa5c9a7c680e160e47cdbdb6`  
		Last Modified: Tue, 28 Sep 2021 22:15:44 GMT  
		Size: 12.6 MB (12564885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561aa5343e7e066141608c846bebfe035065b891cde50b2d1664d9938761d4d3`  
		Last Modified: Tue, 28 Sep 2021 22:15:39 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fca37ce891f690115fb75fe23f19ae78346453e7e7da1fc9dc27c47a4c9c37`  
		Last Modified: Tue, 28 Sep 2021 22:17:12 GMT  
		Size: 14.5 MB (14510180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8bad6809ef5df2f7a86d81038e531723dce749b2ba5d5169fd3b9667c1df21`  
		Last Modified: Tue, 28 Sep 2021 22:17:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87208e51b23f88c6f70dd3143a3a996f57b6b99f5f5bae5adc706af8796709`  
		Last Modified: Wed, 29 Sep 2021 16:15:23 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08394d798ba760ff50f4d04b7751d7aaa112f12f648202579c405a24d99c0ca8`  
		Last Modified: Wed, 29 Sep 2021 16:15:37 GMT  
		Size: 94.1 MB (94088247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a8fdce22982d9f341c9cba735709050a7b6c925d8cc4a364c189803033fbcf`  
		Last Modified: Wed, 29 Sep 2021 16:15:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be063625f37fde0c6ed3289d307caf760a920758f99c3e03625f24e2c03b8ec`  
		Last Modified: Wed, 29 Sep 2021 16:15:20 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96e70c9b332901ab07d690b69e5815ee485eed91403cc997f224123735d1790`  
		Last Modified: Wed, 29 Sep 2021 16:15:20 GMT  
		Size: 3.1 MB (3061922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945632f36157723a827cd841709e83522032c6cbff248fca6ee34127ac446478`  
		Last Modified: Wed, 29 Sep 2021 16:15:25 GMT  
		Size: 44.1 MB (44129495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcd16cbee8a7b241d654f42267289731f7b821b26255331f07fa4eb5a96eea3`  
		Last Modified: Wed, 29 Sep 2021 16:15:19 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeea1b28f1f3f67f495844037e65a49b769ab07443d4255a22b97fdeedc3911d`  
		Last Modified: Tue, 05 Oct 2021 22:32:01 GMT  
		Size: 21.1 MB (21137107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113de2e797d61dda326d0d01c8f30dcd6dddc423032997a5f13836e382d9228c`  
		Last Modified: Tue, 05 Oct 2021 22:31:59 GMT  
		Size: 4.9 MB (4919286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
