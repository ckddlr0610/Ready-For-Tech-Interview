# Intent Flag

## Intent Flag란?

프로그램을 실행하다보면 여러개의 엑티비티가 쌓이게 되는데, 이 엑티비티들을 관리하는 것이 Task다. Task는 Stack 자료구조의 형태를 가지고 있다. 예를 들면 내가 A화면에서 B화면으로 이동했을 때, B에서 뒤로 가기를 하면, pop이 발생하고, 밑에 있던 A 화면이 다시 나타나는 형태다. 이 Task를 관리하는 것이 Intent Flag다.

## 사용방법

### AndroidManifest에서

<activity android:launchMode = "//attribute">

매니페스트 파일에서 엑티비티 런치모드 속성값을 줌으로써 intent flag를 적용할 수 있다.

- standard : 디폴트 속성이며, 엑티비티에 대한 제약 없이 한 엑티비티가 여러개 생성될 수도 있다.
- singleTop : 만약 top엑티비티가 A인데, 또 A를 호출한다면 기존에 top에 있던 엑티비티가 다시 생성된다. 즉, 이전 화면이 같은 화면이라면 인스턴스가 재생성되는 일을 막는 것이다.
- singleTask : RootActivity로만 존재하며 하나의 인스턴스만 생성 가능하다. 다른 엑티비티 실행 시, 동일 Task내에서 실행이 가능하다.
- singleInstance : RootActivity로만 존재하며 하나의 인스턴스만 생성 가능하다. 다른 엑티비티를 실행하면 새로운 Task가 생성되서 그 Task에 포함된다.

### 코드로 명시

Intent.addFlag() 혹은 Intent.setFlag()를 사용한다.