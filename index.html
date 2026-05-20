<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Smart Elevator</title>

<style>
    *{
        margin:0;
        padding:0;
        box-sizing:border-box;
        font-family:'Pretendard', sans-serif;
    }

    body{
        background:#111827;
        color:white;
        display:flex;
        justify-content:center;
        align-items:center;
        height:100vh;
    }

    .app{
        width:360px;
        height:700px;
        background:#1f2937;
        border-radius:30px;
        overflow:hidden;
        position:relative;
        box-shadow:0 0 30px rgba(0,0,0,0.4);
    }

    .screen{
        width:100%;
        height:100%;
        position:absolute;
        top:0;
        left:0;
        padding:30px 25px;
        display:none;
        flex-direction:column;
        align-items:center;
    }

    .active{
        display:flex;
    }

    h1{
        margin-top:30px;
        margin-bottom:20px;
        font-size:28px;
    }

    .status-box{
        width:100%;
        background:#374151;
        padding:20px;
        border-radius:20px;
        text-align:center;
        margin-top:20px;
    }

    .floor-text{
        font-size:50px;
        font-weight:bold;
        margin-top:10px;
        color:#60a5fa;
    }

    select{
        width:100%;
        padding:15px;
        margin-top:30px;
        border:none;
        border-radius:15px;
        font-size:18px;
    }

    button{
        width:100%;
        padding:16px;
        margin-top:25px;
        border:none;
        border-radius:15px;
        background:#3b82f6;
        color:white;
        font-size:18px;
        cursor:pointer;
        transition:0.3s;
    }

    button:hover{
        background:#2563eb;
    }

    .elevator-container{
        width:120px;
        height:420px;
        background:#374151;
        border-radius:20px;
        margin-top:30px;
        position:relative;
        overflow:hidden;
    }

    .elevator{
        width:80px;
        height:80px;
        background:#60a5fa;
        position:absolute;
        left:20px;
        bottom:0;
        border-radius:15px;
        transition:all linear;
        display:flex;
        justify-content:center;
        align-items:center;
        font-size:24px;
        font-weight:bold;
    }

    .time-text{
        margin-top:30px;
        font-size:24px;
    }

    .arrival-animation{
        margin-top:80px;
        width:150px;
        height:150px;
        border-radius:50%;
        background:#22c55e;
        display:flex;
        justify-content:center;
        align-items:center;
        font-size:70px;
        animation:pulse 1s infinite;
    }

    @keyframes pulse{
        0%{
            transform:scale(1);
        }
        50%{
            transform:scale(1.1);
        }
        100%{
            transform:scale(1);
        }
    }

    .arrival-text{
        margin-top:40px;
        font-size:28px;
        font-weight:bold;
    }

    .sub-text{
        margin-top:15px;
        color:#d1d5db;
    }

</style>
</head>

<body>

<div class="app">

    <!-- 화면 1 -->
    <div class="screen active" id="screen1">

        <h1>Smart Elevator</h1>

        <div class="status-box">
            현재 엘리베이터 위치
            <div class="floor-text">
                <span id="currentFloor">1</span>층
            </div>
        </div>

        <select id="userFloor">
            <option value="">층 선택</option>
        </select>

        <button onclick="callElevator()">엘리베이터 호출</button>

    </div>

    <!-- 화면 2 -->
    <div class="screen" id="screen2">

        <h1>엘리베이터 이동 중</h1>

        <div class="elevator-container">
            <div class="elevator" id="elevator">
                ↑
            </div>
        </div>

        <div class="time-text">
            예상 도착 시간 :
            <span id="arrivalTime"></span>초
        </div>

    </div>

    <!-- 화면 3 -->
    <div class="screen" id="screen3">

        <div class="arrival-animation">
            ✓
        </div>

        <div class="arrival-text">
            엘리베이터 도착!
        </div>

        <div class="sub-text">
            탑승해주세요.
        </div>

        <button onclick="goHome()">
            확인
        </button>

    </div>

</div>

<script>

    // 층 선택 옵션 생성
    const select = document.getElementById("userFloor");

    for(let i = 1; i <= 10; i++){
        let option = document.createElement("option");
        option.value = i;
        option.textContent = i + "층";
        select.appendChild(option);
    }

    let currentFloor = 1;

    function callElevator(){

        const targetFloor = parseInt(document.getElementById("userFloor").value);

        if(!targetFloor){
            alert("층을 선택해주세요!");
            return;
        }

        // 화면 전환
        document.getElementById("screen1").classList.remove("active");
        document.getElementById("screen2").classList.add("active");

        // 거리 계산
        // 층당 높이 3m 가정
        const floorHeight = 3;

        // 엘리베이터 속도
        // 100m/min = 1.666m/s
        const speed = 100 / 60;

        const distance =
            Math.abs(targetFloor - currentFloor) * floorHeight;

        const time =
            Math.ceil(distance / speed);

        document.getElementById("arrivalTime").textContent = time;

        // 엘리베이터 애니메이션
        const elevator = document.getElementById("elevator");

        const moveHeight = (targetFloor - 1) * 34;

        elevator.style.transitionDuration = time + "s";
        elevator.style.bottom = moveHeight + "px";

        // 도착 후 화면 전환
        setTimeout(() => {

            document.getElementById("screen2").classList.remove("active");
            document.getElementById("screen3").classList.add("active");

            currentFloor = targetFloor;
            document.getElementById("currentFloor").textContent = currentFloor;

        }, time * 1000);

    }

    function goHome(){

        document.getElementById("screen3").classList.remove("active");
        document.getElementById("screen1").classList.add("active");

    }

</script>

</body>
</html>
