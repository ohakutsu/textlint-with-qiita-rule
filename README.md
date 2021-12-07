# textlint-with-qiita-rule

:warning: This repository is not an official Qiita.

The rules for prh are in https://github.com/ohakutsu/prh-rule-qiita.

## Usage

1. Clone this repository and initialize submodule.

```bash
$ git clone https://github.com/ohakutsu/textlint-with-qiita-rule.git
$ git submodule update --init --recursive
```

2. Run sample.

```bash
$ yarn run textlint

textlint-with-qiita-rule/contents/sample.md
  1:1  ✓ error  qiita 株式会社 => Qiita株式会社  prh
  3:1  ✓ error  qiita => Qiita                   prh
  5:1  ✓ error  Qiita:Team => Qiita Team         prh
  7:1  ✓ error  Qiita Job => Qiita Jobs          prh

✖ 4 problems (4 errors, 0 warnings)
✓ 4 fixable problems.
Try to run: $ textlint --fix [file]
```

## License

MIT

See [LICENSE](/LICENSE).
