## `dart:sdk`

```console
$ docker pull dart@sha256:42af1a47a170bb9a5f7a569eca8e65dcee7dda2db0ac19fe989e7e2c3136431a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:8852bd6dd29501a374f81818698ee98919bf5dd18f69c2b52882df903162bc2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f409d7eda3093895c419579cb8a6bc7c3038c8b4c99ac377d72287450a98e2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 10:29:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 10:29:23 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 17 Aug 2021 10:29:24 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 17 Aug 2021 10:29:24 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:29:24 GMT
WORKDIR /root
# Tue, 17 Aug 2021 10:29:36 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf70384699785586e7ce2387dcc48a39b1fa8b9837b6ec033441a3dd93ce4818`  
		Last Modified: Tue, 17 Aug 2021 10:30:35 GMT  
		Size: 49.6 MB (49581314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4c0190f1231c9d6c5fbfffaca9ee1baff80d891a3c91988c9bd7de914f9fd6`  
		Last Modified: Tue, 17 Aug 2021 10:30:21 GMT  
		Size: 2.4 MB (2359146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba67f3672479ac113591af7f34f12de75f4d398f8c687c595aa02824c30fde8`  
		Last Modified: Tue, 17 Aug 2021 10:31:00 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
