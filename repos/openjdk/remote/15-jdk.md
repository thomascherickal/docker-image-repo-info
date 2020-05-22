## `openjdk:15-jdk`

```console
$ docker pull openjdk@sha256:e42fc42e760e6ed9cfe6634b310fe9ea2f1ffecacdd7849c0fd612ba284c0446
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `openjdk:15-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:dcaff114f61368b32c4f067885fecc3fc3227fde485b192ba60edf43c62b150d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250273342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624da38a493435711378241fc0d6285d6c7b9b0b802ea9182e09e132295fd467`
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
# Fri, 22 May 2020 01:21:26 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-aarch64_bin.tar.gz; 			downloadSha256=c9817b2efa619dcde0d4a5fa9dd1d6bcbe5bdf05fee152e9a06387544c4e5c90; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz; 			downloadSha256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:21:26 GMT
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
	-	`sha256:acbbf40cf391760f79c8a138e8234829abedd40c54c6b8a19b093df3772bd66b`  
		Last Modified: Fri, 22 May 2020 01:26:10 GMT  
		Size: 192.1 MB (192059783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:18c45ac3be3c05fecb60d21db75dc6ee4c26109c6cdaad6361a3e72aa1934790
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233217482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686360b5f07f25f56af65608260068bb82b3ee1233962f448d8080a9bc558775`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:42:34 GMT
ADD file:b059ded860ba734fbe035c768d5c7e01a82decd7db5ca12f093672dab3b204c3 in / 
# Mon, 04 May 2020 20:42:37 GMT
CMD ["/bin/bash"]
# Fri, 22 May 2020 01:43:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 22 May 2020 01:43:48 GMT
ENV LANG=en_US.UTF-8
# Fri, 22 May 2020 01:43:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 22 May 2020 01:43:49 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 May 2020 01:43:50 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 22 May 2020 01:45:15 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-aarch64_bin.tar.gz; 			downloadSha256=c9817b2efa619dcde0d4a5fa9dd1d6bcbe5bdf05fee152e9a06387544c4e5c90; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz; 			downloadSha256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:45:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fa5299bfe4aa00db1c3f39321cc679889e30f51f690a75b8c75163698c4c7831`  
		Last Modified: Mon, 04 May 2020 20:43:38 GMT  
		Size: 44.1 MB (44074523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342df9bce1d80b8bdf565c6ceb8cbb008ee180f7fd52e3006d84ae4f81d0dc67`  
		Last Modified: Fri, 22 May 2020 01:48:19 GMT  
		Size: 15.0 MB (15028449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fd8200fdfff9aca28885f3b5af2627050e0f3091bc7693d31f40d0457128b`  
		Last Modified: Fri, 22 May 2020 01:48:40 GMT  
		Size: 174.1 MB (174114510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:9d35cc673e5f43891be01c3157a5d1462dcb73bbf043678d9b1dbefb911418b8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1906934522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfca9649b8bee214366583045e40186a57c0ef4c0f90cf09e16011a68a56828`
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
# Fri, 15 May 2020 21:43:51 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 21:43:52 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_windows-x64_bin.zip
# Fri, 15 May 2020 21:43:53 GMT
ENV JAVA_SHA256=7aa6628d9d600e726b0a43856cf7f91531ecfbf44a2b41ec1a4d6ec195c56c3e
# Fri, 15 May 2020 21:45:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 May 2020 21:45:37 GMT
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
	-	`sha256:790682a22530592e3c56aff84d609b6625ac2534b1e82f5965cde7d115a4a983`  
		Last Modified: Fri, 15 May 2020 21:54:23 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5449149f21a6eb8761199314e01d9e89f92fc1e363fefff91c05db3376d873ab`  
		Last Modified: Fri, 15 May 2020 21:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c4224754f056120c1e2d1dc5ec935429010a9fc5036973cc7b67e5fe771440`  
		Last Modified: Fri, 15 May 2020 21:54:23 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c2646400a0fadd3fcadec870e74df36ae08893f8da326c1eb4f3cca5e2d86`  
		Last Modified: Fri, 15 May 2020 21:57:31 GMT  
		Size: 187.9 MB (187947445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f555cb88248a102f55c5c24a8452b0e0dbff80ee10290f6d19b501f76b531d`  
		Last Modified: Fri, 15 May 2020 21:54:23 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:3a2874cc8b75eefbfd55ce0812a7077c9c9c3e61e5567fab7962ce6419cea488
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5940113836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d23b080e4d74c09442033de0a5bc537d4bdecda13d04ae98c96873697a87d68`
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
# Fri, 15 May 2020 21:45:48 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 21:45:49 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_windows-x64_bin.zip
# Fri, 15 May 2020 21:45:50 GMT
ENV JAVA_SHA256=7aa6628d9d600e726b0a43856cf7f91531ecfbf44a2b41ec1a4d6ec195c56c3e
# Fri, 15 May 2020 21:48:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 May 2020 21:48:39 GMT
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
	-	`sha256:f56693bac87cda17ffb96f818829cd62028123ed21793be98b7979ca85c6fbdc`  
		Last Modified: Fri, 15 May 2020 21:57:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8e70aa7dca6fe470c1160d9a3b3be0e735606514461cc403a5bf6e2feeb05`  
		Last Modified: Fri, 15 May 2020 21:57:52 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe8b1dd780f966b91878ae915243911a74b45f75a0ec5a4ad83f2e23b42229`  
		Last Modified: Fri, 15 May 2020 21:57:52 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88070dc0881e928eef624441e75a9c9b7b7a3652c20aebed46d39a7513feb9e`  
		Last Modified: Fri, 15 May 2020 22:01:18 GMT  
		Size: 197.5 MB (197471845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d884c21aed13c82e0262994d83ba50caef0d436fe28af32ab9a4f0150f12ad0`  
		Last Modified: Fri, 15 May 2020 21:57:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
