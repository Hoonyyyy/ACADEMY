# 점포등록
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Full Screen Div</title>
<link rel="stylesheet" href="./css/storeregisterCSS.css">
<script src="./js/jquery-3.6.4.js"></script>

</head>
<body>

    
    <div id="container">
        <div id="header">

            <div id="headerLeft">
                <div class="banner"><a class="mainReturn" href="./main.html">
                    <span>S</span>
                    <span>ᴇ</span>
                    <span>ᴏ</span>
                    <span>ɴ</span>
                    <span>ɢ</span>
                    <span>s</span>
                    <span>ᴜ</span>
                    <span>ᴍ</span>
                    <span>ᴀ</span>
                    <span class="scale-down">ɴ</span>
                    </a>
                </div>
                <div class="searchBox">

                    <input class="searchInput"type="text" name="" placeholder="Search">

                    <button class="searchButton" href="#">
                        <i class="material-icons">
                            검색
                        </i>
                    </button>

                </div>
        
            </div>
            <div id="headerRight">
                <div>
                    <div id="고객마당">고객마당
                        <div class="dropdown">
                            <a href="#">⦁ 자유게시판</a>
                            <a href="#">⦁  폐업신고</a>
                        </div>
                    </div>
                    <div id="점포등록"><a href="#">점포등록</a></div>
                    <div id="로그인"><a href="./login.html">로그인</a></div>
                </div>
            </div>
            
        </div>
    </div>









	<!-- 점포등록하기 -->
	
	<div id="main">
		<h1>점포 등록 하기</h1>
		<hr>

		<div id="registerMain">
			<div id="registerInner">

				<div class="name">
					<h2>상호명</h2>
					<textarea class="textarea" 
								placeholder="상호명을 입력해주세요." width="300px"></textarea>
				</div>

				<div class="name">
					<h2>가게 간단한 설명</h2>
					<textarea class="textarea"
							placeholder="메인에 보여 가게의 간단한 설명을 해주세요 ex)성수에서 커피로 제일 맛있는집"></textarea>
				</div>

				<div class="open">
					<h2>대표 사진 (*3개 사진 필수 입력)</h2>
					<input type="file" id="inputImage">
					  <div class="image-container"></div>
					  
				</div>

				<div class="location">
					<h2>지역</h2>
					<form action="action.jsp" class="location2">
						<input type="radio" name="location" value="1ga1dong" checked >성수 1가 1동
						<input type="radio" name="location" value="1ga2dong">성수1가 2동
						<br>
						<input type="radio" name="location" value="2ga1dong">성수 2가 1동
						<input type="radio" name="location" value="2ga2dong">성수2가 2동
	
					</form>
				</div>

				<div class="injan">
					<h2>1인 1잔</h2>
					<form action="action.jsp" class="jan">
						<input type="radio" name="jan" value="janYes" checked >예
						<input type="radio" name="jan" value="janNo">아니요

	
					</form>
				</div>

				<div class="useTime">
					<h2>1잔당 이용 가능시간</h2>
					<form action="action.jsp" class="useTime">
						<input type="radio" name="useTime" value="time1" checked >1시간
						<input type="radio" name="useTime" value="time2">2시간
						<input type="radio" name="useTime" value="time3">3시간
						<br>
						<input type="radio" name="useTime" value="time4">4시간
						<input type="radio" name="useTime" value="time5">5시간
						<input type="radio" name="useTime" value="time0">무제한
	
					</form>
				</div>




                <!-- 주요 메뉴 -->
				<div class="mainMenu">
                    <h2>주요메뉴</h2>
                    <div class="menuInput">
                    <input type="text" id="menuInput" placeholder="메뉴를 입력하세요">
                    <input type="button" id="addMenu" value="메뉴 추가">
                    </div>
                    <ul class="menuList"></ul>
                </div>





                <!-- 영업시간 -->
                <div class="workTime">
                    <h2>영업시간</h2>
                    <small>요일별로 입력해주세요.</small><br>
                    <hr>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">월요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">화요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">수요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">목요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">금요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">토요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>
                    <form action="#">
                        <label for="lang" style="font-weight: bolder; margin-right: 5px;">일요일</label>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                        <span>ㅡ</span>
                        <select name="timeN" id="timeI" style="height: 30px; font-size: 15px;">
                            <option value="t0">00:00</option>
                            <option value="t1">01:00</option>
                            <option value="t2">02:00</option>
                            <option value="t3">03:00</option>
                            <option value="t4">04:00</option>
                            <option value="t5">05:00</option>
                            <option value="t6">06:00</option>
                            <option value="t7">07:00</option>
                            <option value="t8">08:00</option>
                            <option value="t9">09:00</option>
                            <option value="t10">10:00</option>
                            <option value="t11">11:00</option>
                            <option value="t12">12:00</option>
                            <option value="t13">13:00</option>
                            <option value="t14">14:00</option>
                            <option value="t15">15:00</option>
                            <option value="t16">16:00</option>
                            <option value="t17">17:00</option>
                            <option value="t18">18:00</option>
                            <option value="t19">19:00</option>
                            <option value="t20">20:00</option>
                            <option value="t21">21:00</option>
                            <option value="t22">22:00</option>
                            <option value="t23">23:00</option>
                        </select>
                    </form>
                    <br>

                </div>




			</div>
		</div>






		<div id="incan">
			<input type="button" value="버튼">
			<input type="button" value="취소">
		</div>

	</div>
    

  <script>

	  /* img upload */
    const inputImage = document.getElementById('inputImage');
    const imageContainer = document.querySelector('.image-container');
    let imageCount = 0;

    inputImage.addEventListener('change', () => {
      const files = inputImage.files;

      if (files.length > 3 - imageCount) {
        alert(`최대 3개의 이미지만 선택 가능합니다.`);
        inputImage.value = '';
        return;
      }

      for (const file of files) {
        if (!file.type.match('image.*')) continue;

        const reader = new FileReader();
        reader.onload = (e) => {
          const img = document.createElement('img');
          img.src = e.target.result;
		  img.classList.add('image-preview');
		  
          img.addEventListener('click', () => {

            const newInput = document.createElement('input');
            newInput.type = 'file';
			newInput.accept = 'image/*';
			
            newInput.addEventListener('change', () => {
              const newFile = newInput.files[0];
              if (!newFile.type.match('image.*')) return;
              const newReader = new FileReader();
              newReader.onload = (newE) => {
                img.src = newE.target.result;
			  };
			  
			  newReader.readAsDataURL(newFile);
			  
            });
            newInput.click();
		  });
		  
          imageContainer.appendChild(img);
          imageCount++;
        };
        reader.readAsDataURL(file);

        if (imageCount >= 3) break;
      }
    });







    /* 메뉴추가 주요메뉴 칸 */

    const menuInput = document.getElementById('menuInput');
    const addMenuBtn = document.getElementById('addMenu');
    const menuList = document.querySelector('.menuList');

    addMenuBtn.addEventListener('click', () => {
      addMenu();
    });

    menuInput.addEventListener('keydown', (e) => {
      if (e.key === 'Enter') {
        addMenu();
        e.preventDefault();
      }
    });

    function addMenu() {
      const menuText = menuInput.value;
      if (menuText === '') return;

      if (menuList.children.length >= 5) {
        alert('최대 5개까지만 입력할 수 있습니다.');
        menuInput.value = ''
        return;
      }

      const li = document.createElement('li');
      li.textContent = menuText;

      const deleteBtn = document.createElement('button');
      deleteBtn.textContent = 'X';
      deleteBtn.addEventListener('click', () => {
        li.remove();
      });

      li.appendChild(deleteBtn);
      menuList.appendChild(li);

      menuInput.value = '';
      menuInput.focus();
    }
     

</script>

</body>
</html>
```
