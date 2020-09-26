## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b1d92380682f9b0bad962636255fafec59f2a4e696211a1efec7112ad8a448db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
