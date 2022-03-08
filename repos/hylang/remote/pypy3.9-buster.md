## `hylang:pypy3.9-buster`

```console
$ docker pull hylang@sha256:3dfc6369f45ca30fb1a7c44c57ccd6cce5ec3942194006fc204309af72a27b47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.9-buster` - linux; amd64

```console
$ docker pull hylang@sha256:f08a7790f190aee08f3e2590559475d3c85fdddf885aa62c1446eff1c3e1dc0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72625901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1bb75b6096e1dbc8b912b34b2aa45062bf04db4830ccf90f0a2fffb5fa3c83c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:42:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 01:42:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 01:42:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 01:42:33 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 05:17:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='b7282bc4484bceae5bc4cc04e05ee4faf51cb624c8fc7a69d92e5fdf0d0c96aa'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 05:17:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 05:17:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 05:17:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 05:17:36 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 09:18:24 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 09:18:24 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 09:18:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 09:18:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3cc5174486607f75e34ab6b618d1189a85876dcd67167b29afccc8bcbcfe17`  
		Last Modified: Wed, 02 Mar 2022 01:56:23 GMT  
		Size: 2.8 MB (2757894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9a2f7fd9d503c6d36622a130bcc22398830a121557dd31a00154a40d5f1f39`  
		Last Modified: Tue, 08 Mar 2022 05:28:02 GMT  
		Size: 37.2 MB (37244779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5cf98468a97fec37203601fe654d65fff6799c816ee789356de43c6faf48c7`  
		Last Modified: Tue, 08 Mar 2022 05:27:56 GMT  
		Size: 2.6 MB (2635175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eb5a886380b3d97d0c840fbb9ac66a3fd389fc2eb4a5a983df2665ee7e4541`  
		Last Modified: Tue, 08 Mar 2022 11:04:15 GMT  
		Size: 2.8 MB (2834316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-buster` - linux; 386

```console
$ docker pull hylang@sha256:c0ca337a3c685dc43cc9307639043b8db6eeba5b53f1a17b7f0fcc7b36e014e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75256271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff24a42979d34ebc66609abae98641b27af6f9f4903905320073678ee572f8c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:20:32 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 21:20:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 21:20:33 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 03:58:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='b7282bc4484bceae5bc4cc04e05ee4faf51cb624c8fc7a69d92e5fdf0d0c96aa'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 03:58:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 03:58:26 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 03:58:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 03:58:39 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 04:32:22 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 04:32:22 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 04:32:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 04:32:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2fa69f8281d0c88d1c268092ba8dbb609cfa2a0eeb0b72e7acfdc35b5c255d`  
		Last Modified: Tue, 01 Mar 2022 21:40:45 GMT  
		Size: 2.8 MB (2769490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c27108eff009c46f6a914cd1ef7e281ec32c7c4ae3d0251a51f199b7be2548`  
		Last Modified: Tue, 08 Mar 2022 04:13:27 GMT  
		Size: 39.2 MB (39213194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a710020d0f3894193676b998c71e403511ee2d2ceb39615e583b38ceb52dad`  
		Last Modified: Tue, 08 Mar 2022 04:13:18 GMT  
		Size: 2.6 MB (2634795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ad56d03fc6fe8cf7a2cd2c04e73ddbbac06f1b176fe0f34c26d6dde7ca8ecc`  
		Last Modified: Tue, 08 Mar 2022 04:40:16 GMT  
		Size: 2.8 MB (2834202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-buster` - linux; s390x

```console
$ docker pull hylang@sha256:41ab692f0f089ec3f5a67692ee049be35739c9d982dd46f0fdaacd0cc8537141
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68790283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac54054a642715f304c8977dc789fc1a292b9ca1883d6f5024360e4fce18cd7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:27 GMT
ADD file:908bd36a2b17b792aa02339ed6a72d1051267279d72330b1c5cd8617ca5d819e in / 
# Tue, 01 Mar 2022 02:02:28 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:13:42 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 10:13:42 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 10:13:42 GMT
ENV PYPY_VERSION=7.3.8
# Mon, 07 Mar 2022 23:49:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='b7282bc4484bceae5bc4cc04e05ee4faf51cb624c8fc7a69d92e5fdf0d0c96aa'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 07 Mar 2022 23:49:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 07 Mar 2022 23:49:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 07 Mar 2022 23:49:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 07 Mar 2022 23:49:21 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 04:50:55 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 04:50:55 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 04:50:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 04:51:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cb73b674076b2da947cefa0692c1d193bda8bfd443c178f9bb39bbae7656ead8`  
		Last Modified: Tue, 01 Mar 2022 02:08:05 GMT  
		Size: 25.8 MB (25769053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09aaf957a3af05d974bd1245a06df174f1c8119b5cc605286be610ed8ae423b`  
		Last Modified: Tue, 01 Mar 2022 10:18:37 GMT  
		Size: 2.5 MB (2452746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aca0218d34fa026b36d96f61108f7775b90aa213209924a5563ef21ca3d6d3`  
		Last Modified: Tue, 08 Mar 2022 04:32:47 GMT  
		Size: 35.1 MB (35099199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315d082636d380ff832416a003be99780136fe90c1dbfb94c31471170b1a267a`  
		Last Modified: Tue, 08 Mar 2022 04:32:41 GMT  
		Size: 2.6 MB (2635070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb500b990d64a327b078b99bd79d94ab88f6774e9a4974a893c65ddfa01fe5e`  
		Last Modified: Tue, 08 Mar 2022 04:55:55 GMT  
		Size: 2.8 MB (2834215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
