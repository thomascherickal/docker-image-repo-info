## `aerospike:ee-6.4.0.2`

```console
$ docker pull aerospike@sha256:2f1646466d811f139c6eeed06aa8a3b07721eed7ce80f7c7607e64af942e2a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `aerospike:ee-6.4.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:0556d606610aeee55bb6ba26c1fba54c4f93ed7a6e211d240077b8743950ecc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83105471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb1adb2551a7c5fbf2d29e8f9e4548d1b2518e7ddd994b36fbf8791f3647750`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:51 GMT
ADD file:3a8cd4de7f163d93718670f4db1de49045f5e04af3a8aa27d81c0f14647db707 in / 
# Thu, 07 Sep 2023 00:20:51 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:46:02 GMT
ARG AEROSPIKE_EDITION=enterprise
# Thu, 07 Sep 2023 02:46:02 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_x86_64.tgz
# Thu, 07 Sep 2023 02:46:02 GMT
ARG AEROSPIKE_SHA_X86_64=b63face987a0c7c0392d59a2744d11b72846805cca2db73f0db22a03a979105c
# Thu, 07 Sep 2023 02:46:02 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_aarch64.tgz
# Thu, 07 Sep 2023 02:46:02 GMT
ARG AEROSPIKE_SHA_AARCH64=0b3fd109e0e80a1e345ee3f63cb97612fd5bf5786fd55d77fd43ac3b11b6038d
# Thu, 07 Sep 2023 02:46:02 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 07 Sep 2023 02:46:22 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_aarch64.tgz AEROSPIKE_EDITION=enterprise AEROSPIKE_SHA_AARCH64=0b3fd109e0e80a1e345ee3f63cb97612fd5bf5786fd55d77fd43ac3b11b6038d AEROSPIKE_SHA_X86_64=b63face987a0c7c0392d59a2744d11b72846805cca2db73f0db22a03a979105c AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+[.][0-9]+[.][0-9]+([.][0-9]+)+(-rc[0-9]+)*/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 07 Sep 2023 02:46:23 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 07 Sep 2023 02:46:23 GMT
EXPOSE 3000 3001 3002
# Thu, 07 Sep 2023 02:46:23 GMT
COPY file:57ed4c0390f91371a6d5ddbdf0ecf475b40dc8871b369f3100b157df0d753fc5 in /entrypoint.sh 
# Thu, 07 Sep 2023 02:46:23 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 07 Sep 2023 02:46:23 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:360eba32fa65016e0d558c6af176db31a202e9a6071666f9b629cb8ba6ccedf0`  
		Last Modified: Thu, 07 Sep 2023 00:25:22 GMT  
		Size: 29.1 MB (29124494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9bd0116a14e3f782a7e6cf352fe004f74cf762fdb6c2445370999f6cc5b80`  
		Last Modified: Thu, 07 Sep 2023 02:47:03 GMT  
		Size: 54.0 MB (53978787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f7b3c65eadb5f5dc1a23d44765f68515735863f9bfcd383c3332f863c6e63`  
		Last Modified: Thu, 07 Sep 2023 02:46:56 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b1c24d2a5677386ce35ff843e381fd6f45bdba91f522cb45c297dbfbc73d71`  
		Last Modified: Thu, 07 Sep 2023 02:46:56 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `aerospike:ee-6.4.0.2` - linux; arm64 variant v8

```console
$ docker pull aerospike@sha256:44a827c41c0f7b738b2bf502dedb1f84515026164d8c7830cf0c98b4bf5a8ada
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82359630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89650872bf98a1276adc411db405f92d555bc0d6a9014466f588f2700640f5fa`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-Eeuo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:39 GMT
ADD file:fb5c8f411c4a1e06c25ac32455221938386907d0b4782fc228ca67de63a7e9de in / 
# Thu, 07 Sep 2023 00:39:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:23:59 GMT
ARG AEROSPIKE_EDITION=enterprise
# Thu, 07 Sep 2023 09:23:59 GMT
ARG AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_x86_64.tgz
# Thu, 07 Sep 2023 09:23:59 GMT
ARG AEROSPIKE_SHA_X86_64=b63face987a0c7c0392d59a2744d11b72846805cca2db73f0db22a03a979105c
# Thu, 07 Sep 2023 09:23:59 GMT
ARG AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_aarch64.tgz
# Thu, 07 Sep 2023 09:23:59 GMT
ARG AEROSPIKE_SHA_AARCH64=0b3fd109e0e80a1e345ee3f63cb97612fd5bf5786fd55d77fd43ac3b11b6038d
# Thu, 07 Sep 2023 09:23:59 GMT
SHELL [/bin/bash -Eeuo pipefail -c]
# Thu, 07 Sep 2023 09:24:17 GMT
# ARGS: AEROSPIKE_AARCH64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_aarch64.tgz AEROSPIKE_EDITION=enterprise AEROSPIKE_SHA_AARCH64=0b3fd109e0e80a1e345ee3f63cb97612fd5bf5786fd55d77fd43ac3b11b6038d AEROSPIKE_SHA_X86_64=b63face987a0c7c0392d59a2744d11b72846805cca2db73f0db22a03a979105c AEROSPIKE_X86_64_LINK=https://artifacts.aerospike.com/aerospike-server-enterprise/6.4.0.2/aerospike-server-enterprise_6.4.0.2_tools-9.0.0_debian12_x86_64.tgz
RUN {     export DEBIAN_FRONTEND=noninteractive;     apt-get update -y;     apt-get install -y --no-install-recommends apt-utils;     apt-get install -y --no-install-recommends       binutils       ca-certificates       curl       xz-utils;   };   {     apt-get install -y --no-install-recommends procps;   };   {     VERSION="$(grep -oE "/[0-9]+[.][0-9]+[.][0-9]+([.][0-9]+)+(-rc[0-9]+)*/" <<<"${AEROSPIKE_X86_64_LINK}" | tr -d '/')";   };   {     ARCH="$(dpkg --print-architecture)";     if [ "${ARCH}" = "amd64" ]; then       sha256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940;       suffix="";     elif [ "${ARCH}" = "arm64" ]; then       sha256=1c398e5283af2f33888b7d8ac5b01ac89f777ea27c85d25866a40d1e64d0341b;       suffix="-arm64";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     curl -fsSL "https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static${suffix}" --output /usr/bin/as-tini-static;     echo "${sha256} /usr/bin/as-tini-static" | sha256sum -c -;     chmod +x /usr/bin/as-tini-static;   };   {     ARCH="$(dpkg --print-architecture)";     mkdir -p aerospike/pkg;     if [ "${ARCH}" = "amd64" ]; then       pkg_link="${AEROSPIKE_X86_64_LINK}";       sha256="${AEROSPIKE_SHA_X86_64}";     elif [ "${ARCH}" = "arm64" ]; then       pkg_link="${AEROSPIKE_AARCH64_LINK}";       sha256="${AEROSPIKE_SHA_AARCH64}";     else       echo "Unsuported architecture - ${ARCH}" >&2;       exit 1;     fi;     if ! curl -fsSL "${pkg_link}" --output aerospike-server.tgz; then       echo "Could not fetch pkg - ${pkg_link}" >&2;       exit 1;     fi;     echo "${sha256} aerospike-server.tgz" | sha256sum -c -;     tar xzf aerospike-server.tgz --strip-components=1 -C aerospike;     rm aerospike-server.tgz;     mkdir -p /var/{log,run}/aerospike;     mkdir -p /licenses;     cp aerospike/LICENSE /licenses;   };   {     if [ "${AEROSPIKE_EDITION}" = "enterprise" ]; then       apt-get install -y --no-install-recommends         libcurl4         libldap-2.4.2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.0" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         libcurl4;     fi;     dpkg -i aerospike/aerospike-server-*.deb;     rm -rf /opt/aerospike/bin;   };   {     if ! [ "$(printf "%s\n%s" "${VERSION}" "5.1" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python2;     elif ! [ "$(printf "%s\n%s" "${VERSION}" "6.2.0.3" | sort -V | head -1)" != "${VERSION}" ]; then       apt-get install -y --no-install-recommends         python3         python3-distutils;     fi;   };   {     pushd aerospike/pkg || exit 1;     ar -x ../aerospike-tools*.deb;     popd || exit 1;     tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/;   };   {     find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +;     mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike;     if ! [ "$(printf "%s\n%s" "${VERSION}" "6.2" | sort -V | head -1)" != "${VERSION}" ]; then        mv aerospike/pkg/opt/aerospike/bin/aql /usr/bin;     fi;     if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     else       mkdir /usr/lib/asadm;       mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f 'aerospike/pkg/opt/aerospike/bin/asinfo' ]; then       mv aerospike/pkg/opt/aerospike/bin/asinfo /usr/lib/asadm/;     fi;     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;   };   {     rm -rf aerospike;   };   {     rm -rf /var/lib/apt/lists/*;     dpkg --purge       apt-utils       binutils       ca-certificates       curl       xz-utils 2>&1;     apt-get purge -y;     apt-get autoremove -y;     unset DEBIAN_FRONTEND;   };   echo "done";
# Thu, 07 Sep 2023 09:24:18 GMT
COPY file:c76954551192450f2d9e2a428b0b3a3daeba46fccf29d07ceabb675e275a068e in /etc/aerospike/aerospike.template.conf 
# Thu, 07 Sep 2023 09:24:18 GMT
EXPOSE 3000 3001 3002
# Thu, 07 Sep 2023 09:24:18 GMT
COPY file:57ed4c0390f91371a6d5ddbdf0ecf475b40dc8871b369f3100b157df0d753fc5 in /entrypoint.sh 
# Thu, 07 Sep 2023 09:24:18 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 07 Sep 2023 09:24:18 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:155eab17d86c47443adc8cebe7fc62c847c03db8cfb1ca53aa6276564fff23ef`  
		Last Modified: Thu, 07 Sep 2023 00:43:02 GMT  
		Size: 29.2 MB (29157149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba941babcc7c14b435ed29f5f0d8138eeedadbbf82c8a10236cd692f312d9bb`  
		Last Modified: Thu, 07 Sep 2023 09:24:54 GMT  
		Size: 53.2 MB (53200294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89bc9cb1a7d5c479b27d03264f99624704024be451fe6415a90a2bed7def0f0`  
		Last Modified: Thu, 07 Sep 2023 09:24:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebe3b6f193a2265ea0ce8ad6b3927c777c83da163021cb665332af4d80252ed`  
		Last Modified: Thu, 07 Sep 2023 09:24:47 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
