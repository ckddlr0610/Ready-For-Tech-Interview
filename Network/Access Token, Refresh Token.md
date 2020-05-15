# Token의 정의

프로그래밍 언어에서 말하는 토큰은 문법적으로 더 이상 나눌 수 없는 기본적인 언어요소를 말한다. 최근 회원인증 방식에서 JWT 방식을 많이 사용함에 따라 Access Token과 Request Token이 많이 언급된다. 이런 토큰들은 Request 문자열 헤더에 더해져서 서버로 보내지는 역할을 한다.

# Access Token과 Refresh Token의 차이

처음 회원가입하거나 로그인을 하면 Access Token과 Refresh Token이 발급된다. 이러한 토큰들을 저장하는 방식은 다양한데, Shared Preference에 저장하기도 한다.

클라이언트에서 서버에 요청을 보낼 때, 서버는 Request에 담긴 Access Token을 검증하는 작업을 한다. 회원과 일치하는 Access Token이어야 올바른 Response를 받을 수 있다. 즉 토큰은 해당 회원임을 인증하는 데이터 중 하나인 것이다. 따라서 Token을 보안하기 위한 다양한 기술들이 있다.

Refresh Token은 Access Token의 기간이 만료됐을 때 다시 발급받기 위한 토큰이다. Access Token의 유효 기간은 비교적 짧기 때문에 기간이 긴 Refresh Token을 따로 둬서 Access Token을 갱신하게 한다.

이러한 토큰 기술은 JWT와 OAuth와 매우 연관이 있으므로 해당 기술들에 대해서도 숙지할 필요가 있다.