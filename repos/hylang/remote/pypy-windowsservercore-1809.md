## `hylang:pypy-windowsservercore-1809`

```console
$ docker pull hylang@sha256:38e1ae89b44cf1c82919989f6c45357cb2d2293c91839ff160b1737356187266
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `hylang:pypy-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull hylang@sha256:ce76231a6772b1d7c72b95dd147ae460a93f90e6db5f03c60de37da30778a1d7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2524132847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221080fad6668f84839673b6eb91dc44a540ade93ca070d6d37846e867d6b546`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 12:10:30 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 12:11:13 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 12:11:14 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 14 Apr 2021 12:12:20 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0ff4e4653f1ff0653f105680eb101c64c857fa8f828a54a61b02f65c94b5d262'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.4-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 12:12:21 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 14 Apr 2021 12:12:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Apr 2021 12:12:24 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Apr 2021 12:14:07 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 12:14:08 GMT
CMD ["pypy3"]
# Wed, 21 Apr 2021 12:32:06 GMT
ENV HY_VERSION=1.0a1
# Thu, 22 Apr 2021 07:32:29 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 22 Apr 2021 07:32:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f6d57ba0852b3fce341e01e03fc7d9d38056c3b9ed689b9f524af859e95e96`  
		Last Modified: Wed, 21 Apr 2021 12:05:49 GMT  
		Size: 5.1 MB (5070800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a176e14776b64754370c5ac7655befeb0136deb25470bbfbed583a54164123`  
		Last Modified: Wed, 21 Apr 2021 12:05:49 GMT  
		Size: 15.5 MB (15495438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1be0ecdd97142203f27572dbfa49f7efbea928e1db4fd80777ce981d30d1e1`  
		Last Modified: Wed, 21 Apr 2021 12:05:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246153cb1e457451e7954341ee04b6b5d99c2ef6f117df95114633bd0c4c311a`  
		Last Modified: Wed, 21 Apr 2021 12:05:57 GMT  
		Size: 26.9 MB (26944628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8af3e5570178719379f21e82972d66ab7e5dd8b1789099cf99f9909300bfb3c`  
		Last Modified: Wed, 21 Apr 2021 12:05:43 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ef34e798ec3a172b83baa7da2507400c95e9af5b9f7a91556b6d6973204d7`  
		Last Modified: Wed, 21 Apr 2021 12:05:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee26a43dd2e25ea8d566bd48d5b4ebc065fc988125e1891b13f3737ba9de3c2`  
		Last Modified: Wed, 21 Apr 2021 12:05:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc12a004c03f45e8e9aef1538d9c875cfce64f5e5e5d644c154c5b97efc76e7`  
		Last Modified: Wed, 21 Apr 2021 12:05:46 GMT  
		Size: 2.9 MB (2907943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd82eef8f80fff889d6ae18687fb13f5d1fbd60c7c98b0066048cd885165104b`  
		Last Modified: Wed, 21 Apr 2021 12:05:43 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e695f6328c69b7169d27c41cd0d96fa31bdbc5a7cd16f25b23ab62e46e9d90dd`  
		Last Modified: Thu, 22 Apr 2021 07:33:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877e475df0905c37c45159bbaa0210f7ea05ba5e541fc2fa6f1360123e936f92`  
		Last Modified: Thu, 22 Apr 2021 07:33:21 GMT  
		Size: 3.9 MB (3948771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de23befab97b0f729bca10f94283451749f1e4fe1392770db543cd78b2e44451`  
		Last Modified: Thu, 22 Apr 2021 07:33:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
