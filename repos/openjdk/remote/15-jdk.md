## `openjdk:15-jdk`

```console
$ docker pull openjdk@sha256:efeb15a8ef482a77de70e46f9f90a562ca3a3566306773109fd81d8737e721b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `openjdk:15-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:4d3f25f148cfeb1ecc547a71979310de88df0da5adc2c4bb046f048f0619af81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250273134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf5eaf27e749665bcf478dd16bba9ddd019c25111efa5ca1490b80c16857d36`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:20:53 GMT
ADD file:d23891d2372d6aae3d738388c74dacd92f9406083ee0c1ac0e2bfd140f92ec2b in / 
# Mon, 04 May 2020 20:20:53 GMT
CMD ["/bin/bash"]
# Mon, 04 May 2020 20:38:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Mon, 04 May 2020 20:38:21 GMT
ENV LANG=en_US.UTF-8
# Mon, 04 May 2020 20:38:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Mon, 04 May 2020 20:38:21 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:58:26 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 20:58:27 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz
# Fri, 15 May 2020 20:58:27 GMT
ENV JAVA_SHA256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0
# Fri, 15 May 2020 20:59:08 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 15 May 2020 20:59:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:83755823a002357171a0b229ef5769a60db47a90b624adc45f8c6b7cd1d1394f`  
		Last Modified: Mon, 04 May 2020 20:22:07 GMT  
		Size: 43.5 MB (43455265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e105caaf23acf967db67aa1f683d428603dbb51e12295bfe8f5df6a4cce8bb`  
		Last Modified: Mon, 04 May 2020 20:40:58 GMT  
		Size: 14.8 MB (14758294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7d7b55b8f2efac94bd12a0cc4194666cee137aa0424fc4cab7ad4b3d2ddfc`  
		Last Modified: Fri, 15 May 2020 21:06:39 GMT  
		Size: 192.1 MB (192059575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:818d467b37bce53b84a1a3639648891ea30c7f497b7d0f74f80e795f6aaf5429
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1906862573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3adbbcd2c233f765bcb6ccf4029ce2099cb8efd21f1c3b3780cbba7cffb1ef`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:22:51 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 13 May 2020 15:22:52 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 13 May 2020 15:23:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:23:15 GMT
ENV JAVA_VERSION=15-ea+22
# Wed, 13 May 2020 15:23:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/22/GPL/openjdk-15-ea+22_windows-x64_bin.zip
# Wed, 13 May 2020 15:23:17 GMT
ENV JAVA_SHA256=df01fe6b5cfa1ec43cd3754d1e76723ab1c6041283b369d2b4e5b7182e9fbaec
# Wed, 13 May 2020 15:25:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 May 2020 15:25:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc1950cbc28db7632bd0afe94e7afdd5ca08b3a3ca57687e6a837312b287f7a`  
		Last Modified: Wed, 13 May 2020 16:04:15 GMT  
		Size: 347.0 KB (346988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccd9bd22f75be58d6e2a85f96e44ed57e761dd5917328d2ab7a827a81241f7e`  
		Last Modified: Wed, 13 May 2020 16:04:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fd42a12a95b96ecfd3687faac5e7c17ace93c556f6920de761fb801902ada`  
		Last Modified: Wed, 13 May 2020 16:04:15 GMT  
		Size: 300.4 KB (300354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257430049cb1b55cdd1c186b876a44d5f80ed13f71094a3854637c8b626e027`  
		Last Modified: Wed, 13 May 2020 16:04:11 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60d36d74cfba7dcf7d7ccd1287c24de64ed84859f5fdd78bef1e37071c825e`  
		Last Modified: Wed, 13 May 2020 16:04:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3e98ca227d47f4581082f0c9a85aea871865a42e52c5167675183fed62356`  
		Last Modified: Wed, 13 May 2020 16:04:12 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55a03f6c052d4b46ef236c4e62d06db24867df36110968bc0e237084de804f`  
		Last Modified: Wed, 13 May 2020 16:07:58 GMT  
		Size: 187.9 MB (187875538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f498e8b9036d00d29d63150c5d17f77e3370fbd513cbe5b725411b141d9ef8`  
		Last Modified: Wed, 13 May 2020 16:04:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:284091cf98ecb6550e75bbcb7affe367539b11a1c70f3b380750872418511082
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5935577342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ce31933c658e779a411a49ee3e3052f489a63c6a9276aab47ff3c7221c1d4e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:26:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 13 May 2020 15:26:35 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 13 May 2020 15:27:52 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:27:53 GMT
ENV JAVA_VERSION=15-ea+22
# Wed, 13 May 2020 15:27:55 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/22/GPL/openjdk-15-ea+22_windows-x64_bin.zip
# Wed, 13 May 2020 15:27:56 GMT
ENV JAVA_SHA256=df01fe6b5cfa1ec43cd3754d1e76723ab1c6041283b369d2b4e5b7182e9fbaec
# Wed, 13 May 2020 15:30:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 May 2020 15:30:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56eaed4a20d0f67d3d00bc23ac486a70424c1d5ebc2b77f4b3bf17c8fcf765d`  
		Last Modified: Wed, 13 May 2020 16:08:25 GMT  
		Size: 5.4 MB (5382606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19edd7328d1003d3b7eb7cc52937a9ad37740aeddce56a7db9cf0cbff77e015`  
		Last Modified: Wed, 13 May 2020 16:08:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78316c2a5c012f8c77766fd738f4887044ffc57b19cc57ce29a90b94edbef075`  
		Last Modified: Wed, 13 May 2020 16:08:28 GMT  
		Size: 5.4 MB (5362683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff149b3fd37bc7ecba20e60f14d305c8c7029d8d187811dfcb848c483ea9a18c`  
		Last Modified: Wed, 13 May 2020 16:08:20 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f0678f4644695ecf00ceda4d2a23af3a7052468ce9dc03c7d3edc595204ab2`  
		Last Modified: Wed, 13 May 2020 16:08:20 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83f9d42e0994aa695b44278604ee754e0b73a7771fc0e4cc07d69bebf38c86f`  
		Last Modified: Wed, 13 May 2020 16:08:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eed92105c56b0e1e5b0eefc73b0728666de60ad4a6d3bdef9652fc9c103411`  
		Last Modified: Wed, 13 May 2020 16:08:50 GMT  
		Size: 192.9 MB (192935322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55357229ced5d702e156f68e879aa73fbbce0ade04a95708362afd68c343d9a7`  
		Last Modified: Wed, 13 May 2020 16:08:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
