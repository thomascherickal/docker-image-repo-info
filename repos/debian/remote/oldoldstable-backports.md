## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:9304575427c32f5181eed16950f85d6e4260b34bfa6ee8f16f2df58b1ab6dc2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:2bf3569eece4adff200b7b5c4a04db91caefe6835bc7c71d7cc6cea0fd44a55d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50499356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ab00a15b108d6451b5f8d546dd1375f34f4c7068b145e7dc22afb3aab8f468`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:43 GMT
ADD file:9a5f9d2fbf4e8ff77289cde86e300dd0874dc73356d69ea45519a99f009e99dc in / 
# Wed, 01 Nov 2023 00:21:44 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:21:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d32eed0415310f14276202887b8e6edc2ea9dada5fd5f1c0584d59040bb20eec`  
		Last Modified: Wed, 01 Nov 2023 00:27:16 GMT  
		Size: 50.5 MB (50499127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6608e23ca6d71ba0644db02b975f47921f00478fa335151e11ae0e5ee3182262`  
		Last Modified: Wed, 01 Nov 2023 00:27:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:2458f72456ef1a85117966f6688dbd470cfd39fb94a72fca638a619d755c4211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e513140ded15c3bfc97b34daca60da4f68bd05f8769a73f4e66b032db947139c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:30 GMT
ADD file:16e24782831afb010e862a2ac0a2ceed2617535dff06e6cd8a091df2c0bbe452 in / 
# Tue, 21 Nov 2023 03:58:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 03:58:34 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c18d73f59fce2adf5960353a3a44ed26b5e9c631e434a3979db569ffbde89ca1`  
		Last Modified: Tue, 21 Nov 2023 04:03:41 GMT  
		Size: 46.0 MB (45966330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcab596109d56b969ccb5eb44cf0d2c6b29bf3e608d8fadb21ee147bca050a5d`  
		Last Modified: Tue, 21 Nov 2023 04:03:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7cfc6ffccdb0b1035f209ccd43df5bddddb6572ef76ab0add3e8ba7c7a149706
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6435d18ad66707d003e6c2207a40453ae0e8bcbbbb9fc1e241d05090f1f0f6fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:16 GMT
ADD file:067322df328f58025784b9686a4644e51c8f916021db33c8d3c1ca825d08a7ba in / 
# Wed, 01 Nov 2023 00:40:17 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:40:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8b24c39ded2c8ab2a51da2d9f95c90b25bc2f243c3967c3abb056d2ab71f1f8b`  
		Last Modified: Wed, 01 Nov 2023 00:44:43 GMT  
		Size: 49.3 MB (49291089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9297f107a08a0a3122e166ad996c5f258afbeb11e37e9cae95ce84dff8d4489c`  
		Last Modified: Wed, 01 Nov 2023 00:44:51 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:1baf7f4642a907081c1282ea13dbe4449e579fa0d5b04db3ce7b4ca0da25bfb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51256373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c562a5214e90164e925b9baef094d04cf8805405d34a43d990b965f681c470`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:48 GMT
ADD file:31e793a57f0790996fe5a2214acd41429941a3b362aff70d5fd504eada62085d in / 
# Tue, 21 Nov 2023 04:40:48 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:40:52 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:04418c23f29bd4990c6b8fa1256b0c7d50b97b5dac1f1b40d0856bd4ab82ba8d`  
		Last Modified: Tue, 21 Nov 2023 04:46:33 GMT  
		Size: 51.3 MB (51256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0685d979af90eb07d1103976ccd7db171aa412d6156181eb60d44c49580958`  
		Last Modified: Tue, 21 Nov 2023 04:46:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
