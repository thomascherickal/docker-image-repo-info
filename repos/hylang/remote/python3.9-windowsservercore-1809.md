## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:1e4c97d7bf330ddf0352b8a7b4f2c1efe1bd0ca280120e6af24f2828ace32036
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull hylang@sha256:370790f4becc6d1c405b1b76dacd373cc992e28b2222900225b59fd732a28bb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743420485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b389397a4acae3215eac59f5e381150f9426a6cf5917335912403aa49926af`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:23:09 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Aug 2021 17:08:02 GMT
ENV PYTHON_VERSION=3.9.6
# Wed, 11 Aug 2021 17:08:05 GMT
ENV PYTHON_RELEASE=3.9.6
# Wed, 11 Aug 2021 17:10:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Thu, 12 Aug 2021 20:18:53 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Thu, 12 Aug 2021 20:18:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Thu, 12 Aug 2021 20:18:57 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Thu, 12 Aug 2021 20:20:29 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Thu, 12 Aug 2021 20:20:32 GMT
CMD ["python"]
# Thu, 12 Aug 2021 20:42:20 GMT
ENV HY_VERSION=1.0a3
# Thu, 12 Aug 2021 20:43:32 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 12 Aug 2021 20:43:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4881292935afd838255a98d792717471c7acc2a01fcf2ad09b21e588fd8567`  
		Last Modified: Wed, 11 Aug 2021 17:18:02 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65044140da47c6921a0b456b847c51d8a0be011662132e68df409d51797c43f9`  
		Last Modified: Wed, 11 Aug 2021 17:18:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5261836ebb755d69851c52b5b5d767eba7120bc7b2322834284f00007a473f`  
		Last Modified: Wed, 11 Aug 2021 17:18:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02578ae2653aef33c68ec66e83b05ae4cf370a81f69645009b15163cf73af9e`  
		Last Modified: Wed, 11 Aug 2021 17:19:00 GMT  
		Size: 49.8 MB (49751707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ac2d669785c6b7b7dd7c9ce4450769e55529f612241d566c436e843a268bdf`  
		Last Modified: Thu, 12 Aug 2021 20:24:45 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cbf8109085cdcb9dfd0189e71bf06e6046ca7970a7c7e051a83443ebcfaa7c`  
		Last Modified: Thu, 12 Aug 2021 20:24:45 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6bd97bd68d5a6bb60e6140d96a69e8d49dde18b70a0ae099183c000d010ad4`  
		Last Modified: Thu, 12 Aug 2021 20:24:45 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ba5096b805b15ef5d02e0508f3e812c21c74ac9b7d314269792f4297e6b3a`  
		Last Modified: Thu, 12 Aug 2021 20:24:47 GMT  
		Size: 6.3 MB (6317343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb45968cc67024d1d2e62d95f0796b19f2a9771130fa9cc537eb03cda853da9`  
		Last Modified: Thu, 12 Aug 2021 20:24:45 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddfc975ce6e6624a5b610fadc848e58cea8b967b0bb27a2a3ab7246272d8cf9`  
		Last Modified: Thu, 12 Aug 2021 20:46:15 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bee894949ae44f920c930f386738cc5f9c912caccc83cfa1a17abb0194857e1`  
		Last Modified: Thu, 12 Aug 2021 20:46:16 GMT  
		Size: 1.3 MB (1339421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acbebdeae4e839b899eb961022f0247571c1e825de03ee586a97bb6847c5285`  
		Last Modified: Thu, 12 Aug 2021 20:46:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
