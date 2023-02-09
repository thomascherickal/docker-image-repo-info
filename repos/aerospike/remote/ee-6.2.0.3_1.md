## `aerospike:ee-6.2.0.3_1`

```console
$ docker pull aerospike@sha256:3362c9853fa6ade63d5edbfc847cf7127119f2f4c0a5da1fc921a3bba021b536
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `aerospike:ee-6.2.0.3_1` - linux; amd64

```console
$ docker pull aerospike@sha256:8f9abde565eb8381ee108bc173987517f2718b94679d67579d28c742d74b733b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81183549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaf8a8e5fb166b39f7533d07eb2579baf700bc306cc44b7ccc7685abee4a880`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:06:47 GMT
ARG AEROSPIKE_EDITION=enterprise
# Thu, 09 Feb 2023 09:06:47 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
# Thu, 09 Feb 2023 09:06:47 GMT
ARG AEROSPIKE_SHA_X86_64=2c3cd14843a62aaaf158dcab1e16f16050e170a0d591fdb56805defb93a8e5bf
# Thu, 09 Feb 2023 09:06:47 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz
# Thu, 09 Feb 2023 09:06:47 GMT
ARG AEROSPIKE_SHA_AARCH64=367357112e4da434814617dad19cc5c0cf8211de67384a161a3511b2a86453da
# Thu, 09 Feb 2023 09:06:48 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 09 Feb 2023 09:07:12 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz AEROSPIKE_EDITION=enterprise AEROSPIKE_SHA_AARCH64=367357112e4da434814617dad19cc5c0cf8211de67384a161a3511b2a86453da AEROSPIKE_SHA_X86_64=2c3cd14843a62aaaf158dcab1e16f16050e170a0d591fdb56805defb93a8e5bf AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+([.][0-9]+){2,3}/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 09 Feb 2023 09:07:13 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 09 Feb 2023 09:07:13 GMT
EXPOSE 3000 3001 3002
# Thu, 09 Feb 2023 09:07:13 GMT
COPY file:d50c4b59c6030f47e41221b7d152a3e0cf299b7e8bf38ea42e3c2e33b1c9cc1f in /entrypoint.sh 
# Thu, 09 Feb 2023 09:07:13 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 09 Feb 2023 09:07:13 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353c69f7226ee2d4f457569836ec13776b7552573f194c1bc531065f03c370e3`  
		Last Modified: Thu, 09 Feb 2023 09:07:58 GMT  
		Size: 49.8 MB (49769547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a7e3d75542a2d5e20cb81f25163e638e69c6d89f5aea92285197160455353`  
		Last Modified: Thu, 09 Feb 2023 09:07:51 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86d874fd9f200c8981d7f2d3fc162742a9799bf8991ac4e9b0f0d5de052bb41`  
		Last Modified: Thu, 09 Feb 2023 09:07:50 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `aerospike:ee-6.2.0.3_1` - linux; arm64 variant v8

```console
$ docker pull aerospike@sha256:be1cde79abb12034654a8706208b8020ea3a97aa9f4cde3eec7c95ab0ab03212
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78500825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0a5c359f5e1a5035c6bee301c904b0afbe64e41779205c89645139c9e8bd26`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:02:47 GMT
ARG AEROSPIKE_EDITION=enterprise
# Thu, 09 Feb 2023 09:02:47 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
# Thu, 09 Feb 2023 09:02:47 GMT
ARG AEROSPIKE_SHA_X86_64=2c3cd14843a62aaaf158dcab1e16f16050e170a0d591fdb56805defb93a8e5bf
# Thu, 09 Feb 2023 09:02:47 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz
# Thu, 09 Feb 2023 09:02:47 GMT
ARG AEROSPIKE_SHA_AARCH64=367357112e4da434814617dad19cc5c0cf8211de67384a161a3511b2a86453da
# Thu, 09 Feb 2023 09:02:47 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 09 Feb 2023 09:03:05 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz AEROSPIKE_EDITION=enterprise AEROSPIKE_SHA_AARCH64=367357112e4da434814617dad19cc5c0cf8211de67384a161a3511b2a86453da AEROSPIKE_SHA_X86_64=2c3cd14843a62aaaf158dcab1e16f16050e170a0d591fdb56805defb93a8e5bf AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.2.0.3/aerospike-server-enterprise_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+([.][0-9]+){2,3}/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 09 Feb 2023 09:03:05 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 09 Feb 2023 09:03:05 GMT
EXPOSE 3000 3001 3002
# Thu, 09 Feb 2023 09:03:06 GMT
COPY file:d50c4b59c6030f47e41221b7d152a3e0cf299b7e8bf38ea42e3c2e33b1c9cc1f in /entrypoint.sh 
# Thu, 09 Feb 2023 09:03:06 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 09 Feb 2023 09:03:06 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80df0d9b8418bac049e0e7cf04c8817f5d29369a114bf61d08f7a2fd651603`  
		Last Modified: Thu, 09 Feb 2023 09:03:50 GMT  
		Size: 48.4 MB (48436127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8d9af8dc9582d3c2d26b29d135b5fdf05aec6f5ce11bbeefe22a81a3d55e`  
		Last Modified: Thu, 09 Feb 2023 09:03:42 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc39bbb7b499c57cd6c8f2bed54f01fcfaadd57fd1ef87521813eb89637f303d`  
		Last Modified: Thu, 09 Feb 2023 09:03:42 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
