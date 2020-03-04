<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cirros`

-	[`cirros:0`](#cirros0)
-	[`cirros:0.5`](#cirros05)
-	[`cirros:0.5.0`](#cirros050)
-	[`cirros:latest`](#cirroslatest)

## `cirros:0`

```console
$ docker pull cirros@sha256:5e8fbc0173baecef5422f68527fb17a452b9361d875b344c627702b6de3c3a86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0` - linux; amd64

```console
$ docker pull cirros@sha256:96137d51e0e46006243fa2403723eb47f67818802d1175b5cde7eaa7f19446bd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4898135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc94bceaae77cc5249dc61d35a1c4c34de0a8af4783f72db1bbc9c07b262a997`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Mon, 07 Jan 2019 00:20:54 GMT
ADD file:5ec7b4c2fd8d0568d91d14345e9b66a717b83ca0d414aa72e88194f4e77456ea in / 
# Mon, 07 Jan 2019 00:20:55 GMT
RUN rm /etc/rc3.d/S40-network
# Mon, 07 Jan 2019 00:20:55 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Mon, 07 Jan 2019 00:20:55 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3d6427f49fe318fc8062066677acb50b2f755b716313f238de517f2b751f15b9`  
		Last Modified: Wed, 25 Jul 2018 18:20:09 GMT  
		Size: 4.9 MB (4896732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1915bfe8159b9eb0715555abf9ede26623b18d26db30bcaa56e5fcf8027037e7`  
		Last Modified: Mon, 07 Jan 2019 00:21:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ec9ef25b96bd430d3303c343865d4e65878a4b6167b50d4b79d27889557b06`  
		Last Modified: Mon, 07 Jan 2019 00:21:11 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm variant v5

```console
$ docker pull cirros@sha256:2c6772feefb5d44d01953fe16460967c4730f968616ddb35b8f52d9aab35357e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4551937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee428d894fd5ad44942074cf24ab1cfb9ffca6185ea3346153308f4751320e2`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 26 Feb 2020 00:44:54 GMT
ADD file:ef4ef283d7113c6bd4458b79d179995f485350f4d6e04a045f9d912fb897ad5a in / 
# Wed, 26 Feb 2020 00:44:57 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 26 Feb 2020 00:45:01 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 26 Feb 2020 00:45:02 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:ff85acfc2885a10f7435d3bf891800c0cb81fa92df6711637075ae6be180604c`  
		Last Modified: Wed, 26 Feb 2020 00:45:27 GMT  
		Size: 4.6 MB (4550528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8db706b362e87b778db226eb3d0b8c4f76e65c0d523faf66aaa26f6b224924`  
		Last Modified: Wed, 26 Feb 2020 00:45:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4d52e8c7bf17eb410e4fdf3de38346d556f408cec995574978b4f7866f86a`  
		Last Modified: Wed, 26 Feb 2020 00:45:26 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:810d5176ef12243043d309695c14269b63dbb1e07441263a410d99757b81a2fa
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8180883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0446752835a8cf5217534d23ccee4ae9f1e01c9549e54f69a96a9ba4fcdb84`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 26 Jul 2018 08:40:23 GMT
ADD file:fd61ae7812080b0d055ec1da6c4c3a9058c717baa40bfe0f2edab650ca50aa42 in / 
# Thu, 26 Jul 2018 08:40:26 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 26 Jul 2018 08:40:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 26 Jul 2018 08:40:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:a2cb5895ad559485b06ffc60454417d3e9585b90189d83cd322a609924c9b89f`  
		Last Modified: Thu, 26 Jul 2018 08:41:06 GMT  
		Size: 8.2 MB (8179477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc52f8c05de83650b63a3b9bcfbee00096e55efa093d53a6fe4fe1f303789c7a`  
		Last Modified: Thu, 26 Jul 2018 08:41:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e7e8d0b83455a2612f469373be735045e4795ec3917aab2189588edc3e73ca`  
		Last Modified: Thu, 26 Jul 2018 08:41:03 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; 386

```console
$ docker pull cirros@sha256:6cee7eabbe9bf34e73fde4a6d8b955c808f430599a259591d1ab795048bc3fa8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4531093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5d9fa097c8440fd2cfb8843a8dd8d9a972b555e123ecd6171d56a631f487835`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 10 Oct 2018 10:41:12 GMT
ADD file:3509494e259d2bd55cf88a9b3d124726566ccfbe9f09d1c406aa4b8cb30a80fa in / 
# Wed, 10 Oct 2018 10:41:13 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 10 Oct 2018 10:41:14 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 10 Oct 2018 10:41:14 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:4a52327b10d42ee792828c05768f292d8a259f648b6683dab18cee5ae4807c9c`  
		Last Modified: Thu, 26 Jul 2018 10:40:00 GMT  
		Size: 4.5 MB (4529691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a60ea55f4f1f0334e550b0642eb7738350bb3b83bf3ca78378c00888ec98ac`  
		Last Modified: Wed, 10 Oct 2018 10:41:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13cb801b6fa540134678091d7e09572b9fe3e7059ffe025db71819f351e3f2d`  
		Last Modified: Wed, 10 Oct 2018 10:41:25 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; ppc64le

```console
$ docker pull cirros@sha256:23bb04ad34dde0a9482d78a8eee177b468e842ea35b4f048ed9af2f864ca16ce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8631315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3779987c4e3a6a820a3c99fecf2110fbb55cf138a207150ef8a9db81a690ab1a`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 26 Jul 2018 08:16:54 GMT
ADD file:48673b15a50b1958dd9d689bbc5af6187c49cfceb67e67399dd55f23721a89dc in / 
# Thu, 26 Jul 2018 08:17:03 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 26 Jul 2018 08:17:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 26 Jul 2018 08:17:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:b9cc78c330c94db6b434c47d8c31d390d5d7907ff6f5cd248b069e300984a8f1`  
		Last Modified: Thu, 26 Jul 2018 08:17:30 GMT  
		Size: 8.6 MB (8629904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c78701b15f15302094237753457e5c6c733baee7a8a4e121a3fe8ebda53f6c7`  
		Last Modified: Thu, 26 Jul 2018 08:17:28 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f94b09c7b21d4ad038fc4ec2b52592b52aa3ffee20139b1a4c1a92a8b2ecf3b`  
		Last Modified: Thu, 26 Jul 2018 08:17:30 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.5`

**does not exist** (yet?)

## `cirros:0.5.0`

**does not exist** (yet?)

## `cirros:latest`

```console
$ docker pull cirros@sha256:5e8fbc0173baecef5422f68527fb17a452b9361d875b344c627702b6de3c3a86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:latest` - linux; amd64

```console
$ docker pull cirros@sha256:96137d51e0e46006243fa2403723eb47f67818802d1175b5cde7eaa7f19446bd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4898135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc94bceaae77cc5249dc61d35a1c4c34de0a8af4783f72db1bbc9c07b262a997`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Mon, 07 Jan 2019 00:20:54 GMT
ADD file:5ec7b4c2fd8d0568d91d14345e9b66a717b83ca0d414aa72e88194f4e77456ea in / 
# Mon, 07 Jan 2019 00:20:55 GMT
RUN rm /etc/rc3.d/S40-network
# Mon, 07 Jan 2019 00:20:55 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Mon, 07 Jan 2019 00:20:55 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3d6427f49fe318fc8062066677acb50b2f755b716313f238de517f2b751f15b9`  
		Last Modified: Wed, 25 Jul 2018 18:20:09 GMT  
		Size: 4.9 MB (4896732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1915bfe8159b9eb0715555abf9ede26623b18d26db30bcaa56e5fcf8027037e7`  
		Last Modified: Mon, 07 Jan 2019 00:21:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ec9ef25b96bd430d3303c343865d4e65878a4b6167b50d4b79d27889557b06`  
		Last Modified: Mon, 07 Jan 2019 00:21:11 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm variant v5

```console
$ docker pull cirros@sha256:2c6772feefb5d44d01953fe16460967c4730f968616ddb35b8f52d9aab35357e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4551937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee428d894fd5ad44942074cf24ab1cfb9ffca6185ea3346153308f4751320e2`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 26 Feb 2020 00:44:54 GMT
ADD file:ef4ef283d7113c6bd4458b79d179995f485350f4d6e04a045f9d912fb897ad5a in / 
# Wed, 26 Feb 2020 00:44:57 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 26 Feb 2020 00:45:01 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 26 Feb 2020 00:45:02 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:ff85acfc2885a10f7435d3bf891800c0cb81fa92df6711637075ae6be180604c`  
		Last Modified: Wed, 26 Feb 2020 00:45:27 GMT  
		Size: 4.6 MB (4550528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8db706b362e87b778db226eb3d0b8c4f76e65c0d523faf66aaa26f6b224924`  
		Last Modified: Wed, 26 Feb 2020 00:45:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4d52e8c7bf17eb410e4fdf3de38346d556f408cec995574978b4f7866f86a`  
		Last Modified: Wed, 26 Feb 2020 00:45:26 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:810d5176ef12243043d309695c14269b63dbb1e07441263a410d99757b81a2fa
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8180883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0446752835a8cf5217534d23ccee4ae9f1e01c9549e54f69a96a9ba4fcdb84`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 26 Jul 2018 08:40:23 GMT
ADD file:fd61ae7812080b0d055ec1da6c4c3a9058c717baa40bfe0f2edab650ca50aa42 in / 
# Thu, 26 Jul 2018 08:40:26 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 26 Jul 2018 08:40:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 26 Jul 2018 08:40:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:a2cb5895ad559485b06ffc60454417d3e9585b90189d83cd322a609924c9b89f`  
		Last Modified: Thu, 26 Jul 2018 08:41:06 GMT  
		Size: 8.2 MB (8179477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc52f8c05de83650b63a3b9bcfbee00096e55efa093d53a6fe4fe1f303789c7a`  
		Last Modified: Thu, 26 Jul 2018 08:41:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e7e8d0b83455a2612f469373be735045e4795ec3917aab2189588edc3e73ca`  
		Last Modified: Thu, 26 Jul 2018 08:41:03 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; 386

```console
$ docker pull cirros@sha256:6cee7eabbe9bf34e73fde4a6d8b955c808f430599a259591d1ab795048bc3fa8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4531093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5d9fa097c8440fd2cfb8843a8dd8d9a972b555e123ecd6171d56a631f487835`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 10 Oct 2018 10:41:12 GMT
ADD file:3509494e259d2bd55cf88a9b3d124726566ccfbe9f09d1c406aa4b8cb30a80fa in / 
# Wed, 10 Oct 2018 10:41:13 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 10 Oct 2018 10:41:14 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 10 Oct 2018 10:41:14 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:4a52327b10d42ee792828c05768f292d8a259f648b6683dab18cee5ae4807c9c`  
		Last Modified: Thu, 26 Jul 2018 10:40:00 GMT  
		Size: 4.5 MB (4529691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a60ea55f4f1f0334e550b0642eb7738350bb3b83bf3ca78378c00888ec98ac`  
		Last Modified: Wed, 10 Oct 2018 10:41:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13cb801b6fa540134678091d7e09572b9fe3e7059ffe025db71819f351e3f2d`  
		Last Modified: Wed, 10 Oct 2018 10:41:25 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; ppc64le

```console
$ docker pull cirros@sha256:23bb04ad34dde0a9482d78a8eee177b468e842ea35b4f048ed9af2f864ca16ce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8631315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3779987c4e3a6a820a3c99fecf2110fbb55cf138a207150ef8a9db81a690ab1a`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 26 Jul 2018 08:16:54 GMT
ADD file:48673b15a50b1958dd9d689bbc5af6187c49cfceb67e67399dd55f23721a89dc in / 
# Thu, 26 Jul 2018 08:17:03 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 26 Jul 2018 08:17:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 26 Jul 2018 08:17:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:b9cc78c330c94db6b434c47d8c31d390d5d7907ff6f5cd248b069e300984a8f1`  
		Last Modified: Thu, 26 Jul 2018 08:17:30 GMT  
		Size: 8.6 MB (8629904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c78701b15f15302094237753457e5c6c733baee7a8a4e121a3fe8ebda53f6c7`  
		Last Modified: Thu, 26 Jul 2018 08:17:28 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f94b09c7b21d4ad038fc4ec2b52592b52aa3ffee20139b1a4c1a92a8b2ecf3b`  
		Last Modified: Thu, 26 Jul 2018 08:17:30 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
