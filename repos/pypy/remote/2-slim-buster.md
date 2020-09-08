## `pypy:2-slim-buster`

```console
$ docker pull pypy@sha256:604c865072254f17d60720d72f72ef9eda682d31f85b604e08445fd4253ff528
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-slim-buster` - linux; amd64

```console
$ docker pull pypy@sha256:c44fb0ed9d9662a6ba97fa6ebc37d440cc1240434ab9b98280f224da76b95192
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69375761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03c03aefd7478750ef1f186153349cbfa03f2c9fff81b9c60326b2193b8f57a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:28:23 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 06:28:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:28:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 06:28:30 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 05 Aug 2020 06:29:00 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='be74886547df7bf7094096a11fc0a48496779d0d1b71901797b0c816f92caca3' ;; 		arm64) pypyArch='aarch64'; sha256='094f23ab262e666d8740bf27459a6b1215a628dad9b6c2a88f1ed5c793fab267' ;; 		i386) pypyArch='linux32'; sha256='cd155d06cd0956d9de4a16e8a6bdf0722cb45b5bc4bbf805825d393ebd6690ad' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Sep 2020 20:27:34 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:27:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:27:35 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:27:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:27:50 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba752debb3c3e0ed5c7d24db21b2548297fed7d74e1da6804f764e5c63d18fff`  
		Last Modified: Wed, 05 Aug 2020 06:31:52 GMT  
		Size: 2.7 MB (2742465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271d699913ca86dd3baf29e254e6fe265d8f7de61efa3699abe11c98184b7a1f`  
		Last Modified: Wed, 05 Aug 2020 06:31:59 GMT  
		Size: 37.3 MB (37317300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8fa1a2a1d8de134c0a1f990c3a5c522a2fe68abc794190ccca8d458dddeda4`  
		Last Modified: Tue, 08 Sep 2020 20:29:34 GMT  
		Size: 2.2 MB (2223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:bc747ac787ef925c6bf0bb0c90a25b75cf0e03a7fb5ea25db12c333ebcc4ec94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61667631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3561aeccb974afa811237d54eff52a10018acf52668419d5e288cb37bf29e5ac`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:53:00 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 09:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 09:53:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Aug 2020 09:53:27 GMT
ENV PYPY_VERSION=7.3.1
# Tue, 04 Aug 2020 09:54:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='be74886547df7bf7094096a11fc0a48496779d0d1b71901797b0c816f92caca3' ;; 		arm64) pypyArch='aarch64'; sha256='094f23ab262e666d8740bf27459a6b1215a628dad9b6c2a88f1ed5c793fab267' ;; 		i386) pypyArch='linux32'; sha256='cd155d06cd0956d9de4a16e8a6bdf0722cb45b5bc4bbf805825d393ebd6690ad' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 11 Aug 2020 20:11:01 GMT
ENV PYTHON_PIP_VERSION=20.2.2
# Tue, 11 Aug 2020 20:11:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5578af97f8b2b466f4cdbebe18a3ba2d48ad1434/get-pip.py
# Tue, 11 Aug 2020 20:11:02 GMT
ENV PYTHON_GET_PIP_SHA256=d4d62a0850fe0c2e6325b2cc20d818c580563de5a2038f917e3cb0e25280b4d1
# Tue, 11 Aug 2020 20:11:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 11 Aug 2020 20:11:39 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ead8238ab6c3577178d87cecdfba4724b27518c235f3c352ca7b7232df97e0`  
		Last Modified: Tue, 04 Aug 2020 09:59:20 GMT  
		Size: 2.6 MB (2606653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6657ed95bb4f2beacbcc1699b4755309e8352a4e424af73c6d48db32319`  
		Last Modified: Tue, 04 Aug 2020 09:59:32 GMT  
		Size: 31.0 MB (30993199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2bdfc02629f957b9ce4ec20967de37862a87c2565c0437d993b02836059f1b`  
		Last Modified: Tue, 11 Aug 2020 20:14:38 GMT  
		Size: 2.2 MB (2218478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim-buster` - linux; 386

```console
$ docker pull pypy@sha256:b73bd3618c06be6eb6db247b22c8c2d537e5c6886e16aa8cd59dc5ea17180f79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72096968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d716abc328b2c5e5aa41a2e7cf4284db92be91b9def62b5dfd278ac429cca046`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:20:59 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 06:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:21:07 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Aug 2020 06:21:07 GMT
ENV PYPY_VERSION=7.3.1
# Tue, 04 Aug 2020 06:21:43 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='be74886547df7bf7094096a11fc0a48496779d0d1b71901797b0c816f92caca3' ;; 		arm64) pypyArch='aarch64'; sha256='094f23ab262e666d8740bf27459a6b1215a628dad9b6c2a88f1ed5c793fab267' ;; 		i386) pypyArch='linux32'; sha256='cd155d06cd0956d9de4a16e8a6bdf0722cb45b5bc4bbf805825d393ebd6690ad' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Sep 2020 20:15:18 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:15:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:15:18 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:15:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:15:34 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cfccc3b3781d496a79401f47d7ccd4157a669c743cd881c94902078a99e67`  
		Last Modified: Tue, 04 Aug 2020 06:23:35 GMT  
		Size: 2.8 MB (2752668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449c59074caf5760b551a2b68d25b6b06772e0508c1396dcec5d1b719b91664`  
		Last Modified: Tue, 04 Aug 2020 06:23:48 GMT  
		Size: 39.4 MB (39370386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb4dbe6237bdc699a88c5c23e2abc547df19d2476ce47e2dba1102da0575d4`  
		Last Modified: Tue, 08 Sep 2020 20:17:10 GMT  
		Size: 2.2 MB (2223479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
