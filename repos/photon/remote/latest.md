## `photon:latest`

```console
$ docker pull photon@sha256:5bbad39cb8600b9c83689180a003d9a70349cfffcd57b2f687e32b19b420c722
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:314846ab67239eb3f0b94eec3990e4479bf8baf4ab6ebe60676195ba63944c83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15676523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d86b8678383af20c05e02a08709a78906dfaf41d683bf7dbe6310be9390357`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 21 Nov 2020 01:29:09 GMT
ADD file:8cbc6b2b9a26afa2ac0413f003440ded1b105bab98420f6d95af68b1eeb5b2fa in / 
# Sat, 21 Nov 2020 01:29:10 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20201120
# Sat, 21 Nov 2020 01:29:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6153de43c9393bb4fda2c85775c3be52ae61512caa94ae0c858de87ac6b5d85b`  
		Last Modified: Sat, 21 Nov 2020 01:29:52 GMT  
		Size: 15.7 MB (15676523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:0dff4395441eacabf5205a5edab7288f40a5b9984be27f6e2861b043fffc2e9f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13438888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9e70b048339fa0097df3519ca87f32145b1b0b9486cf49a5d918238d68109a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 21 Nov 2020 01:48:38 GMT
ADD file:5a7050f1ddd54177f4271c539f2accfed4c78a7127ab84a2cd8f305a9175897f in / 
# Sat, 21 Nov 2020 01:48:39 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20201120
# Sat, 21 Nov 2020 01:48:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6be304979be4f76a296c945a0ade10c1b911012edaeb69105c2734ec500d2d2c`  
		Last Modified: Sat, 21 Nov 2020 01:48:55 GMT  
		Size: 13.4 MB (13438888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
