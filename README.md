# libgo-http

## conv/header

��HTTP Header��JSON�`���Ȃǂɕϊ����܂��B

jq�̂悤�ȃR�}���h�Ƒg�ݍ��킹��΁A�V�F���ŗ��p�\�ɂȂ�܂��B

### �g�p���@

#### �v���O�����Ăяo����

�v���O�����ŗ��p����ꍇ��conv/header.go���g�p���܂��B

```golang
import (
	"github.com/ngv-jp/libgo-http/conv"
)
�i�����j
	c := conv.NewHttpHeaderConverter()
	r, e := c.Output()
```

#### �R�}���h���s��

�R�}���h�Ŏ��s����ꍇ��conv/main/header.go���g�p���܂��B
�p�C�v�Ōq����΁A�W���o�͂���̓f�[�^�ɂ��邱�Ƃ��\�ł��B

```bash
curl -I https://example.com | go run conv/main/header.go
```

�f�t�H���g�ł�JSON�`���ŏo�͂���܂��B

```json
{"acceptRanges":"bytes","age":"197337","cacheControl":"max-age=604800","code":"200","contentEncoding":"gzip","contentLength":"648","contentType":"text/html; charset=UTF-8","date":"Thu, 07 Jul 2022 14:50:20 GMT","etag":"\"3147526947\"","expires":"Thu, 14 Jul 2022 14:50:20 GMT","lastModified":"Thu, 17 Oct 2019 07:18:26 GMT","server":"ECS (sec/973B)","xCache":"HIT"}
```
