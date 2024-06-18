
---

1. 소요시간 : 
2. 문제 사이트 : 
3. 문제 수준 : 
4. 문제 유형 : 
5. 다른 사람의 풀이를 참고 했는가 ? :
6. 문제 링크 : https://www.acmicpc.net/problem/2857

---

### 1. 사용한 자료구조 & 알고리즘
X


### 2. 소스코드
```java
import java.io.*;
import java.util.*;
// command shift f

public class Main {

    static Integer arr[];
    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StringBuilder sb = new StringBuilder();
        
        Queue<Integer> queue = new LinkedList<>();
        for(int i=0;i<5;i++) {
            String word = br.readLine();
            if(word.contains("FBI")) queue.add(i+1);
        }
        
        if(queue.isEmpty()) {
            System.out.println("HE GOT AWAY!");
        } else {
            while(!queue.isEmpty()) {
                System.out.print(queue.poll()+" ");
            }
        }
    }
}
```
### 3. 결과

<img width="1235" alt="Capture" src="https://github.com/KimNahun/algorithm-1day1solve/assets/118811606/df6bc3c8-d8e0-46d2-a818-bd13923248bb">

