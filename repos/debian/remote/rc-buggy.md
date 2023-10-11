## `debian:rc-buggy`

```console
$ docker pull debian@sha256:ee5a7974022c3f0fa3944294d0ec9501324320712b14e1b0b091421313979bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:f7bda1fb6bd58fa2ee489e4755008f1e59ead8bba6057d526ddcae21402dcb97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49482952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b34b5d9bd870726f23fe84b40ffe4688d4b4a78cc1c0d8a7a00fe890c094a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:bc0b5b71ee53adf6297821668404ace4f79c4256461b99497849721dbd8e86ae in / 
# Wed, 20 Sep 2023 04:57:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:58:52 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d036181e87bed9eb2432498f0ccbf7baa06719a2d8360c3bc9c496bd9f853a7c`  
		Last Modified: Wed, 20 Sep 2023 05:03:10 GMT  
		Size: 49.5 MB (49482728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9543f9ff840ec709f29824e47f1779f6ce05db7ea6fe7876b9a7acb8889084f`  
		Last Modified: Wed, 20 Sep 2023 05:05:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:75699e8d50ab61022ddd61fd32709d14734d95fc3ce3463ff9282107cf91e6d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47165076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b27dff265f266a3346840b6d19f967ea010d8a1c20ea185e1a62a3509e6db5ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:39:33 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2f4ea7fe7b8690c3ca25a1b3c670c2f82209d55ff6d955af872eb0ab8df5ff97`  
		Last Modified: Wed, 11 Oct 2023 17:42:28 GMT  
		Size: 47.2 MB (47164847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03bcd2cf6d3f877a74c6bb581732051de6e3ce6932de41c83467a7c64f25ac4`  
		Last Modified: Wed, 11 Oct 2023 17:45:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:87f140bcc00661bfbe34df97fdd69c960899ca9f531cfbe767f3223ba0aa2ac5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44953808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a601f31b3ab1d33180c472b9a1059a92758d66c06c001db293f362c4e4c1f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:44:55 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b724b570b5800a7c354a5dac64a4fa673c71f6df8cbf449ab4ce5efd684dd911`  
		Last Modified: Wed, 11 Oct 2023 17:49:18 GMT  
		Size: 45.0 MB (44953579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb4828c65f8c5ea30bfc4b96993feafada91e4ee5d9e59278afb44e987e4e08`  
		Last Modified: Wed, 11 Oct 2023 17:52:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:85e2564f5b21e054c934e406e5e33d820c323496bd166c1cfecfd390f4e593fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49450716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d133d098236a20aa09484102a2808aa91e01a011f45e27fef4507a981a6324`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:16 GMT
ADD file:3493f4ad2710629ee9ad4c981682b2afcc1d9964cb5034de77189556f0c0e810 in / 
# Wed, 20 Sep 2023 02:45:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d83e3b52cf7f7a250777a05d8d2d7960fd6dba8a6438beed3879ff3c389bb01b`  
		Last Modified: Wed, 20 Sep 2023 02:50:04 GMT  
		Size: 49.5 MB (49450488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb5191978a2e1433d7d932ed3bf3fb213113be6f09dca5a12e1a588f5c6ee7a`  
		Last Modified: Wed, 20 Sep 2023 02:52:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:6b9b020ced8252fd1b97c9028977adc3888286596755da3943fe4771ad2de7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50485495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade81859d11d770f87e2d52c383a42bcb50c1fc8ac6bd1789dbaadfda8265962`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:54 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b15be2fd60b9adae282f32076fd2c71211d17ebbacfcd05f447fd925da0b81a7`  
		Last Modified: Wed, 11 Oct 2023 17:49:04 GMT  
		Size: 50.5 MB (50485267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a5e41d8c7bbadc3b4a65de5f51fb852ae00782c0039ee21107aefc3162b716`  
		Last Modified: Wed, 11 Oct 2023 17:52:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:8c68e74ffd7792f60a60c963676fb7261f89d4006f4dcacaee900b74a621ba55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49300591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777c37e818174c861a59bffaca3701a582a5525ab93913c05f5d97c66ebbfc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:58:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f19fff78c927722277ff3254b811f343062ed8e219c72e6938e3662c09994cc3`  
		Last Modified: Wed, 11 Oct 2023 18:04:05 GMT  
		Size: 49.3 MB (49300361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46554899b4196ee9e29c5345613932b3605ec7a07fb9467390aa0eb58d5b73dc`  
		Last Modified: Wed, 11 Oct 2023 18:09:44 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:e8bcce6e53dbe5a634cd6c35ee54386bdb3ee6e9d352ca7f48168b34f0139ca4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53418512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782716d7a4dc57f6a2a4e402fa7e6f0761af6350d0974241ab681c1ff372cade`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:44 GMT
ADD file:5f062baf648f8cba61d84347ebedbe11eca129a318a8146b4c7c30586cbf0436 in / 
# Wed, 11 Oct 2023 17:45:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:48:25 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ba8528ad854acf64973cba0749a6cf58ce475318878f99dccc45c01a8b19dafc`  
		Last Modified: Wed, 11 Oct 2023 17:52:11 GMT  
		Size: 53.4 MB (53418284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f3d80f10f068590a237c401237020caa56c22c6acd0758c1ee86ead2ffc15f`  
		Last Modified: Wed, 11 Oct 2023 17:55:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; riscv64

```console
$ docker pull debian@sha256:b99f818de0f3f967f5967d3bcb011460eae3250c9a138ab1c885efbcfd473096
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47864112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb27c52e5865462495f8eb5391e4000e4b77b7f85e922135e40779343c47b8d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:51 GMT
ADD file:1badbd46f7264a094446a8b1be5e0a7a86f6596b595a4fdcd4f53e886ceb37ac in / 
# Wed, 11 Oct 2023 17:38:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:40:37 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f01d648ec32af182bd1587fcd0bbef74db47d09399659d4a3c3eb94c6da4c47f`  
		Last Modified: Wed, 11 Oct 2023 17:41:43 GMT  
		Size: 47.9 MB (47863883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad41197a940e22b47ca412095c5f22d9cdf3551117b5f7fa412bc113bfe92d94`  
		Last Modified: Wed, 11 Oct 2023 17:44:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:e7a06afd77a68c23473478860f28bcebae6361ffef7320246ed441be19075520
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48923929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ad9ecec5ac3c5a1a7ac3cb59890bb83828aece0fdc47d1bbadc6bb80c91dd06`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:54:08 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1c682795de2323b695b3a151f23480c972ce25be65bcc04708dd6eb7250c65b8`  
		Last Modified: Wed, 11 Oct 2023 17:59:19 GMT  
		Size: 48.9 MB (48923705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5def1b7980e9f3dab84da444abacc8dd7ba260282fa80f2cd21a516ed2bf72e`  
		Last Modified: Wed, 11 Oct 2023 18:03:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
