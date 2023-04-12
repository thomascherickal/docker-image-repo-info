## `openjdk:21-ea-jdk`

```console
$ docker pull openjdk@sha256:4404bc22f248a26878056906e761242d70f8b69447b73f9590ef002143a615e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1607; amd64
	-	windows version 10.0.17763.4131; amd64

### `openjdk:21-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:ee558e6c9310a4bada83ba090c34300b35dbfe40f14a53cba8d4b12b140f9c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260995026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd166ee26c8afd6831641b7f3abdeb257c97434b796ecbba26e0922891f808a`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:37:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:37:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 06 Apr 2023 18:37:15 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Apr 2023 18:37:16 GMT
ENV LANG=C.UTF-8
# Tue, 11 Apr 2023 23:32:45 GMT
ENV JAVA_VERSION=21-ea+17
# Tue, 11 Apr 2023 23:32:55 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='98dcda513be6f72005f9b52c79d88f7e6bef066baddf0b89d9847c125b6d9bed'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='795231d9254753b31583afabc08fb092c00cc2459962cfdd3e0b0bd32edcad92'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 11 Apr 2023 23:32:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55560f49b1cd4515e5c12b0a190ca11492533ca3757e761c254daf809031bdc5`  
		Last Modified: Thu, 06 Apr 2023 18:38:00 GMT  
		Size: 15.0 MB (15002954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec0c3aae91733fa54f9afeefb57e2f204f68f572ecd21b62715e11ac49b5d28`  
		Last Modified: Tue, 11 Apr 2023 23:34:56 GMT  
		Size: 201.4 MB (201428170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6f9583a748877782857db2ebcf564a0dada768a9b99a97c5fdca0d134f359816
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259114411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dccdcdfd0b35482c2ede84f2ec0555a13e0d45cf1172cf9cba03204396005c0c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:59:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:59:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 06 Apr 2023 18:59:01 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Apr 2023 18:59:01 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 00:00:34 GMT
ENV JAVA_VERSION=21-ea+17
# Wed, 12 Apr 2023 00:00:44 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='98dcda513be6f72005f9b52c79d88f7e6bef066baddf0b89d9847c125b6d9bed'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='795231d9254753b31583afabc08fb092c00cc2459962cfdd3e0b0bd32edcad92'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 Apr 2023 00:00:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57603b9946d65e0ac1577d90598fe906f0885a24be64058c4412b3d03b03a59a`  
		Last Modified: Thu, 06 Apr 2023 18:59:42 GMT  
		Size: 15.8 MB (15844620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b03716ffb4a5a037c7c4b893517089800999c5cf8ce5506df527266452c663a`  
		Last Modified: Wed, 12 Apr 2023 00:02:36 GMT  
		Size: 199.8 MB (199792743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - windows version 10.0.20348.1607; amd64

```console
$ docker pull openjdk@sha256:c7e96e9ee3bf9dbb13dd8db49a4edc48cde407e2bd396c48a5b35c70142caa73
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1911884387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377dd6a50a0b6a0579b917e68e6241784fef4c2900f666847945a07fb5cb1218`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:14:25 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Mar 2023 04:14:26 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Mar 2023 04:14:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 03 Apr 2023 21:16:18 GMT
ENV JAVA_VERSION=21-ea+16
# Mon, 03 Apr 2023 21:16:19 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/16/GPL/openjdk-21-ea+16_windows-x64_bin.zip
# Mon, 03 Apr 2023 21:16:20 GMT
ENV JAVA_SHA256=f7dbf4427d5b0cba84358a0009a657a29410e38cdea7a550d0fa8e3d0e16bd78
# Mon, 03 Apr 2023 21:17:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 03 Apr 2023 21:17:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9232261c30bc22ec57212f386e8fea077a0775299f58234bfec01a611d98144`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 736.0 KB (736009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545d4a9e39b1cc7dac0d42fb0a331c120f1bfed624e7850e1faa4eb99110ce01`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8063d1ae112267a681a9e7feb4d398e107825072b3fd2b95b3bad2efc8571978`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 538.0 KB (538004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013cc4d9ebbacd4a590509221c4cb191a9b07c3445606687a2d83063a224bb7`  
		Last Modified: Mon, 03 Apr 2023 21:22:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f12507315f93d8f556407b3d3f5a7dee7c3a788cee1a7a6dbed32a72aaa8415`  
		Last Modified: Mon, 03 Apr 2023 21:22:14 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03eb0cb1da1acc3d9b865826335d0e674d6dca239df0544857f024f99b78d418`  
		Last Modified: Mon, 03 Apr 2023 21:22:14 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ad6294d39f64b5d01b1518bdca3d53abbda78a379da9de947c090d239f994`  
		Last Modified: Mon, 03 Apr 2023 21:22:38 GMT  
		Size: 196.7 MB (196661756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945c98b4599510160ccdb425021e2804c41ebe7ccf72db3a26696fb393fefbcd`  
		Last Modified: Mon, 03 Apr 2023 21:22:14 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - windows version 10.0.17763.4131; amd64

```console
$ docker pull openjdk@sha256:0d6a20fde8a2e8869910097ee17e9ca098e31ef6dfda1b0cb7f18a99670989b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2210754020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f55bcc66a2d17c3cc7e3986f2638f0c6feaac07b1b4ef0d93433fff5863dae`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:17:49 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Mar 2023 04:17:50 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Mar 2023 04:19:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 03 Apr 2023 21:17:47 GMT
ENV JAVA_VERSION=21-ea+16
# Mon, 03 Apr 2023 21:17:49 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/16/GPL/openjdk-21-ea+16_windows-x64_bin.zip
# Mon, 03 Apr 2023 21:17:50 GMT
ENV JAVA_SHA256=f7dbf4427d5b0cba84358a0009a657a29410e38cdea7a550d0fa8e3d0e16bd78
# Mon, 03 Apr 2023 21:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 03 Apr 2023 21:20:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6954ad7da48d4dd7acf8132bc41996dfcd7f157b30b2ca35ec4814ffc26a94d3`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 480.4 KB (480436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087e24b23846aed99e303ff6d5268f444daecd74c150fb70198dabc16487141`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2836db1b10d5ae1b6c026b5fc8f9667c86fafa8854926472e99f786aea1aaf7f`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 309.7 KB (309740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9712c2107c485e271962572d79ab534ac9e78857494015b66c64872fe31fb9`  
		Last Modified: Mon, 03 Apr 2023 21:22:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036570a531adc10a2f649ed0903789a8e594cf1d1206e9d42154f79a38908d4c`  
		Last Modified: Mon, 03 Apr 2023 21:22:58 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d6f07aa63d36f66bb58bb895c6bc0f7c7dda7c58a3d4b99b62b234f846be3`  
		Last Modified: Mon, 03 Apr 2023 21:22:58 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97c20a4ce38387b343781e268db1271586402bbefc65153b62230649587109`  
		Last Modified: Mon, 03 Apr 2023 21:23:22 GMT  
		Size: 196.4 MB (196446363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e87fcdf9d6a589c9b6d2911dc217a9904f9ce4b919589c4422dfac124b257e`  
		Last Modified: Mon, 03 Apr 2023 21:22:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
