# mainCSS
```CSS
@charset "UTF-8";

 *{
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
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
	
	.mainReturn {
		text-decoration: none;
	}

	.mainReturn:link {
	color : burlywood;
	}
	.mainReturn:visited {
	color : burlywood;
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








 
        /* container2 */

        #container2{
            width: 100%;
            min-width: 1300px;
            margin-top: 30px;
        }



        #container2>h1{
            color: burlywood;
            font-weight: 10px;
            border-top: 5px double burlywood;
        }

        #container2>div {
            margin: 0 auto;
            margin-top: -30px;
            width: 80vw;
            min-width: 1400px;
            height: 350px;
        }

        #container2>h1 {
            text-align: center;
        }

        #container2 ul {
            display: flex;
        }

        #container2 ul>li {
            margin: 0 auto;
            margin-top: 20px;
            margin-right: 75px;
            list-style: none;
            width: 400px;
            height: 300px;
            border: 3px solid burlywood ;
        }

        #container2 ul>#grade1fi {           
            margin-top: -20px;
            background-image: url("../image/cafe1.jpg");
            background-size: cover;
            filter: grayscale(50%);
        }

        #container2 ul>#grade2se {
            margin-top: 30px;
            background-image: url("../image/cafe2.jpg");
            background-size: cover;
            filter: grayscale(50%);
        }

        #container2 ul>#grade3th {
            margin-top: 30px;
             background-image: url("../image/cafe3.jpg");
            background-size: cover;
            filter: grayscale(50%);
        }

        ul .grade {
            color: white;
            position: relative;
            top: 87%;
            text-align: center;
            line-height: 40px;
            font-weight: bolder;
            background-color: burlywood;
            height: 40px;
            opacity: 90%;
            display: none;
            
        }

        
        #container2 ul li {
            transition: all 0.2s linear;
            margin-left: 30px;
        }

        #container2 ul li:hover {
            transform: scale(1.05);
            cursor: pointer;
        }

        #container2 ul li:hover .grade {
            display: block;
        }

        







        /* container3 */
        
        #container3{
            margin: 0 auto;
            margin-top: 30px;
            width: 73.1%;
            min-width: 1260px;
        }

        #container3Inner>h1{
            font-size: 40px;
            border-bottom: 3px solid burlywood;
            color: burlywood;
        }

        #listUL{
            height: 500px;
            min-width: 1260px;
            padding-left: 10px;
        }

        #listLI{
            margin: 0;
            padding: 0;
            float: left;
            width: 31%;
            height: 350px;
            background-color: lightblue;
            margin-left: 20px;

            margin-bottom: 20px;
        }
```
