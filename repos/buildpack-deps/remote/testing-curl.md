## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:369e8b15d042857570347d14440195c8bc1407f394c368cbc3f1eb6e04aaada4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b60f7a4239e61d1c59cde41fa7b68364299c2adb56df95d8f8387512e643bf8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70199010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f97a2c63eb6f20dbb2c777e08c1709c9852863e8c18ea806b8cdad0088622704`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:21:21 GMT
ADD file:d8f8a66e04b091b1ee6d1d330b5cd80472768f8cef96db861ba4dfaa2472fe20 in / 
# Thu, 16 Apr 2020 03:21:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:57:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:58:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d9ec154a243cb2fcf510aa97241fa4d7c075add5b018b19db3f1dca9f93c83a`  
		Last Modified: Thu, 16 Apr 2020 03:30:54 GMT  
		Size: 52.0 MB (51968339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f52bafd3e8510b30e30d2ccb5e044a4647586a4b5dcdee4e79b63b54296a77`  
		Last Modified: Thu, 16 Apr 2020 04:14:57 GMT  
		Size: 7.9 MB (7932617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61caa2b6b1a3f079feb31d0b6ce33740955163e262ec2f624070129b13ebc779`  
		Last Modified: Thu, 16 Apr 2020 04:14:58 GMT  
		Size: 10.3 MB (10298054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:30f46fa0b5f70583785fcc069f9cbee6c753f49751ee7d93fb02a320bbb04f5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68070736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfeccff5ef475aceff75d9e7ec178977bd661a1976423ff1ef31ec13e159b4b1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:41 GMT
ADD file:4315cf04b632155858b9a0c6d22c433dba5c9b23c240abe83ceeca80e94a841a in / 
# Tue, 31 Mar 2020 01:23:44 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:19:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c0806b4d4e10fd104cbda1f65b5dcee9a5b4202716f5e8367e2bff3143216eda`  
		Last Modified: Tue, 31 Mar 2020 01:32:04 GMT  
		Size: 49.9 MB (49920582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0382c643bf4a04c23f9e10efeb789cdadcdcbfd9c890261da945bbfb379473`  
		Last Modified: Tue, 31 Mar 2020 03:45:41 GMT  
		Size: 7.5 MB (7504856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d3b4a29b142be89febad4954c371a81253e3970f04a9664005d4733ece339f`  
		Last Modified: Tue, 31 Mar 2020 03:45:41 GMT  
		Size: 10.6 MB (10645298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a2be7729ce0ac6f16827bb0570d09f80afa6f39e02005909027e6e6253f9766
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64574658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89dbeb4c8a3e30f92b7011abf39b3c47b1639796275a482139e7ef8abc11d2a6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:58:05 GMT
ADD file:353f89e64e5475f2d99be1c5e0eaa80d5aeb89e02c274ba507df4def8f7ccc8a in / 
# Thu, 16 Apr 2020 00:58:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:33:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a287a7fa81e293e147ba52c36ae34e643e975ef88ebe9a6f226a048dbb7ee9fa`  
		Last Modified: Thu, 16 Apr 2020 01:08:03 GMT  
		Size: 47.6 MB (47646389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47358f6975165f42a9cd9b867f0d03e95a00b52627d5e833781a9eb45eca84cc`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 7.3 MB (7255347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376a0294fac4492ac4a3da9b92cdf02ee87e6bfd519ee19fb996c5db96da33ae`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 9.7 MB (9672922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c95b0c0060cfebb357deb8bbc453c3c89a27c72df8c65ee14e22dd9347220b53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69003377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a31d465c7351837ff159573df28586e631e6b0deddb272161852a871c0de97`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:40:12 GMT
ADD file:27c25cdd69090f4b15f9f2f4a147879d1d7510b7b2f8c231a92fc74832325413 in / 
# Thu, 16 Apr 2020 02:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c6bfde49c5261423574a9f9bc077a0cd0057775509f9d9e061556a16b84e1d7`  
		Last Modified: Thu, 16 Apr 2020 02:48:01 GMT  
		Size: 50.9 MB (50901465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c744c6854f291e264392cb87f79c4675b05d5383ca93df9f5b4be8f447aba3a7`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 7.8 MB (7807688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a53c53b80bd91c029938e07ae8fb49e75ae1d45620212fa6fc041e97f5750`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 10.3 MB (10294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:25e3c482a9fb517172c71b0f06d2d9e4d03776ed9a36f4ec84e488b66bf6897e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71883845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7fc6c6bbf2b4506b5aa012e0c821cda6ca26b8ae377fb105540ae7ac03bd472`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:50 GMT
ADD file:1d78edb74644d640409b64831c000f00654603e8888b50c46ac37ca0c186c3e9 in / 
# Thu, 16 Apr 2020 01:38:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:16:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:17:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d162d6311c3b7618a8b9a80392bb71455272c7ef63938e132282070923f16ead`  
		Last Modified: Thu, 16 Apr 2020 01:45:26 GMT  
		Size: 53.1 MB (53116500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d42814ec88fe50214d62dfdaf2c1a27abf7c61f1718b16dc664b952cc85492`  
		Last Modified: Thu, 16 Apr 2020 02:35:50 GMT  
		Size: 8.1 MB (8110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97139d647978bbac84cf0fbb6575ccf2950e262ccf617d10aa0e60e479481bb`  
		Last Modified: Thu, 16 Apr 2020 02:35:51 GMT  
		Size: 10.7 MB (10657214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:69f0c2981406d811ba0b2d0a23b20c526dd5b2233afc051e0f1ba13d95f931b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75830677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7925b49f09a4b3d6728e193fb64ee676200acb78a2af97e4c6d174cbe5c400d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:30:51 GMT
ADD file:544f960bbf6b0c556a3946247e7163ea2d8976c01f513bb4e7ed8eb8df4d09ae in / 
# Tue, 31 Mar 2020 01:30:57 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:03:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:03:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:de0d878984bf9a338e5828a66a5f63ae0852a3a1838645e030f18c29df6748ed`  
		Last Modified: Tue, 31 Mar 2020 01:42:06 GMT  
		Size: 55.8 MB (55810298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80755c7f1f2b64223e3ae4cbc62d0e4c2a93eda7f1f3734ea3686292ae264420`  
		Last Modified: Tue, 31 Mar 2020 03:58:05 GMT  
		Size: 8.3 MB (8349042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e4215faaae7e504e17484b61fdfc1a375ec0c1b46b37361c8b0c6de944883`  
		Last Modified: Tue, 31 Mar 2020 03:58:09 GMT  
		Size: 11.7 MB (11671337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ffcd45e69802bcb5f191d7d6e569cf1e583906e30a905962fb5296a400fd8edb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68352962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739b463e24e2d882023e6bd808663fa3a770c3111736bc31fb9ae4dd3249278b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:41:36 GMT
ADD file:91904e1cbd0660c7c48420aa34dd58c0e8619c69afe6c1412a495c364773b5bb in / 
# Thu, 16 Apr 2020 00:41:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:56:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:56:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:929a8c37dff5f4096f453d7847637ff8b3e3fa702bd1043408eb37af338237d4`  
		Last Modified: Thu, 16 Apr 2020 00:45:37 GMT  
		Size: 50.6 MB (50569040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625f45e55816a01b4e47db24dfb9857e953051816a723f6999906fa8fe1cb40e`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 7.6 MB (7600032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af726635ebace664ecb1c229bba4cbd77183a3411aacacaae74f1cbb0882eadb`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 10.2 MB (10183890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
