## `openjdk:18-ea-19-jdk`

```console
$ docker pull openjdk@sha256:3f0fd90c828b9dc6d3681714a58691c200c60c7b57997a1d2a7133cf968a4e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `openjdk:18-ea-19-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:5bccabacd6544321b7696daa7a8f2b8ff287d9caf605f5628decfb486746e526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243366280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de71d85248b7ec3e0778b1305fd499f826907d14fa7c68fe50640d101fbe9b2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:29:51 GMT
ADD file:3223e5829b65b376c23e1faa6f519d37b0166b38063f91b793a8ed710a39fe33 in / 
# Wed, 13 Oct 2021 18:29:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:47:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 18:47:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 13 Oct 2021 18:47:48 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:47:49 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 00:25:11 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:25:23 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:25:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:58c4eaffce77ac1fb013bf82c91927c631802ad54465ebc9b687b5dc8ee73c02`  
		Last Modified: Wed, 13 Oct 2021 18:31:20 GMT  
		Size: 42.0 MB (41961111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a22c806ee8aa2b360bd5818a4f78bc3da280abb86f3db09805b1daddd78324`  
		Last Modified: Wed, 13 Oct 2021 18:56:49 GMT  
		Size: 13.5 MB (13489427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a080d1765cf61db2d06b433ef96e1e558c0d32bc5e32f95f618d0aa0b5f17697`  
		Last Modified: Sat, 16 Oct 2021 00:32:27 GMT  
		Size: 187.9 MB (187915742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-19-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:12f00b2f3960964c31c93ae9e7e67993607894821d6d27bdfe0407a13db4f7dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (242984371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f6bf0555d9086506c4e2173e859b32ce44ec5c6be5704c030c53e6ccf43f66`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:23 GMT
ADD file:f161e88dde917cf9d761056277b85a1880719b445048fc52649306cec001db66 in / 
# Thu, 14 Oct 2021 03:43:24 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:42:19 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 14 Oct 2021 05:42:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 14 Oct 2021 05:42:21 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:42:22 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 00:05:14 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:05:26 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:05:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a1eec3e47437e3334dd709f3a36be617982ec7579fa52be305301bb95c0d4be1`  
		Last Modified: Thu, 14 Oct 2021 03:44:37 GMT  
		Size: 41.9 MB (41877085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec5552a84ea6485845e8e0a4d9b09b5e8f78d742440c18650d1ec9b1aacd89`  
		Last Modified: Thu, 14 Oct 2021 05:57:59 GMT  
		Size: 14.3 MB (14270572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b26d61ec65d120fad56d64d30ec0aece564d132b15a468d94aa9bdfde29f6f`  
		Last Modified: Sat, 16 Oct 2021 00:17:59 GMT  
		Size: 186.8 MB (186836714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-19-jdk` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:7925f9afb0c52b93d7195991aba6f6319d1da0bd1b51512a9175e4ec05d99776
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2870415308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e3508984f0d772b75157630ffcb0c3e710dcedac940aad758d5c0e69f11657`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:31:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:31:05 GMT
ENV JAVA_HOME=C:\openjdk-18
# Thu, 14 Oct 2021 00:32:09 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 16 Oct 2021 00:26:36 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:26:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_windows-x64_bin.zip
# Sat, 16 Oct 2021 00:26:38 GMT
ENV JAVA_SHA256=7774877321c01d81955febf33c0f66242f31deec7598cb5e15ce819fe376a2d1
# Sat, 16 Oct 2021 00:28:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 16 Oct 2021 00:28:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778f0ab9c363534bcf1068a50329066ca025f6499401dd667a232ffdd9687e4`  
		Last Modified: Sat, 16 Oct 2021 00:35:18 GMT  
		Size: 349.3 KB (349328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0a2b03b48b44277b5193d5197edaed6d8f3a05a714236a7f114b1a760ea024`  
		Last Modified: Sat, 16 Oct 2021 00:35:17 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd03122307cd712ddbb44adaeef533b9d027b4fd1d82e2162fe4d0dfa76012d`  
		Last Modified: Sat, 16 Oct 2021 00:35:17 GMT  
		Size: 310.9 KB (310913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89404a5acaa9266726ee8985d760dcdcd0342cd6fed174b67ff450c7f90a59e7`  
		Last Modified: Sat, 16 Oct 2021 00:35:15 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb40a0ba0179923c93a24a39aa2660d470de31ba9d6a8aadceaf7427b81eca94`  
		Last Modified: Sat, 16 Oct 2021 00:35:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d93b4d906eb34df26aef3a94ed7e08f8fe6df7a96af3def5b1b1cdf1daae04`  
		Last Modified: Sat, 16 Oct 2021 00:35:15 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d59c9399c8f15d45efa8e664be2f4ce4fa90aeafa38dd28b37ce572dda2b08`  
		Last Modified: Sat, 16 Oct 2021 00:35:34 GMT  
		Size: 183.4 MB (183427821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a117db25ba039cda232a5637e19ca9ed64155908c9ab6c369a4410e38357c96`  
		Last Modified: Sat, 16 Oct 2021 00:35:15 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-19-jdk` - windows version 10.0.14393.4704; amd64

```console
$ docker pull openjdk@sha256:1b5628e487667e06edcea305bac1689c3932e217fa15e3f2740c1bfea315d49a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6456902084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10d7bcb95be95174268518e7c892e2dae7b93aa1f72838d120983033210a0ad`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:35:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:35:33 GMT
ENV JAVA_HOME=C:\openjdk-18
# Thu, 14 Oct 2021 00:36:39 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 16 Oct 2021 00:28:34 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:28:35 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_windows-x64_bin.zip
# Sat, 16 Oct 2021 00:28:36 GMT
ENV JAVA_SHA256=7774877321c01d81955febf33c0f66242f31deec7598cb5e15ce819fe376a2d1
# Sat, 16 Oct 2021 00:30:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 16 Oct 2021 00:30:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df06f60babff5e4f22bec0a3230e7cb06b975eee8a07f9541607a63c6f54ec1`  
		Last Modified: Sat, 16 Oct 2021 00:35:57 GMT  
		Size: 352.3 KB (352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d102eb2191e4f3dc1d3161448876d7ca39ddbdf59ce99128c02345b2f37d5a7`  
		Last Modified: Sat, 16 Oct 2021 00:35:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925804b8e49990f4d1d67406a2478bccf5a1d14fc5af2bd05ff3cd31251cf4af`  
		Last Modified: Sat, 16 Oct 2021 00:35:56 GMT  
		Size: 348.2 KB (348170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c198e305448d1c9925ff9b6e51eaef4a4d891527c04e0fc22cb0b79b970abb5`  
		Last Modified: Sat, 16 Oct 2021 00:35:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81c7d891bd5eefcd54c0583e183de75c4b7b90cfa78dfa954a25b8d793ad63`  
		Last Modified: Sat, 16 Oct 2021 00:35:54 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa692a86dacab3b490f0801231f78ee3b66e625788b9a62e492309dbd3f4dbf`  
		Last Modified: Sat, 16 Oct 2021 00:35:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d305cd0a701131c1e328a1987c18ac58ea5e75d4eeb9a0650403bf4c2504b012`  
		Last Modified: Sat, 16 Oct 2021 00:39:14 GMT  
		Size: 183.4 MB (183426667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a15cd0f9ae47bf2aa559ac98a09df919b464e2e1b36869defd9d782037f3b`  
		Last Modified: Sat, 16 Oct 2021 00:35:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
