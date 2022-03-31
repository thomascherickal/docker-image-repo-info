## `hylang:pypy3.7-buster`

```console
$ docker pull hylang@sha256:2c7106671e54e6a3666ddbdc9a790a20d0220ad484adfe20357dfff346aedf4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:9a5acd8b2cacc27cc04896f3eca82eb6310504c37cf8d0a12abda0af4359435b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71244263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf682da3739e2d619babe662e742a8ae4ba1fe8af0292d30529f3b43147b4d4`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:15:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:15:38 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:15:38 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 18:15:38 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 29 Mar 2022 18:21:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='639c76f128a856747aee23a34276fa101a7a157ea81e76394fbaf80b97dcf2f2'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 29 Mar 2022 18:21:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 29 Mar 2022 18:21:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 29 Mar 2022 18:22:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Mar 2022 18:22:03 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 14:01:20 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 14:01:20 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 14:01:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 14:01:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403755530240b815f3bec242ebade359d2edf509c46f7eb0871f6a479be008bc`  
		Last Modified: Tue, 29 Mar 2022 18:27:12 GMT  
		Size: 2.8 MB (2765092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2615ee5d508b2bb1f9d67d0a3f69b9764dff1a7455e897a6e53a0f363a232ce7`  
		Last Modified: Tue, 29 Mar 2022 18:31:30 GMT  
		Size: 36.4 MB (36410557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc9ba81d6b36f6044eaa162b37da3fa3f119824140592ee3d2af2ca12e387b3`  
		Last Modified: Tue, 29 Mar 2022 18:31:25 GMT  
		Size: 2.4 MB (2367715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a029d03f7fc3c1d7a1e7ae4aa96d538d54ed66eb1828a622325a138343abab7`  
		Last Modified: Wed, 30 Mar 2022 14:07:35 GMT  
		Size: 2.5 MB (2548929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:4ba5028d53889fed96d7c25616ed9762ff0da794756e880b9c0627ff647e5b66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66575283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd445638aada34408f3686bc29cc1963b26610559c9149053ca3184f2429d3bb`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:50:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:50:34 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:50:35 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 04:50:36 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 30 Mar 2022 04:58:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='639c76f128a856747aee23a34276fa101a7a157ea81e76394fbaf80b97dcf2f2'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 30 Mar 2022 04:58:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 04:58:51 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 04:59:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 30 Mar 2022 04:59:07 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 19:27:15 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 19:27:16 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 19:27:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 19:27:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f753e27a948649e02cce274d9571a644d98c11dadffc8f18b18b2cc73e5e5`  
		Last Modified: Wed, 30 Mar 2022 05:07:51 GMT  
		Size: 2.6 MB (2634640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9950698b47b9ca74791661d97a4ca5fbc01484f6586f823e477b8c2de81eef`  
		Last Modified: Wed, 30 Mar 2022 05:12:44 GMT  
		Size: 33.3 MB (33316262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22ef030cbb2465366c0f5ac6289c5dc86e98adb811712c2fb62adb438e72c73`  
		Last Modified: Wed, 30 Mar 2022 05:12:37 GMT  
		Size: 2.2 MB (2155282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2cac379f08231e065633b057ee0ec7187bd68a3213009af2332bf586f5d580`  
		Last Modified: Wed, 30 Mar 2022 19:35:41 GMT  
		Size: 2.5 MB (2549322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:f7896f8168fb4e2afd02f7e733b5fe80a10d1b3d35c2a3f2b38c6f2312ce5ed7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75587281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd720bb1601093376571a2ba461c2761fb93ecb54288a4373989b91138f50df`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:28:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:28:01 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 17:28:02 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 17:42:50 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 30 Mar 2022 17:50:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 30 Mar 2022 17:50:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 17:50:34 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 17:50:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 30 Mar 2022 17:50:48 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 19:03:22 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 19:03:22 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 19:03:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 19:03:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233e5959675f3ed65989a324abc0c6349cc5b162d62ab68997dc30e78dcc3684`  
		Last Modified: Tue, 29 Mar 2022 17:44:18 GMT  
		Size: 2.8 MB (2777530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7facf497ce4670220ce93f55351bbb0b2f9afb888c13a6ea1f1aa27a60382ba9`  
		Last Modified: Wed, 30 Mar 2022 18:04:20 GMT  
		Size: 39.1 MB (39088622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41142594a6b96ff371dfcbe0da0bc5e88dd3b8f32711f608b10d39a0393d6044`  
		Last Modified: Wed, 30 Mar 2022 18:04:14 GMT  
		Size: 2.7 MB (2748539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8ceb22b0ff207deae050919ebcbe603f07060399104eaa513ca7b726bcea9`  
		Last Modified: Wed, 30 Mar 2022 19:08:03 GMT  
		Size: 3.2 MB (3171338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; s390x

```console
$ docker pull hylang@sha256:80c79fbd75bd7832aaf0d395ab5d8885133c6799db66a12428a08a15c042aefd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69209444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9bca4750b44983fcfaeaa405fc3b0f0ed1cefb61cb35d42f72541b327211db`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:45:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:45:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:45:56 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 19:49:49 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 30 Mar 2022 19:52:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 30 Mar 2022 19:52:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 19:52:54 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 19:53:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 30 Mar 2022 19:53:04 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 20:25:01 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 20:25:01 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 20:25:05 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 20:25:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9dc374da413c966df05615366012e350a2cac2c3f3b280e253d3df4b0effa`  
		Last Modified: Wed, 30 Mar 2022 04:52:20 GMT  
		Size: 2.5 MB (2457211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8c77ff423f9abd5c55eac34de3e9f88bb493bba75927924952de40f16d6fed`  
		Last Modified: Wed, 30 Mar 2022 19:57:44 GMT  
		Size: 34.8 MB (34848388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27530cc5f6d91055c89d69e8cb9738d524833b3ac615a3fd4517c15927a18cb9`  
		Last Modified: Wed, 30 Mar 2022 19:57:38 GMT  
		Size: 3.0 MB (2966343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e565d4d0859d19983ba617ab8ac42efae77ad64827b421d241fe8eb64d904d0`  
		Last Modified: Wed, 30 Mar 2022 20:28:26 GMT  
		Size: 3.2 MB (3171586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
