## `hylang:0-python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:673685d64b81d54964676f5b09b69ac9b1d88d0e2b53750df7a94cf392722b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `hylang:0-python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull hylang@sha256:9dadea0cb8418d44523e4a9442637f1b6a013c552e11b8be26799b8bcb844e90
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5882275049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceee5dbdca7e6034bdf9a457b682fd2a9c5d09869a63ef13dbc2944dcd8789f3`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 17:06:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 02 Apr 2021 20:28:51 GMT
ENV PYTHON_VERSION=3.8.9
# Fri, 02 Apr 2021 20:28:52 GMT
ENV PYTHON_RELEASE=3.8.9
# Mon, 05 Apr 2021 17:37:29 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:37:31 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 05 Apr 2021 17:37:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/29f37dbe6b3842ccd52d61816a3044173962ebeb/public/get-pip.py
# Mon, 05 Apr 2021 17:37:33 GMT
ENV PYTHON_GET_PIP_SHA256=e03eb8a33d3b441ff484c56a436ff10680479d4bd14e59268e67977ed40904de
# Mon, 05 Apr 2021 17:39:29 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:39:30 GMT
CMD ["python"]
# Mon, 05 Apr 2021 18:04:05 GMT
ENV HY_VERSION=0.20.0
# Mon, 05 Apr 2021 18:05:34 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Mon, 05 Apr 2021 18:05:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d125fe0eea998b84d015b04287600700e6c6b273702461066209a3d1b9df51d0`  
		Last Modified: Wed, 10 Mar 2021 17:27:40 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f3366e0d757da87d532f69fc81f6d105413696598e61770dcf36733b370ec`  
		Last Modified: Fri, 02 Apr 2021 20:38:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df45bd0ee984fd66cbad4a67832bd0afe7aa840e485c5427eb35c81e4f309a92`  
		Last Modified: Fri, 02 Apr 2021 20:38:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09e61dfa76ad48ea06ddf5f8d95659852b17496b75b1d4883029f13acc474b`  
		Last Modified: Mon, 05 Apr 2021 17:46:25 GMT  
		Size: 58.7 MB (58697926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8133f8b29c8f522adcf6ab3def67bb80ecb28c3e5e261a4c76acc382c14ffb82`  
		Last Modified: Mon, 05 Apr 2021 17:45:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4d409f43d1e354d105b1c072cf0159712bf42edf6aa7e479d56ba1ae6891c3`  
		Last Modified: Mon, 05 Apr 2021 17:45:13 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deed2e4e6b622924e435885e335d06056dac63318dbe296f6d141f3eebb276f5`  
		Last Modified: Mon, 05 Apr 2021 17:45:13 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8150b78560db7381792da83c7d9002eb17d1865bfe3fa363a7d2ec975d6581`  
		Last Modified: Mon, 05 Apr 2021 17:45:17 GMT  
		Size: 15.7 MB (15680728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9241063f6609fa9aa9e5e56e47221d779bf675c0cdfbd29aa525494f39e71b3e`  
		Last Modified: Mon, 05 Apr 2021 17:45:13 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c764babcf0ee715b47d4fa6f892bd8dbcfb658fad1221059cb4b34a986ad1c4d`  
		Last Modified: Mon, 05 Apr 2021 18:07:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2655aab393fb03c182897f40f45cddc06dd0ff52560a8cdbe624932ce278ac0a`  
		Last Modified: Mon, 05 Apr 2021 18:07:51 GMT  
		Size: 11.0 MB (10971792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9fb81ed7ab46c51332431e78e0d7a0c9671ee5d0248291d214fd403400bbf`  
		Last Modified: Mon, 05 Apr 2021 18:07:38 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
