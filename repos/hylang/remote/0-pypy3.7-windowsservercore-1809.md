## `hylang:0-pypy3.7-windowsservercore-1809`

```console
$ docker pull hylang@sha256:88ef1968438c6e82ae3dba8afdf98f5c2625c7f56c70d6a7be273ffd9ed1b43b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.1817; amd64

### `hylang:0-pypy3.7-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull hylang@sha256:00d77ea05d13c36e258d7e16e5379c1334705a017c392bc12bff13fbeef93c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2537862967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fec37af041bb2fa071229ba943cf73a91ad33aea1df2fc067499d63189a2411`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:09:43 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 08 Apr 2021 19:30:49 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 08 Apr 2021 19:30:51 GMT
ENV PYPY_VERSION=7.3.4
# Thu, 08 Apr 2021 19:32:26 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0ff4e4653f1ff0653f105680eb101c64c857fa8f828a54a61b02f65c94b5d262'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.4-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 08 Apr 2021 19:32:27 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 08 Apr 2021 19:32:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 08 Apr 2021 19:32:30 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 08 Apr 2021 19:34:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 08 Apr 2021 19:34:03 GMT
CMD ["pypy3"]
# Thu, 08 Apr 2021 19:56:31 GMT
ENV HY_VERSION=0.20.0
# Thu, 08 Apr 2021 19:57:31 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 08 Apr 2021 19:57:32 GMT
CMD ["hy"]
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
	-	`sha256:9aaa06ae93a71781008a718e572b4c76dd2b31ee79e2f7f1ce9863e7e5639208`  
		Last Modified: Wed, 10 Mar 2021 13:21:17 GMT  
		Size: 9.5 MB (9455936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730738027c0222e38d830ad488c2fd425e28930967e836320015535aa0f23f40`  
		Last Modified: Thu, 08 Apr 2021 19:38:37 GMT  
		Size: 19.9 MB (19913403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c315dc61e742e1386b068d38c50bbbf78f0369fd33439d8b512d16f3aad067`  
		Last Modified: Thu, 08 Apr 2021 19:38:32 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805b1d592f27ed1231542f6a58aedd95dbb56456487ccdb18c97f1c64b55dd5e`  
		Last Modified: Thu, 08 Apr 2021 19:38:42 GMT  
		Size: 31.3 MB (31338656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b00a22e4c5882681e792166b1783886d5fe8dc530cac141d3c5096f658eb6`  
		Last Modified: Thu, 08 Apr 2021 19:38:29 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4fc572a39dac1defd8c612a1f190aa75f3b177f108e86372c4df8c4d2fc264`  
		Last Modified: Thu, 08 Apr 2021 19:38:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a142c46cf47b20c64c993e999375f038bf9464238202e10b6aad8837594c37`  
		Last Modified: Thu, 08 Apr 2021 19:38:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65739693c83de616ab3c3e7114173785aa12aa77d71ad7511f56a6a5c24b198a`  
		Last Modified: Thu, 08 Apr 2021 19:38:32 GMT  
		Size: 7.3 MB (7314882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2070325a4e3659b03f506b9059aaa96b1393cc3da5679cc980e02d5d55d22b`  
		Last Modified: Thu, 08 Apr 2021 19:38:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4ff4b857abddbd4e6f21d3455db1978956af7b8c67127abde026df21b4eb3e`  
		Last Modified: Thu, 08 Apr 2021 19:58:59 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65554d2672c5b07d27b8c8edb35a2bc5ea08b37c8244326b4b69bb89e8be95d5`  
		Last Modified: Thu, 08 Apr 2021 19:59:08 GMT  
		Size: 8.3 MB (8294231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d6e8bd62d524e1bf4d9247fb59f560378e1e0b9bd77832dbaf4502e2943f9`  
		Last Modified: Thu, 08 Apr 2021 19:58:59 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
