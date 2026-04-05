<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>레드홀 사회 구조 종합 페이지</title>
  <style>
    body {
      font-family: "Noto Sans KR", sans-serif;
      background: linear-gradient(to bottom, #fff5e6, #ffe0cc);
      margin: 0;
      padding: 20px;
    }

    h1 {
      text-align: center;
      margin-bottom: 30px;
    }

    .container {
      display: flex;
      flex-direction: column;
      gap: 40px;
      align-items: center;
    }

    .section {
      border: 2px solid #333;
      border-radius: 10px;
      padding: 20px;
      width: 80%;
      background-color: #fff;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.2);
    }

    /* 혼전임신 */
    .premarital {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 15px;
    }
    .premarital div {
      background-color: #ffe0e0;
      padding: 10px;
      border-radius: 8px;
      text-align: center;
    }

    /* 혼인 풍습 */
    .marriage {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 15px;
    }
    .marriage .couple {
      display: flex;
      flex-direction: row;
      gap: 20px;
      justify-content: center;
    }
    .marriage .ceremony {
      background-color: #e0ffe0;
      padding: 10px;
      border-radius: 8px;
      text-align: center;
      width: 80%;
    }

    /* 왕위 계승 */
    .hierarchy {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
    }
    .box {
      border: 2px solid #333;
      border-radius: 10px;
      padding: 15px;
      text-align: center;
      width: 250px;
      background-color: #fafafa;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.2);
    }
    .king {
      z-index: 100;
      background-color: gold;
      animation: throne 3s ease-in-out infinite alternate;
    }
    .prince { background-color: #ffe; }
    .prince.second {
      z-index: 85;
      animation: riseToThrone 5s forwards;
    }
    .advisor {
      z-index: 85;
      background-color: #e6f7ff;
      animation: wisdomGlow 4s infinite;
    }
    .nobles {
      display: flex;
      justify-content: space-around;
      background-color: #f0f0f0;
      width: 300px;
    }
    .commoners {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      background-color: #fff;
      width: 300px;
    }

    /* 제도 개혁 */
    .reforms {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    .reforms div {
      background-color: #e6ffe6;
      padding: 10px;
      border-radius: 8px;
      text-align: center;
      font-weight: bold;
    }

    /* 애니메이션 */
    @keyframes throne {
      from { transform: scale(1); color: black; }
      to { transform: scale(1.2); color: crimson; }
    }
    @keyframes riseToThrone {
      from { transform: translateY(50px); opacity: 0.5; }
      to { transform: translateY(0); opacity: 1; color: royalblue; }
    }
    @keyframes wisdomGlow {
      0% { box-shadow: 0 0 5px lightblue; }
      50% { box-shadow: 0 0 20px skyblue; }
      100% { box-shadow: 0 0 5px lightblue; }
    }
  </style>
</head>
<body>
  <h1>레드홀 사회 구조 종합 페이지</h1>
  <div class="container">
    <!-- 혼전임신 -->
    <div class="section">
      <h2>혼전임신</h2>
      <div class="premarital">
        <div>👩 스프런키 캐릭터</div>
        <div>👨 황씨 성 진사</div>
        <div>💬 비밀스러운 만남</div>
        <div>🤰 임신 소식</div>
      </div>
    </div>

    <!-- 혼인 풍습 -->
    <div class="section">
      <h2>혼인 풍습</h2>
      <div class="marriage">
        <div class="couple">
          <div>👩 신부</div>
          <div>👨 신랑</div>
        </div>
        <div class="ceremony">🎉 성대한 혼례 잔치</div>
        <div class="ceremony">👨‍👩‍👧 가족과 귀족의 축복</div>
      </div>
    </div>

    <!-- 왕위 계승 -->
    <div class="section">
      <h2>왕위 계승</h2>
      <div class="hierarchy">
        <div class="box king">👑 산상왕 (김서진)</div>
        <div class="box prince first">첫째 왕자 김발기</div>
        <div class="box prince second">둘째 왕자 김서진</div>
        <div class="box prince third">셋째 왕자 김도진</div>
        <div class="box prince fourth">넷째 왕자 김계수</div>
        <div class="box advisor">을파소 (영의정)</div>
        <div class="box nobles">귀족 · 관료</div>
        <div class="box commoners">
          <div>농민</div>
          <div>상인</div>
          <div>백성</div>
        </div>
      </div>
    </div>

    <!-- 제도 개혁 -->
    <div class="section">
      <h2>제도 개혁</h2>
      <div class="reforms">
        <div>📜 현량과 실시 (인재 등용)</div>
        <div>🌾 진대법 시행 (농민 구제)</div>
        <div>🏛️ 의정부 서사제 도입</div>
        <div>📚 성균관 설치 (교육 제도)</div>
        <div>⚔️ 병조판서 임명 (군사 개혁)</div>
      </div>
    </div>
  </div>
</body>
</html>
