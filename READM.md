# choice_lamb_project

<!DOCTYPE html>
<html>

<head>
    <link rel="stylesheet" href="common.css">
    <meta charset="UTF-8">
    <title>좌측 토글 사이드 바 만들기</title>
    <script src="https://use.fontawesome.com/releases/v5.2.0/js/all.js"></script>
</head>

<body>
    
    <div class="emm">Navigation</div>
    
    
    <ul>
        <li> <a href="#"></a></li>

    </ul>

    <div class="left-side-bar">
        <div class="status-ico">
            <i class="fas fa-bars"></i>
        </div>

        <ul>
            <li>
                <a href="#">Home</a>
                <ul>
                    <li><a href="#">2차 메뉴 아이템1</a></li>
                    <li><a href="#">2차 메뉴 아이템2</a></li>
                </ul>
            </li>
            <li>
                <a href="#">첫번째</a>
                <ul>
                    <li><a href="#">2차 메뉴 아이템1</a></li>
                    <li><a href="#">2차 메뉴 아이템2</a></li>
                </ul>
            </li>
            <li>
                <a href="#">두번째</a>
                <ul>
                    <li><a href="#">2차 메뉴 아이템1</a></li>
                    <li><a href="#">2차 메뉴 아이템2</a></li>
                </ul>
            </li>
            <li>
                <a href="#">네번째</a>
                <ul>
                    <li><a href="#">2차 메뉴 아이템1</a></li>
                    <li><a href="#">2차 메뉴 아이템2</a></li>
                </ul>
            </li>
            <li>
                <a href="#">다섯번째</a>
                <ul>
                    <li><a href="#">2차 메뉴 아이템1</a></li>
                    <li><a href="#">2차 메뉴 아이템2</a></li>
                </ul>
            </li>
        </ul>
    </div>
</body>

<style>

.nav {
  flex: 1;
  width: 10%;
  height: 20px;
  border: 2px solid;
  margin-bottom: 5px;
}
 
ul,
li {
    padding: 0;
    margin: 0;
    list-style: none;
}

a {
    color: inherit;
    text-decoration: none;
}

.left-side-bar > ul ul {
    display: none;
    position: absolute;
    top: 0;
    left: 100%;
    background-color: #dfdfdf;
}


.left-side-bar {
    top: -10px;
    background-color: #dfdfdf;
    height: 1000px;
    width: 185px;
    position: fixed;
    left: -150px;
    transition: left .3s;
}

.left-side-bar > .status-ico {
    text-align: right;
    padding: 10px;
}

.left-side-bar > ul li {
    position: relative;
}

.left-side-bar ul {
    font-weight: bold;
    text-align: center;
    padding: 0;
}

.left-side-bar ul > li > a {
    display: block;
    padding: 10px;
    white-space: nowrap;
}

.left-side-bar:hover {
    left: 0;
}

.left-side-bar ul > li:hover ul {
    display: block;
}

.left-side-bar ul > li:hover > a {
    color: white;
    background-color: black;
}

.left-side-bar > .status-ico > span:last-child {
    display: none;
}

.left-side-bar:hover > .status-ico > span:last-child {
    display: block;
}

.left-side-bar:hover > .status-ico > span:first-child {
    display: none;
}
</style>

</html>