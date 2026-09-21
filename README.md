# test9

// [Dart] 숫자 값을 증가/리셋하는 간단한 카운터 클래스 모델

class Counter {
  int _value = 0; // 카운트 값을 저장하는 프라이빗 변수 (0 초기화)

  // 현재 카운트 값을 읽을 수 있는 getter
  int get value => _value;

  // 카운트 값을 1 증가시키는 메서드
  void increment() {
    _value++;
    print("현재 카운트: $_value");
  }

  // 카운트 값을 0으로 리셋하는 메서드
  void reset() {
    _value = 0;
    print("카운터가 리셋되었습니다.");
  }
}

void main() {
  Counter myCounter = Counter(); // Counter 객체 생성

  myCounter.increment(); // 카운트 1 증가 (출력: 1)
  myCounter.increment(); // 카운트 1 증가 (출력: 2)
  myCounter.reset();     // 카운트 리셋 (출력: 0)
}
