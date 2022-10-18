# pointerStudy

``` C
#include <stdio.h>

void a(int* ptr) {
	*ptr = 2; //인자로 받은 주소의 값을 2로 바꿈
}
int main() {
	int num = 0; //정수형 변수 선언
	int* ptr=&num; //num변수의 주소를 정수 포인터 ptr에 저장함
	printf("%d\n", *ptr); //num 변수를 출력
	a(ptr);// num변수의 주소가 담긴 포인터를 인자로 넘김
	printf("%d", *ptr); //num 변수를 출력
}
```
