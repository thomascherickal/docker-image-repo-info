## `plone:latest`

```console
$ docker pull plone@sha256:3a7f88157dfb725b2fc2f760e59e8995a805b4370dd5ea0ea541e5eb4ddc5912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `plone:latest` - linux; amd64

```console
$ docker pull plone@sha256:aebee5b0e1d6a34a852f798a796b3752617ed603afdf51d5e36be33ec3d039b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244385799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8ad26ae56f530270aab4d028485bef67b435efe5d8525abf12f5a8385a5b54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:26:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 12:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 12:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 14:22:00 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 14:50:21 GMT
ENV PYTHON_VERSION=3.8.13
# Tue, 29 Mar 2022 14:57:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 29 Mar 2022 14:57:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 14:57:34 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 14:57:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 29 Mar 2022 14:57:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 14:57:35 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 14:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 14:57:47 GMT
CMD ["python3"]
# Wed, 30 Mar 2022 14:08:16 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.5 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.7 PLONE_VERSION_RELEASE=Plone-5.2.7-UnifiedInstaller-1.0 PLONE_MD5=c180d7ce3170b1871a7e8d53938096b1
# Wed, 30 Mar 2022 14:08:17 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 30 Mar 2022 14:08:17 GMT
COPY file:7b22c8ff5914ecee959543c0622bbb71de3b59961836e6f0bad3c41c35197e25 in /plone/instance/ 
# Wed, 30 Mar 2022 14:12:36 GMT
RUN buildDeps="default-libmysqlclient-dev dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libldap2-dev libopenjp2-7-dev libpcre3-dev libpq-dev libsasl2-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="default-libmysqlclient-dev git gosu libjpeg62 libopenjp2-7 libpq5 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 30 Mar 2022 14:12:39 GMT
VOLUME [/data]
# Wed, 30 Mar 2022 14:12:39 GMT
COPY multi:fb30eb2e09be8af3f02c6ae43c3107721065efb27e2804bf29977286bb96d490 in / 
# Wed, 30 Mar 2022 14:12:39 GMT
EXPOSE 8080
# Wed, 30 Mar 2022 14:12:40 GMT
WORKDIR /plone/instance
# Wed, 30 Mar 2022 14:12:40 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 30 Mar 2022 14:12:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 30 Mar 2022 14:12:40 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f192ed04782b15b45c31ce33d4fd7f8a80041ff0cfa31c95e7cd750fc396f7`  
		Last Modified: Tue, 29 Mar 2022 15:42:21 GMT  
		Size: 2.8 MB (2779103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e7b7dc56b7a621e7cc3599b145a8535ad965602abf6ccbeafb34d38e67ab32`  
		Last Modified: Tue, 29 Mar 2022 15:45:41 GMT  
		Size: 11.3 MB (11289540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d931cd7e647a12910eb509471d193ce6f19fb1f261b8632face8dad9749404c3`  
		Last Modified: Tue, 29 Mar 2022 15:45:39 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0372c15f94026a2184cb24894401ff9e832ab7840e2e792cd98c448f19a39266`  
		Last Modified: Tue, 29 Mar 2022 15:45:40 GMT  
		Size: 3.2 MB (3166327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da91c4c02a78841d816d4c8342b9b30fb3a17534e8a5d049071b2ddf58e05218`  
		Last Modified: Wed, 30 Mar 2022 14:13:06 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f79f2b845233b1577209e9e8c9df4cdd3896c0a7135a6fdf277735dbcf2a7a`  
		Last Modified: Wed, 30 Mar 2022 14:13:06 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec07299a80de2785ecc7c5ffc37865b43307c1b8da05ca6ac67c6b914d66b0`  
		Last Modified: Wed, 30 Mar 2022 14:13:35 GMT  
		Size: 200.0 MB (199989396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4556e469128adbf31a6fc9b51027228331829cc56fb82d48cc809e181b257e01`  
		Last Modified: Wed, 30 Mar 2022 14:13:06 GMT  
		Size: 4.0 KB (4022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
