## `dart:beta`

```console
$ docker pull dart@sha256:809ebfb70b742054e3c1b531c2422b2ca3ff6d2a3ddbbd1ca07b0bdb9c4ba95d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:20f47939ff623398ca76ec9716f9663dd615fe726af538b49a7bd4040af7f537
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.0 MB (289001985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67c3ee874ac9d8f7d1be12258da06da9151edf80d6a494469d5328f76389c424`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 03:33:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 03:33:21 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Fri, 03 Sep 2021 03:33:21 GMT
ENV DART_SDK=/usr/lib/dart
# Fri, 03 Sep 2021 03:33:21 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 03:33:21 GMT
WORKDIR /root
# Fri, 03 Sep 2021 03:33:55 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.14.0-377.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "73ed9204792cd5c4a06ccffc98884c201ca23876a8fd01db133a7e7b5b28a0ac *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7e1abeaae14b916e75f56944ce7bcfe42a03875edb1bf4377b00df41aae202`  
		Last Modified: Fri, 03 Sep 2021 03:34:26 GMT  
		Size: 49.6 MB (49583194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ba2d113bca583e95fd1ffd40466d29c60c848eb97cae88f7c707a78e107c3a`  
		Last Modified: Fri, 03 Sep 2021 03:34:17 GMT  
		Size: 2.4 MB (2359138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cada0585635a95d5b25598f18b09da198070dd7ad8fe3ad1448104962c64d6a6`  
		Last Modified: Fri, 03 Sep 2021 03:36:03 GMT  
		Size: 209.9 MB (209913809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
