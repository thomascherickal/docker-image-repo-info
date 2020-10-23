## `openjdk:16-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:14a32aa9de295372e32a2c6f29aaac47236b800cfe0070d83d45c21780a27906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `openjdk:16-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull openjdk@sha256:823b97c0f0eb2524f3937156cf739e8928d1ff57d4c09a5e24e52392166e9043
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2582888345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fb2a001798c3ef2903ad33fcfa40a9c94106e90fa4f8f12715530daecca09c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 17:38:17 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 14 Oct 2020 17:38:18 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 14 Oct 2020 17:38:40 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 22 Oct 2020 23:15:20 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 23:15:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_windows-x64_bin.zip
# Thu, 22 Oct 2020 23:15:21 GMT
ENV JAVA_SHA256=8373e5ff39d7d577be70b3b8bc9e649cb600d16c87d36c528e21c9afe0965476
# Thu, 22 Oct 2020 23:17:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 22 Oct 2020 23:17:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5f8e5825cfa7b4f8c5a50657da7a44c0547d90306b4fa11bbf82021b684262`  
		Last Modified: Wed, 14 Oct 2020 18:26:50 GMT  
		Size: 9.2 MB (9230486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e034563561e5379df3a00fd4da250e977243aacd8623dc768db3ef40497b87`  
		Last Modified: Wed, 14 Oct 2020 18:26:42 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24997a5d1f99495d60fc79a47ec6d7bcf172f637b322078eccbc230cebf01c74`  
		Last Modified: Wed, 14 Oct 2020 18:26:42 GMT  
		Size: 307.8 KB (307821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f5339e209809df36cee7e558645af9c6d4f46809e734ca23aa5dc4ff83002a`  
		Last Modified: Thu, 22 Oct 2020 23:33:36 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d61a2e25590163bcb0ab2d730e845df993e8ce6e9993c3c48226b7762cc840`  
		Last Modified: Thu, 22 Oct 2020 23:33:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93ee129c078aa469a7440b18f777e1ba1e220007edbe1188d840d787d7e22a`  
		Last Modified: Thu, 22 Oct 2020 23:33:36 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713929eb4aa0fa2de28ffc4e0297c58ec291640838de5600e2e39c089ef2a182`  
		Last Modified: Thu, 22 Oct 2020 23:33:56 GMT  
		Size: 199.3 MB (199253057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbc1171830f0fee69432c404addd634b7646bb369553c4c325d2e2ac8e25223`  
		Last Modified: Thu, 22 Oct 2020 23:33:37 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
