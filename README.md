Dockerfile for Cabocha (Japanese Dependency Structure Analyzer) with UniDic

## Usage
```
$ docker run -i skozawa/cabocha-unidic cabocha
```

```
$ echo "太郎は花子が読んでいる本を次郎に渡した" | docker run -i skozawa/cabocha-unidic cabocha
    太郎は---------D
      花子が-D     |
    読んでいる-D   |
            本を---D
            次郎に-D
              渡した
EOS
```