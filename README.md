# 코딩 테스트 스터디

> 기존에 자바로 풀이한 문제는 [링크](https://github.com/Jwhyee/coding-test-study)에서 확인할 수 있습니다.

## 참여자

<center>

<table style="margin: 0 auto" align='center'>
    <th>
        <a href="https://github.com/Jwhyee">가준영</a>
    </th>
    <th>
        <a href="https://github.com/ealswjd">이민정</a>
    </th>
    <th>
        <a href="https://github.com/hyunjeong222">정현정</a>
    </th>
    <tr>
        <td><img src="https://avatars.githubusercontent.com/u/82663161?v=4" width="200" height="200"/></td>
        <td><img src="https://avatars.githubusercontent.com/u/79951187?v=4" width="200" height="200"/></td>
        <td><img src="https://avatars.githubusercontent.com/u/57525431?v=4" width="200" height="200"/></td>
    </tr>
</table>

</center>

## 진행 방식

1. 모든 인원이 일요일까지 한 문제를 선정해 디스코드 **문제-업로드** 채널에 업로드합니다.
    - 문제를 업로드할 때, 알고리즘 종류에 대해 언급하지 않습니다.
    - 방장이 `n주차 문제 업로드`라는 채팅을 올리면 해당 채팅 쓰레드에 문제를 올려주시면 됩니다!
2. 주어진 문제를 발표일 전까지 풀이를 완료합니다.
3. 한 문제당 모든 인원이 발표를 진행합니다.
    - 본인의 코드를 `디버깅` 혹은 `출력`을 통해 **최대한 자세하게 설명**합니다.
    - 문제 발표 순서는 **사다리 타기**로 정합니다.
4. 한 문제에 대한 발표가 끝나면 메모리와 시간을 비교합니다.
    - 어느 부분에서 메모리와 시간 차이가 나는지 비교하며 공부합니다.
        - 프로그래머스는 제출 과정에서 뜨는 마지막 테스트를 기준으로 비교합니다.
    - 비교가 끝나면 **3번 과정**으로 돌아가 다음 문제 발표를 진행합니다.

## 주의사항

- 가능한 **모든 라인에 주석을 작성**해주세요.
    - 주석은 코드 위쪽을 기준으로 작성해주세요.
    ```java
    // 방향 조절 : 아래 -> 오른쪽 -> 좌측 상단 대각선 순서
    int[] dy = {1, 0, -1};
    int[] dx = {0, 1, -1};
    ```
- 앞서 발표한 사람과 코드가 동일하더라도 발표는 진행합니다.
    - 코드를 읽고 설명할 수 있는 능력을 키우기 위함
- 풀이하지 못한 문제는 **본인이 할 수 있는 부분까지만 코드를 작성** 후 이해되지 않는 부분에 대해 질문합니다.
- 한 문제에 대해 모두가 발표하기 때문에 **인당 발표 횟수는 참여자 수와 동일**합니다.

## 풀이 업로드 방식

- `Javadoc`을 이용해 클래스단에 문제 이름(난이도), 시간, 메모리, 링크를 기입해주세요.

```java
/**
 * 문제 이름(난이도) : 두 수의 합(LV0)
 * 시간 : 0.02ms
 * 메모리: 77MB
 * 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/120802
 * */
public class BOJ_3197_1 {
    public static int solution(int a, int b){
        return a + b;
    }
    public static void main(String[] args) {
        System.out.println(solution(1, 2) == 3);
    }
}
```

- 백준의 경우 제출 페이지에서 시간 및 메모리를 확인 가능
- 프로그래머스의 경우 `제출 후 채점하기`를 눌러서 나오는 가장 마지막 테스트 케이스의 내용을 입력
    - 정확성, 효율성 2개가 존재할 경우 `효율성`에 대한 내용으로 기입합니다.
- 코드 작성이 완료되면, `commit & push`를 진행해주세요.

```bash
git add .

# 백준일 경우 브(BRO), 실(SIL), 골(GOL) 앞 3글자만 작성
git commit -m "[BOJ][BRO] - 단어 길이 재기"
# 프로그래머스일 경우 문제 레벨 작성
git commit -m "[PRG][LV2] - 두 수의 합"

git push origin master
```