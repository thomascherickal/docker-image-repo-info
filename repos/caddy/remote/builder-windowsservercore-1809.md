## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f51cbb2f6355b4ba86c8133c76ec964e0385fd4a3ee980a35a7e700ebf761366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
