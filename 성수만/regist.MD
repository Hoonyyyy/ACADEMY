### regis

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Full Screen Div</title>
    <link rel="stylesheet" href="normalize.css">
	
    <style>

        *{
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }

        body {
            margin: 0 0;
            
            
        }

        #container {
            width: 100%;
            height: 120px;
            min-width: 1300px;
            background-size: cover;

        }

        

        #header {
            width: 80%;
            height: 100px;
            margin: 0 auto;
            margin-top: 20px;
            min-width: 1200px;

        }

        
        

        #header>#headerLeft{
            float: left;
            display: flex;
        }

        #header>#headerLeft>.banner {
            margin-top: 55px;
            font-size: 30px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: burlywood;
            overflow: hidden;

        }

        .banner {
            font-size: 10em;
            color: #fff;
            text-transform: uppercase;
            text-align: center;
            display: flex;
        }

        .banner>span {
            transition: 1.5s;
            animation: anime_textup 1.5s infinite;
        }

        @keyframes anime_textup {
        0% { top: 0; }
        10% { top: -0.3rem; }
        20% { top: 0.2rem; }
        30% { top: -0.1rem; }
        40% { top: 0.1rem; }
        50% { top: -0.05rem; }
        60% { top: 0.05rem; }
        70% { top: -0.02rem; }
        80% { top: 0.02rem; }
        90% { top: -0.01rem; }
        100% { top: 0; }
    }

    .banner span {
        position: relative;
        animation: anime_textup 2s infinite;
    }

    .banner span:nth-of-type(1) {
        animation-delay: 0.15s;
    }

    .banner span:nth-of-type(2) {
        animation-delay: 0.3s;
    }

    .banner span:nth-of-type(3) {
        animation-delay: 0.45s;
    }

    .banner span:nth-of-type(4) {
        animation-delay: 0.6s;
    }

    .banner span:nth-of-type(5) {
        animation-delay: 0.75s;
    }

    .banner span:nth-of-type(6) {
        animation-delay: 0.9s;
    }

    .banner span:nth-of-type(7) {
        animation-delay: 1.05s;
    }

    .banner span:nth-of-type(8) {
        animation-delay: 1.2s;
    }

    .banner span:nth-of-type(9) {
        animation-delay: 1.35s;
    }

    .banner span:nth-of-type(10) {
        animation-delay: 1.5s;
    }

     #header>#headerLeft>.searchBox {
        margin-top: 55px;   
        margin-left: 20px;
        
     }

        .searchInput {
            width: 30%;
            height: 30px;
            min-width: 500px;
        }

        .searchButton {
            height: 30px;
        }


        #header>#headerRight{
            width: 350px;
            float: right;
            margin-top: 50px;
        }



        #고객마당{
            float: left;
            margin-top: 10px;
            display : inline-block;
            width: 120px;
            font-size: 20px;
            font-weight: bolder;
        }


        #고객마당>.dropdown {
            width: 120px;
            display : none;
            font-size: 18px;
        }

        #고객마당>.dropdown a{
            margin: 0 auto;
            display: block;
            text-decoration: none;
            color: black;
        }

        #고객마당>.dropdown a:hover {
            color: burlywood;
        }

        #고객마당:hover .dropdown {
            display: block;
        }

        #점포등록 {
            float: left;
            margin-top: 10px;
            width: 120px;
            font-size: 20px;
            font-weight: bolder;
        }

        #점포등록>a {
            margin: 0 auto;
            text-decoration: none;
            color: black;
        }

        #점포등록>a:hover {
            color: burlywood;
        }

        #로그인 {
            float: left;
            margin-top: 13px;
            width: 50px;
            font-size: 15px;
            font-weight: bolder;
        }

        #로그인>a {
            text-decoration: none;
            color: black;
        }

        #로그인>a:hover {
            color: burlywood;
            transform: scale(1.5);
        }













		/* 등록장 */




		#main>h1{
			text-align: center;
		}

		#main>#registerMain{
			width: 50%;
			min-width: 800px;
			height: 2000px;
			background-color: lightgray;
			margin: 0 auto;
			padding-left: 20px;
			padding-top: 10px;
			
		}
		

		#main textarea{
			width: 97%;
			height: 6.25em;
			border: none;
			resize: none;
		}

		.open>img{
			margin-right: 10px;
		}

		.location2{
			font-size: 20px;
			font-weight: bolder;
		}

		.location2>input{
			margin: 10px;
			width: 15px;
			height: 15px;
		}

		.jan{
			font-size: 20px;
			font-weight: bolder;
		}

		.jan>input{
			margin: 10px;
			width: 15px;
			height: 15px;
		}

		.useTime{
			font-size: 20px;
			font-weight: bolder;
		}

		.useTime>input{
			margin: 10px;
			width: 15px;
			height: 15px;
		}


        
    </style>
</head>
<body>
    
    <div id="container">
        <div id="header">

            <div id="headerLeft">
                <div class="banner">
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
					<img src="./image/cafe1.jpg" width="250px" height="180px">
					<img src="./image/cafe1.jpg" width="250px" height="180px">
					<img src="./image/cafe1.jpg" width="250px" height="180px">
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

				<div class="manu">
					<h2>주요메뉴</h2>

				</div>

				<div class="manu">
					<h2>영업시간</h2>

				</div>



			</div>
		</div>






		<div id="incan">
			<input type="button" value="버튼">
			<input type="button" value="취소">
		</div>

	</div>
    



</body>
</html>
```
