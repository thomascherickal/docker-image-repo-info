## `hylang:0-pypy3.7-buster`

```console
$ docker pull hylang@sha256:1ff277a2700a29a1c4b1a48f982dca13ec97c0011ac9bf4303382a4bcc86f9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `hylang:0-pypy3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:9da6312189cc06dfbe916842ec310ec40ea009c9e7bbf93d268b23838457044d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76456799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7966e5baf74c40bc8b9ca6c4017664061894a2da803d8d3e4c1a65fe359c44`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:22:22 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:22:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Sep 2020 22:29:30 GMT
ENV PYPY_VERSION=7.3.2
# Fri, 25 Sep 2020 22:33:45 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='a285ddcbc909d68c648585fae4f33b0ba24961bb4e8fafe5874cf725d6e83df6' ;; 		arm64) pypyArch='aarch64'; sha256='c5c35a37917f759c19e2a6b3df3b4d56298faa2fae83c143469bcbda42ca5dd2' ;; 		i386) pypyArch='linux32'; sha256='34c7e1c7bd06e437ad43cc90a20f9444be1f0a264d0955e32098294c30274784' ;; 		s390x) pypyArch='s390x'; sha256='d4ce71ebba148bf83c24fc963e8282c9b7f0c81fcf6b612301b8efe6bd7658d1' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 25 Sep 2020 22:33:46 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Fri, 25 Sep 2020 22:33:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Fri, 25 Sep 2020 22:33:46 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Fri, 25 Sep 2020 22:34:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 25 Sep 2020 22:34:04 GMT
CMD ["pypy3"]
# Sat, 26 Sep 2020 01:05:39 GMT
ENV HY_VERSION=0.19.0
# Sat, 26 Sep 2020 01:05:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 26 Sep 2020 01:05:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4188f53dca4cf8543c8c5c4056a7c31bd176fd2b356c3a55f9189834ab833c2c`  
		Last Modified: Thu, 10 Sep 2020 15:27:40 GMT  
		Size: 2.8 MB (2752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b06467c3f9e1d379aaac24914114e65df760748da49c16d96e0aa2c5d977db`  
		Last Modified: Fri, 25 Sep 2020 22:37:15 GMT  
		Size: 40.4 MB (40407143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e8437252d64f1747427723fe20cd4b635ef40665ab9532bde84dd24ad5913b`  
		Last Modified: Fri, 25 Sep 2020 22:37:01 GMT  
		Size: 2.5 MB (2546840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6698852fc22048f548227655e01e380f8e09e3f0526a9b882302488a3e490441`  
		Last Modified: Sat, 26 Sep 2020 01:07:11 GMT  
		Size: 3.0 MB (2999795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7-buster` - linux; s390x

```console
$ docker pull hylang@sha256:a1b2369450b974f80404e7d061eb298510e79b2d1119a26fac142746198da4c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68767914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef48063baa09a70758161306db2ca80d9916433bc8a339f89f34c3c170e3f11`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:34:35 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 04:34:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:34:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Sep 2020 21:59:12 GMT
ENV PYPY_VERSION=7.3.2
# Fri, 25 Sep 2020 22:00:49 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='a285ddcbc909d68c648585fae4f33b0ba24961bb4e8fafe5874cf725d6e83df6' ;; 		arm64) pypyArch='aarch64'; sha256='c5c35a37917f759c19e2a6b3df3b4d56298faa2fae83c143469bcbda42ca5dd2' ;; 		i386) pypyArch='linux32'; sha256='34c7e1c7bd06e437ad43cc90a20f9444be1f0a264d0955e32098294c30274784' ;; 		s390x) pypyArch='s390x'; sha256='d4ce71ebba148bf83c24fc963e8282c9b7f0c81fcf6b612301b8efe6bd7658d1' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 25 Sep 2020 22:00:51 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Fri, 25 Sep 2020 22:00:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Fri, 25 Sep 2020 22:00:52 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Fri, 25 Sep 2020 22:01:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 25 Sep 2020 22:01:03 GMT
CMD ["pypy3"]
# Sat, 26 Sep 2020 01:05:53 GMT
ENV HY_VERSION=0.19.0
# Sat, 26 Sep 2020 01:06:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 26 Sep 2020 01:06:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25730a1e3b8989c53b55fae2816f43912b41a14a52a44f5c864cc37548d898b3`  
		Last Modified: Thu, 10 Sep 2020 04:36:21 GMT  
		Size: 2.4 MB (2432841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218f127ecf2887a803b29b033d60cc39d86e3b5b0c6509117be775b7089605b8`  
		Last Modified: Fri, 25 Sep 2020 22:03:03 GMT  
		Size: 35.1 MB (35080472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bd2553d7cf8b29fdd2b89d1a1ad3b2798642740c7a562d6e7ac8ffd1d8fe37`  
		Last Modified: Fri, 25 Sep 2020 22:02:56 GMT  
		Size: 2.5 MB (2547238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a1027cadc0edc4d76ba574d162f0147c47df3099cb8691cf31638bccd7f87`  
		Last Modified: Sat, 26 Sep 2020 01:07:10 GMT  
		Size: 3.0 MB (2999766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
