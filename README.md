## Tango With Django 따라하기

### git tag 추가
```sh
$ git tag chap04 -m 'message'
```

### git tag 리스트
```sh
$ git tag
chap04
```

### git tag 특정한 패턴 검색
```sh
$ git tag --list 'ch*'
chap04
```

### git tag 삭제
```sh
$ git tag --delete chap04
Deleted tag 'test' (was a4e16ee)
```

### git tag 상세 정보 보기
```sh
$ git show chap04
tag chap04
Tagger: tykim <goddes4@gmail.com>
Date:   Mon Aug 10 21:04:49 2015 +0900

Chapter 4

commit ed808f13b820193a9a3117411ef6e51f21ca2991
Author: tykim <goddes4@gmail.com>
Date:   Mon Aug 10 20:55:21 2015 +0900

    * Creating a Django Project
    * Creating a Django Application
    * Creating a view
    * Mapping URLs
```

### remote server 에 tag 전송
```sh
$ git push origin chap04
Username for 'https://github.com': goddes4
Password for 'https://goddes4@github.com':
Counting objects: 1, done.
Writing objects: 100% (1/1), 155 bytes | 0 bytes/s, done.
Total 1 (delta 0), reused 0 (delta 0)
To https://github.com/goddes4/tango_with_django_project.git
 * [new tag]         chap04 -> chap04
```

한번에 모든 태그 전송
```sh
$ git push origin --tags
```
