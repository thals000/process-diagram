# process-diagram

<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>영감→완성 프로세스 도식도</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        h1 {
            text-align: center;
            color: #2c3e50;
            margin-bottom: 40px;
            font-size: 2.5em;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }
        
        .flowchart {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }
        
        .step {
            background: linear-gradient(135deg, #84fab0 0%, #8fd3f4 100%);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.1);
            text-align: center;
            min-width: 300px;
            position: relative;
            transition: transform 0.3s ease;
        }
        
        .step:hover {
            transform: translateY(-5px);
        }
        
        .step-number {
            background: #2c3e50;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            position: absolute;
            top: -15px;
            left: 20px;
            font-weight: bold;
        }
        
        .decision {
            background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
            border-radius: 20px;
            position: relative;
        }
        
        .decision::before {
            content: '';
            position: absolute;
            top: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 0;
            border-left: 20px solid transparent;
            border-right: 20px solid transparent;
            border-bottom: 20px solid #ffecd2;
        }
        
        .branch-container {
            display: flex;
            gap: 30px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .branch {
            background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
            padding: 15px;
            border-radius: 10px;
            min-width: 200px;
            text-align: center;
        }
        
        .arrow {
            font-size: 2em;
            color: #7f8c8d;
        }
        
        .phase {
            background: linear-gradient(135deg, #d299c2 0%, #fef9d7 100%);
            margin: 20px 0;
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #8e44ad;
        }
        
        .phase-title {
            font-size: 1.5em;
            font-weight: bold;
            color: #8e44ad;
            margin-bottom: 15px;
        }
        
        .sub-steps {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .sub-step {
            background: rgba(255,255,255,0.8);
            padding: 10px 15px;
            border-radius: 8px;
            min-width: 120px;
            text-align: center;
            font-size: 0.9em;
        }
        
        .final {
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
            font-weight: bold;
            font-size: 1.1em;
        }
        
        @media (max-width: 768px) {
            .branch-container {
                flex-direction: column;
                align-items: center;
            }
            
            .sub-steps {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎨 영감→완성 프로세스 도식도</h1>
        
        <div class="flowchart">
            <!-- 1단계: 영감 떠올리기 -->
            <div class="step">
                <div class="step-number">1</div>
                <strong>영감 떠올리기</strong>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 분기점 -->
            <div class="step decision">
                <strong>영감이 떠오르는가?</strong>
            </div>
            
            <div class="branch-container">
                <div class="branch">
                    <strong>❌ 안 떠오름</strong><br>
                    • 휴식<br>
                    • 공부<br>
                    • 개인적 영감 스위치 활용
                </div>
                
                <div class="branch">
                    <strong>✅ 떠오름</strong><br>
                    다음 단계로 진행
                </div>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 2단계: 영감 타입 분류 -->
            <div class="step">
                <div class="step-number">2</div>
                <strong>영감 타입 분류</strong>
            </div>
            
            <div class="branch-container">
                <div class="branch">
                    <strong>🖼️ 이미지 영감</strong><br>
                    구체적인 그림이<br>머릿속에 떠오름
                </div>
                
                <div class="branch">
                    <strong>📚 문학적 영감</strong><br>
                    스토리, 상황, 세계관이<br>떠오름
                </div>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 3단계: 초기 작업 -->
            <div class="step">
                <div class="step-number">3</div>
                <strong>초기 작업</strong>
            </div>
            
            <div class="branch-container">
                <div class="branch">
                    <strong>이미지 영감 →</strong><br>
                    0차 러프<br>
                    (떠오른 이미지 대충 스케치)
                </div>
                
                <div class="branch">
                    <strong>문학적 영감 →</strong><br>
                    바로 세계관 설정으로
                </div>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 4단계: 기획 설계 -->
            <div class="phase">
                <div class="phase-title">4단계: 기획 설계</div>
                <div class="sub-steps">
                    <div class="sub-step">세계관 창설</div>
                    <div class="sub-step">구상 설계</div>
                    <div class="sub-step">스토리텔링 작성</div>
                    <div class="sub-step">GPT 활용 추천</div>
                </div>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 5단계: 단계별 시안 제작 -->
            <div class="phase">
                <div class="phase-title">5단계: 단계별 시안 제작</div>
                <div class="sub-steps">
                    <div class="sub-step">1차 스케치 시안<br>(여러 장)</div>
                    <div class="sub-step">2차 밸류 러프 시안<br>(명암/톤)</div>
                    <div class="sub-step">3차 컬러 러프 시안<br>(색상)</div>
                </div>
            </div>
            
            <div class="arrow">↓</div>
            
            <!-- 6단계: 최종 선택 -->
            <div class="step final">
                <div class="step-number">6</div>
                <strong>🎯 선택 및 진행</strong>
            </div>
        </div>
    </div>
</body>
</html>
