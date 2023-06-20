## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:365af5a3b9aafef2a3643b86fdfd9aff48e23ca15f2fcbbc50758f1d1fead5c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:35403a0fb34661054cbfbb38950cff2953ff94c21cdb30ad23917d562024a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72610451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5c0e5a6bad08194e453141d56d08f60663f7b82f8414ea2ea0658ccf7a2f36`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 20 Jun 2023 22:23:30 GMT
ADD file:c282c432beddccdfddad38f09edfd4fd5192f5be2e30bc597cf9a5583291cc4a in / 
# Tue, 20 Jun 2023 22:23:31 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 20 Jun 2023 22:23:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:281f6a765baecfa4d7d44a194acf50d6c143541e688119d438a7d69fb8c53746`  
		Last Modified: Tue, 20 Jun 2023 22:23:48 GMT  
		Size: 72.6 MB (72610237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6685aec18e6f34c941b9701db9f8ba92320cf3b7ce40bf53de2224c21235de28`  
		Last Modified: Tue, 20 Jun 2023 22:23:40 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
