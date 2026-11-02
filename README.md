# flash.bbang

번쩍 만들고 빵 터지는 웹 게임 모음. 인스타그램·유튜브 프로필 링크용 페이지.

- 주소: https://flash-bbang.github.io/
- 게임: [칼퇴 박대리](https://flash-bbang.github.io/kaltoe-park/), [빵 스도쿠](https://flash-bbang.github.io/bbang-sudoku/), [딩! 동물원](https://flash-bbang.github.io/ding-zoo/), [빵빵 블록](https://flash-bbang.github.io/bbang-block/), [SPACE XXX](https://flash-bbang.github.io/space-xxx/)
- 순서: 각 게임이 시작할 때 Firestore `plays` 컬렉션에 한 줄씩 남기고, 이 페이지가 게임별 개수를 세서 많이 한 순으로 정렬합니다 (연결이 안 되면 최신순).

새 게임을 추가할 때는 `index.html`의 `#games` 안에 카드(`<a class="card" data-game="…">…</a>`)를 하나 복사해서 맨 위에 넣고,
게임 쪽 `logPlay()`의 game 값과 Firestore 규칙의 game 목록에도 같은 이름을 추가하고,
썸네일(600×750 jpg)을 같이 올리면 됩니다.
