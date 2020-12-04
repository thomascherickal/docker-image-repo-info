## `hylang:windowsservercore-1809`

```console
$ docker pull hylang@sha256:2572c4e9f8d7b53599993e7d039608461575227fe172f47f39a6393934c42331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `hylang:windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull hylang@sha256:0fb7dd71b21f74106060f9026f89435d6301810e87d0dab682e1939f22c73868
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461822401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1c4b2cdc392b7f74064fadc337d27692bc428263605e8bfb0260ae3bc8b3cf`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 17:13:40 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Nov 2020 17:27:26 GMT
ENV PYTHON_VERSION=3.8.6
# Wed, 11 Nov 2020 17:27:27 GMT
ENV PYTHON_RELEASE=3.8.6
# Wed, 11 Nov 2020 17:29:11 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Thu, 03 Dec 2020 22:38:02 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Thu, 03 Dec 2020 22:38:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Thu, 03 Dec 2020 22:38:04 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Thu, 03 Dec 2020 22:38:49 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Thu, 03 Dec 2020 22:38:49 GMT
CMD ["python"]
# Thu, 03 Dec 2020 23:03:03 GMT
ENV HY_VERSION=0.19.0
# Thu, 03 Dec 2020 23:03:37 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 03 Dec 2020 23:03:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba27fafdef0dd2d90225160fe1fa0393acbcfbe112b6442bf74fa7f41916bcfb`  
		Last Modified: Wed, 11 Nov 2020 17:38:15 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74355b70644a73a63b79f5d4d79142c77fa468a234d0586abe3342b7f685ae3`  
		Last Modified: Wed, 11 Nov 2020 17:40:44 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a18d14026ff2258d76d848d251663689f79d32cff0823e015a09549f1433d1`  
		Last Modified: Wed, 11 Nov 2020 17:40:44 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c00162a4e6b8c12fe3c60be7480c95e5d2aba5b5fb413ea2aada34a74568fe`  
		Last Modified: Wed, 11 Nov 2020 17:40:54 GMT  
		Size: 57.9 MB (57922952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba612a3f7ada7931a293d4d8cd2e81cceddcb672ffe57a2df7fec892e1e5b70`  
		Last Modified: Thu, 03 Dec 2020 22:43:52 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9e2251cc238af485cdb1f6a2097a4bf81c193838e862e6bdc43c114f0cfecc`  
		Last Modified: Thu, 03 Dec 2020 22:43:52 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865fff2706b19860254d2c2c171d41a11ffa5209e157de910ebc7274f6a50639`  
		Last Modified: Thu, 03 Dec 2020 22:43:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dc2ecf92c7fab1689ebd6cff45552ea7219bda99f461975e8acd81793f5198`  
		Last Modified: Thu, 03 Dec 2020 22:43:54 GMT  
		Size: 10.3 MB (10324112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af278520f1c6a2aa427f7acadb9e32d9e7d23d702ea08e79958ed18223d9e1b9`  
		Last Modified: Thu, 03 Dec 2020 22:43:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba7da90244c897f88f62d44703879c6ff36619d9c1c9a814256fa0d349cedba`  
		Last Modified: Thu, 03 Dec 2020 23:08:26 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22072b4744eff21e00206836d081026e2b5260d9f6113ce6da1e73470c225beb`  
		Last Modified: Thu, 03 Dec 2020 23:08:28 GMT  
		Size: 5.5 MB (5534699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b57ba6434803f8548df7c8e4753ab2f5103ccd2ece334541ed3fcee09c15f6`  
		Last Modified: Thu, 03 Dec 2020 23:08:26 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
