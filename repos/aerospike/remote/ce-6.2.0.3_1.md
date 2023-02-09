## `aerospike:ce-6.2.0.3_1`

```console
$ docker pull aerospike@sha256:8a7201a36705ea066ffd635d5aba07c0eb8cde6225ab2b36efa5e3935442110f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `aerospike:ce-6.2.0.3_1` - linux; amd64

```console
$ docker pull aerospike@sha256:914926a00eb88743c3793db45ab8088be93cae5492914ea2f759e29527822e84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78160564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2450695c4c52b0f0ec1927af8e9e80f420b157677e2e132bb0642df94a2d50e4`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:07:15 GMT
ARG AEROSPIKE_EDITION=community
# Thu, 09 Feb 2023 09:07:16 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
# Thu, 09 Feb 2023 09:07:16 GMT
ARG AEROSPIKE_SHA_X86_64=622b7b8d694a54ee42515bc56aa9aeb006c1f731b10df82777cbf1f154b12fff
# Thu, 09 Feb 2023 09:07:16 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz
# Thu, 09 Feb 2023 09:07:16 GMT
ARG AEROSPIKE_SHA_AARCH64=7218303567741912537b564cf50580d37b84b615aa01965ecfba20596ccfb594
# Thu, 09 Feb 2023 09:07:16 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 09 Feb 2023 09:07:37 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz AEROSPIKE_EDITION=community AEROSPIKE_SHA_AARCH64=7218303567741912537b564cf50580d37b84b615aa01965ecfba20596ccfb594 AEROSPIKE_SHA_X86_64=622b7b8d694a54ee42515bc56aa9aeb006c1f731b10df82777cbf1f154b12fff AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+([.][0-9]+){2,3}/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 09 Feb 2023 09:07:38 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 09 Feb 2023 09:07:38 GMT
EXPOSE 3000 3001 3002
# Thu, 09 Feb 2023 09:07:38 GMT
COPY file:d50c4b59c6030f47e41221b7d152a3e0cf299b7e8bf38ea42e3c2e33b1c9cc1f in /entrypoint.sh 
# Thu, 09 Feb 2023 09:07:38 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 09 Feb 2023 09:07:38 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8cdef96fbabb3e8dba24c36784e8ade347b81d5a3dd0fa53efc94fe6abc29`  
		Last Modified: Thu, 09 Feb 2023 09:08:14 GMT  
		Size: 46.7 MB (46746566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa03ea0e039849b9a1180811b913d821849d882a58ebfcedba9519987292229`  
		Last Modified: Thu, 09 Feb 2023 09:08:07 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c1a01c10e6b0a6f6e8362c934491675587c18fb9bbb98ed398af022a69578e`  
		Last Modified: Thu, 09 Feb 2023 09:08:07 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `aerospike:ce-6.2.0.3_1` - linux; arm64 variant v8

```console
$ docker pull aerospike@sha256:1352c4d54ba25768cb9e63110dae852d078482750ba0671fc2093a5ea05532a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75482810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d99634365fbe7739c048da7516ec6ad781c19e69a9d89c76f7ed0f3ba59f4d6`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:03:10 GMT
ARG AEROSPIKE_EDITION=community
# Thu, 09 Feb 2023 09:03:10 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
# Thu, 09 Feb 2023 09:03:10 GMT
ARG AEROSPIKE_SHA_X86_64=622b7b8d694a54ee42515bc56aa9aeb006c1f731b10df82777cbf1f154b12fff
# Thu, 09 Feb 2023 09:03:10 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz
# Thu, 09 Feb 2023 09:03:10 GMT
ARG AEROSPIKE_SHA_AARCH64=7218303567741912537b564cf50580d37b84b615aa01965ecfba20596ccfb594
# Thu, 09 Feb 2023 09:03:10 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 09 Feb 2023 09:03:27 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_aarch64.tgz AEROSPIKE_EDITION=community AEROSPIKE_SHA_AARCH64=7218303567741912537b564cf50580d37b84b615aa01965ecfba20596ccfb594 AEROSPIKE_SHA_X86_64=622b7b8d694a54ee42515bc56aa9aeb006c1f731b10df82777cbf1f154b12fff AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-community/6.2.0.3/aerospike-server-community_6.2.0.3_tools-8.1.0_debian11_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+([.][0-9]+){2,3}/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 09 Feb 2023 09:03:28 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 09 Feb 2023 09:03:28 GMT
EXPOSE 3000 3001 3002
# Thu, 09 Feb 2023 09:03:28 GMT
COPY file:d50c4b59c6030f47e41221b7d152a3e0cf299b7e8bf38ea42e3c2e33b1c9cc1f in /entrypoint.sh 
# Thu, 09 Feb 2023 09:03:28 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 09 Feb 2023 09:03:28 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a64e9ca190bc658f105e929f22af02b06045fa7823f59caf90a15f9d2227f`  
		Last Modified: Thu, 09 Feb 2023 09:04:04 GMT  
		Size: 45.4 MB (45418111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f82fd4719bbec14c501b1b8e169ba2d35ec6b6b1a82145951cbcf980896baa0`  
		Last Modified: Thu, 09 Feb 2023 09:03:59 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fbdf33e788d109a708213627a87e995f414ebd20a4f27c3be1635afe3cab9b`  
		Last Modified: Thu, 09 Feb 2023 09:03:59 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
