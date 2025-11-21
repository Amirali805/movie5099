<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
     <meta charset="UTF-8">
	 <meta name="viewport" content="width=device-width, initial-scale=1.0">
	 <title>سایت فیلم</title>
	 <style>
	 @import url('https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css');
	 /* استایل‌های قبلی بدون تغییر باقی می‌مانند */
    @import url('https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css');
	 :root{
	 --blank-color:#11151a;
	 --live-color:#f05f5f;
	 --blue-50:#1a2638cc;
	 --blue-color:#1a2638;
	 --light-color:#b465fb;
	 --off-color:#e0e0e0;
	 --yellow:#fb700;
	 --white:#fff;
	 --theme:#b465fb;
	 --font-size-large:22px;
	 --font-size-small:14px;
	 --fw6:600;
	 --fw5:500;
	 --padding-x:120px;
	 }
	 
	 *{
	     margin: 0;
		 padding: 0;
		 box-sizing: border-box;
		 transition: all 0.5s ease;
		 scroll-behavior: smooth;
	 }
	 html{
	     font-family: Vazirmatn, sans-serif;
	 }
	 h1,h2,h3,h4,h5,h6{
	     color: var(--white);
	 }
	 
	 body {
         background-color: var(--blank-color);
		 color: var(--off-color);
     }
	 img{
	     display: block;
		 max-width: 100%;
		 height: auto;
		 pointer-events: none;
	 }
	 input,button,select{
	     font: inherit;
		 background: none;
		 border: none;
		 outline: none;
	 }
	 button{
	     color: var(--off-color);
		 cursor: pointer;
	 }
	 li{
	     list-style: none;
	 }
	 a{
	     text-decoration: none;
		 display: block;
		 color: var(--off-color);
	 }
	 ::-webkit-scrollbar{
	     background: transparent;
	 }
	 ::-webkit-scrollbar-thumb{
	     background: var(--light-color);
		 border-radius: 5rem;
		 border: 3px solid var(--blank-color);
	 }
	 
     header {
         background: linear-gradient(to bottom, rgba(0,0,0,0.7), rgba(0,0,0,0));
         position: absolute;
         top: 0;
         right: 0;
         width: 100%;
         z-index: 10;
     }

     nav {
         margin-right: 200px;
     }

	 .container{
	     max-width: 100%;
		 margin: 0;
	 }
	 
	 /* navbar */
	 /* navbar */
	 .navbar{
	     height: 100px;
		 display: flex;
		 justify-content: space-between;
		 align-items: center;
	 }
	 
	 .navbar-menu-btn{
	     display: none;
	 }
	 nav{
	     margin-right: 200px;
	 }
	 .navbar-nav{
	     display: flex;
	 }
	 .navbar-nav li:not(:last-child){
	     margin-left: 60px;
	 }
	 .navbar-link{
	     font-size: var(--font-size-small);
		 font-weight: var(--fw5);
	 }
	 .navbar-link:hover{
	     color: var(--light-color);
	 }
	 .indicator{
	     position: relative;
	 }
	 .indicator::after{
	     content: "";
		 background: var(--live-color);
		 position: absolute;
		 top: calc(50% - 1px);
		 right: -15px;
		 width: 4px;
		 height: 4px;
		 box-shadow: 0 0 0 2px rgba(240, 95, 95, 0.5);
		 border-radius: 5px;
	 }
	 
	 .navbar-actions{
	     display: flex;
		 align-items: center;
	 }
	 .navbar-form{
	     position: relative;
		 margin-left: 50px;
	 }
	 .navbar-form-search{
	     background: var(--blue-color);
		 width: 100%;
		 padding: 12px 20px;
		 border-radius: 15px;
		 color: var(--off-color);
		 font-size: var(--font-size-small);
		 font-weight: var(--fw5);
	 }
	 .navbar-form-btn{
	     background: var(--blue-color);
		 position: absolute;
		 top: calc(50% - 10px);
		 left: 10px;
	 }
	 .navbar-form-btn ion-icon{
	     font-size: 20px;
		 color: var(--light-color);
	 }
	 .navbar-form-close,
	 .navbar-search-close,
	 .navbar-search-btn {
	     display: none;
	 }
	 .navbar-signin{
	     display: flex;
		 align-items: center;
		 font-size: var(--font-size-small);
	 }
	 .navbar-signin ion-icon{
	     font-size: 22px;
		 color: var(--light-color);
		 margin-left: 5px;
		 transform: rotate(180deg);
	 }
	 .navbar-signin:hover span{
	     color: var(--light-color);
	 }
	 
	 
	 /*banner*/
	 .banner{
	     margin-bottom: 60px;
	 }
	 .banner-card{
	     position: relative;
		 height: 600px;
		 overflow: hidden;
		 border-radius: 20px;
		 cursor: pointer;
	 }
	 
	 .banner-card::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0; /* چون سایت راست‌چینه */
  width: 100%;
  height: 100%;
  background: linear-gradient(to right, rgba(0,0,0,0.8) 30%, rgba(0,0,0,0) 70%);
  z-index: 1;
}

#main-banner img {
  transition: opacity 0.5s ease; /* نیم ثانیه فید */
}

.card-content {
  position: absolute;
  left: 80px;
  bottom: 300px;
  right: auto;
  z-index: 30; /* متن روی لایه تیره بیاد */
}
	 
	 @keyframes rainbow {
  0% { background-position: 0% 50%; }
  100% { background-position: 200% 50%; }
}

.filter-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: var(--blue-color);
  padding: 20px 30px;
  border-radius: 20px;
  margin-bottom: 30px;
  position: relative;
  /* اضافه کردن نوار رنگین‌کمانی مستقیماً به فیلتر بار */
  border: 3px solid transparent;
  background-image: 
    linear-gradient(var(--blue-color), var(--blue-color)),
    linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet);
  background-origin: border-box;
  background-clip: padding-box, border-box;
  background-size: 200% auto;
  animation: rainbow 5s linear infinite;
}

/* حذف یا غیرفعال کردن rainbow-input */
.rainbow-input {
  display: none;
}
	 
	 
/* جایگزین قواعد فعلی .thumbnails, .thumb, .thumb-image */
.thumbnails {
  position: absolute; /* بهتر کنترل در بنر */
  bottom: 2px;       /* قرارگیری در پایین بنر */
  left: 40px;         /* کمی از چپ فاصله */
  width: calc(50% - 80px); /* اشغال حدود نصف پهنای صفحه (مثل عکس) */
  overflow-x: auto;
  white-space: nowrap;
  z-index: 30;
  padding-bottom: 10px;
  scrollbar-width: none;
}

.thumbnails-container {
  display: flex;
  gap: 18px;
  align-items: flex-end; /* تراز پایین کارت‌ها */
}

/* کارت‌ها بلندتر و بزرگتر */
.thumb {
  flex: 0 0 auto;
  width: 180px;                /* پهنای کارت */
  background: rgba(26,38,56,0.65);
  border-radius: 12px;
  overflow: hidden;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
  cursor: grab;
}

/* ارتفاع عکس داخل کارت میشه بیشتر تا کارت بلند به نظر بیاد */
.thumb-image {
  position: relative;
  height: 260px; /* تقریباً نیمی از بنر 700px */
  overflow: hidden;
  border-bottom-left-radius: 12px;
  border-bottom-right-radius: 12px;
}

.thumb-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: transform 0.35s ease;
  -webkit-user-drag: none; /* جلوی درگ تصویر */
  user-drag: none;
  user-select: none;
}

/* وقتی کاربر در حال درگ است (slider.active) افکت های hover حذف شوند */
.thumbnails.active .thumb,
.thumbnails.active .thumb:hover,
.thumbnails.active .thumb:active {
  transform: none !important;
  box-shadow: none !important;
  transition: none !important;
  cursor: grabbing !important;
}

/* همچنین اگر خواستی hover معمولی کارت ها را کم رنگ‌تر کنی (در حالت نرمال) */
.thumb:hover {
  transform: translateY(-8px);
  box-shadow: 0 18px 30px rgba(0,0,0,0.6);
}

/* جلوگیری از انتخاب متن و هایلایت تصاویر در ناحیه تامبنیل */
.thumbnails, .thumbnails * {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  -webkit-touch-callout: none;
}

/* اگر در بالای فایل global img pointer-events: none; هست، برای تامبنیل تصویر را فعال کن */
.thumbnails img {
  pointer-events: auto;
}

.thumb-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.thumb:hover .thumb-overlay {
  opacity: 1;
}

.thumb-overlay ion-icon {
  font-size: 40px;
  color: var(--white);
}

.thumb-title {
  font-size: 14px;
  font-weight: var(--fw6);
  color: var(--white);
  margin-bottom: 8px;
  text-align: center;
  margin-top: 8px;
}

.thumb-rating ion-icon {
  font-size: 12px;
  margin-left: 4px;
}

/* اسکرول بار برای تامبنیل‌ها */
.thumbnails::-webkit-scrollbar {
  display: none;
}

.thumbnails::-webkit-scrollbar-thumb {
  background: var(--light-color);
  border-radius: 3px;
}

.thumbnails::-webkit-scrollbar-track {
  background: rgba(255, 255, 255, 0.1);
  border-radius: 3px;
}

.thumb.active {
  border: 3px solid var(--theme); /* خط بنفش */
  transform: scale(1.05);         /* کمی بزرگتر واسه جذابیت */
  z-index: 50;                    /* بیاد جلو بقیه */
}

.thumb {
  transition: transform 0.3s ease, opacity 0.3s ease;
}
.thumb.active {
  transform: scale(1.1);  /* بزرگ‌تر بشه */
  opacity: 1;
}
.thumb:not(.active) {
  opacity: 0.6;           /* بقیه کم‌رنگ‌تر بشن */
}

		.banner-card img,
        .category-card img,
        .card-head img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
		
		.banner-card image
	 
	 .card-content{
	     position: absolute;
		 right: 80px;
		 bottom: 60px;
		 left: 80px;
	 }
	 .card-info{
	     display: flex;
		 align-items: center;
		 margin-bottom: 20px;
	 }
	 .card-info div{
	     display: flex;
		 align-items: center;
		 margin-left: 20px;
	 }
	 .card-info ion-icon{
	     font-size: 20px;
		 color: var(--theme);
		 margin-left: 5px;
	 }
	 .card-info span{
	     font-weight: var(--fw6);
	 }
	 .quality{
	     background-color: var(--theme);
		 padding: 2px 5px;
		 border-radius: 5px;
		 font-weight: 700;
	 }
	 .card-title{
	     font-size: 3em;
		 color: var(--white);
		 text-shadow: 2px 0 2px #0007;
	 }
	 .banner img{
	     object-position: top;
	 }
	 
	 /*movies*/
	 .movies{
	     margin-bottom: 60px;
	 }
	 .filter-bar{
	     display: flex;
		 justify-content: space-between;
		 align-items: center;
		 background-color: var(--blue-color);
		 padding: 20px 30px;
		 border-radius: 20px;
		 margin-bottom: 30px;
	 }
	 .filter-bar select{
	     color: var(--white);
		 font-size: var(--font-size-small);
		 margin-left: 15px;
		 cursor: pointer;
	 }
	 .filter-bar option{
	     background: var(--blank-color);
	 }
	 
	 .filter-radius{
	     position: relative;
		 background-color: var(--blank-color);
		 padding: 10px;
		 border-radius: 15px;
	 }
	 .filter-radius input{
	     display: none;
	 }
	 .filter-radius label{
	     position: relative;
		 margin: 0 10px;
		 font-size: var(--font-size-small);
		 user-select: none;
		 cursor: pointer;
		 z-index: 10;
	 }
	 .filter-radius input:checked + label,
	 .filter-radius label:hover{
	     color: var(--light-color);
	 }
	 input ~ .checked-radio-bg{
	     --width: 55px;
		 --left: 5px;
		 background-color: var(--blue-color);
		 position: absolute;
		 top: 5px;
		 right: var(--left);
		 bottom: 5px;
		 width: var(--width);
		 border-radius: 10px;
	 }
	 #popular:checked ~ .checked-radio-bg{
	     --width: 59px;
		 --left: 60px;
	 }
	 #newest:checked ~ .checked-radio-bg{
	     --width: 69px;
		 --left: 125px;
	 }
	 .movies-grid{
	     display: grid;
		 grid-template-columns: repeat(auto-fill , minmax(140px , 1fr));
		 gap: 30px;
		 margin-button: 60px;
	 }
	 
	 .movie-card{
	     --scale:0.8;
		 cursor: pointer;
	 }
	 .card-head{
	     position: relative;
		 height: 250px;
		 border-radius: 15px;
		 margin-bottom: 15px;
		 overflow: hidden;
	 }
	 .card-overlay{
	     position: absolute;
		 inset: 0;
		 opacity: 0;
		 backdrop-filter: blur(5px);
	 }
	 .movie-card:hover .card-overlay{
	     opacity: 1;
	 }
	 .movie-card .bookmark ,
	 .movie-card .rating{
	     position: absolute;
		 top: 15px;
		 padding: 6px;
		 border-radius: 10px;
		 color: var(--light-color);
		 transform: scale(var(--scale));
	 }
	 .movie-card .bookmark{
	     background: var(--blue-color);
		 right: 15px;
	 }
	 .movie-card .bookmark:hover{
	     color: var(--yellow);
	 }
	 .movie-card .rating{
	     display: flex;
		 align-items: center;
		 left: 15px;
		 background-color: var(--blue-50);
	 }
	 .movie-card .rating span {
	     color: var(--white);
		 font-size: 13px;
		 font-weight: var(--fw5);
		 margin-right: 5px;
	 }
	 .movie-card ion-icon{
	     font-size: 16px;
		 display: block;
	 }
	 .movie-card .play{
	     position: absolute;
		 top: 50%;
		 left: 50%;
		 transform: translate(-50% , -50%) scale(var(--scale));
	 }
	 .movie-card .play ion-icon{
	     font-size: 60px;
	 }
	 .movie-card .card-title{
	     font-size: 17px;
		 font-weight: var(--fw5);
		 margin-bottom: 5px;
		 text-align: center;
	 }
	 .movie-card:hover .card-title{
	     color: var(--light-color);
	 }
	 .movie-card .card-info{
	     display: flex;
		 justify-content:space-evenly;
		 font-size: var(--font-size-small);
		 font-weight: var(--fw5);
	 }
	 
	 .load-more{
	     background: var(--blue-color);
		 display: block;
		 padding: 20px 50px;
		 margin: auto;
		 font-size: var(--font-size-small);
		 font-weight: var(--fw5);
		 border-radius: 15px;
		 color: var(--white);
	 }
	 .load-more:hover{
	     background-color: var(--light-color);
	 }
	 
	 /*category*/
	 .section-heading{
	     font-size: 40px;
		 font-weight: var(--fw5);
		 margin-bottom: 60px;
	 }
	 .category{
	     margin-bottom: 60px;
	 }
	 .category-grid{
	     display: grid;
		 grid-template-columns: repeat(4, 1fr);
		 gap: 30px;
	 }
	 
	 .category-card{
	     position: relative;
		 height: 150px;
		 border-radius: 20px;
		 overflow: hidden;
		 cursor: pointer;
	 }
	 .category-card::after{
	     content: "";
		 position: absolute;
		 inset: 0;
		 background: linear-gradient(180deg, transparent, 20%, #000a);
	 }
	 .category-card .name,
	 .category-card .total {
	     position: absolute;
		 bottom: 20px;
		 color: var(--white);
		 z-index: 20;
	 }
	 .category-card .name{
	     right: 20px;
		 font-size: 20px;
	 }
	 .category-card:hover .name{
	     color: var(--light-color);
	 }
	 .category-card .total{
	     left: 20px;
		 font-size: 10px;
		 background: var(--blue-50);
		 padding: 5px 8px;
		 border-radius: 8px;
	 }
	 
	 /*live*/
	 .live{
	     margin-bottom: 60px;
	 }
	 .live-grid{
	     display: grid;
		 grid-template-columns: repeat(auto-fit, minmax(250px , 1fr));
		 gap: 30px;
	 }
	 .live-card{
	     cursor: pointer;
	 }
	 .live-card .card-head{
	     position: relative;
		 height: 250px;
		 border-radius: 20px;
		 margin-bottom: 15px;
		 overflow: hidden;
	 }
	 .live-card .card-head::after{
	     content: "";
		 position: absolute;
		 inset: 0;
		 background: linear-gradient(180deg, transparent 20%, #000a)
	 }
	 .live-card:hover .card-head img{
	     transform: scale(1.1);
	 }
	 .live-card .live-badge,
	 .live-card .total-viewers{
	     position: absolute;
		 right: 30px;
		 border-radius: 10px;
		 padding: 5px 10px;
		 z-index: 10;
	 }
	 .live-card .live-badge{
	     top: 30px;
		 font-size: var(--font-size-small);
		 font-weight: var(--fw5);
		 background-color: var(--live-color);
	 }
	 .live-card .total-viewers{
	     bottom: 20px;
		 font-size: 15px;
		 font-weight: var(--fw6);
		 background-color: var(--blue-50);
	 }
	 .live-card .play{
	     position: absolute;
		 top: 50%;
		 left: 50%;
		 transform: translate(-50% , -50%) scale(0.8);
		 z-index: 10;
	 }
	 .live-card:hover .play{
	     transform: translate(-50%, -50%) scale(1);
		 opacity: 1;
	 }
	 .live-card .play ino-icon{
	     font-size: 60px;
	 }
	 .live-card .card-body{
	     display: flex;
		 justify-content: flex-start;
		 align-items: flex-start;
	 }
	 .live-card .card-body img{
	     width: 40px;
		 border-radius: 10px;
		 margin-left: 15px;
	 }
	 .live-card .card-title{
	     font-size: var(--font-size-large);
		 font-weight: var(--fw5);
	 }
	 .live-card:hover .card-title{
	     color: var(--light-color);
	 }
	 
	 /*footer*/
	 .footer{
	     background: rgb(17, 22, 29);
		 padding: 80px var(--padding-x) 40px;
	 }
	 .footer-content{
	     display: flex;
		 justify-content: space-between;
		 align-items: flex-start;
		 border-bottom: 1px solid var(--blue-50);
		 padding-bottom: 80px;
	 }
	 .footer-brand{
	     max-width: 250px;
	     margin-left: 130px;
	 }
	 .footer-brand img {
	     width: 100px;
	     margin-bottom: 30px;
	 }
	 .des {
	     font-size: var(--font-size-small);
		 line-height: 20px;
		 margin-bottom: 20px;
	 }
	 .social-link{
	     display: inline-block;
	 }
	 .footer-links{
	     display: grid;
		 width: 100%;
		 grid-template-columns: repeat(4 ,1fr);
		 gap: 50px;
		 align-items: flex-end;
	 }
	 .link-heading{
	     margin-bottom: 20px;
	 }
	 .link-item {
	     font-size: var(--font-size-small);
	 }
	 ul .link-item:not(:last-child) {
	     margin-bottom: 10px;
	 }
	 .link-item:hover a{
	     color: var(--light-color);
	 }
	 .footer-coypright{
	     display: flex;
		 justify-content: space-between;
		 align-items: center;
		 padding-top: 40px;
	 }
	 .footer-coypright p ,
	 .wrapper a{
	     font-size: var(--font-size-small);
	 }
	 .wrapper a:hover{
	     color: var(--light-color);
	 }
	 .wrapper {
	     display: flex;
	 }
	 .wrapper a:not(:last-child) {
	     margin-left: 50px;
	 }
	 
	 @media screen and (max-width:1200px) {
		 
		 header{
		     position: fixed;
			 top: 0;
			 right: 0;
			 width: 100%;
			 overflow: hidden;
			 z-index: 50;
		 }
		 header.active{
		     top: 250px;
		 }
		 .navbar-menu-btn{
		     display: block;
			 position: absolute;
			 top: 50%;
			 right: var(--padding-x);
			 transform: translateY(-50%);
		 }
		 .navbar-menu-btn span{
		     display: block;
			 background-color: var(--off-color);
			 width: 25px;
			 height: 2px;
			 margin: 8px;
		 }
		 .navbar-search-btn {
		     display: block;
			 font-size: 20px;
			 color: var(--light-color);
			 margin: 10px;
		 }
		 .navbar-menu-btn.active span {
		     background-color: var(--light-color);
		 }
		 .navbar-menu-btn .tow {
		     width: 20px;
		 }
		 .navbar-menu-btn .three {
		     width: 15px;
		 }
		 .navbar-menu-btn.active .one {
		     transform: rotate(45deg) translateY(14px);
		 }
		 .navbar-menu-btn.active .tow {
		     width: 0;
		 }
		 .navbar-menu-btn.active .three {
		     width: 25px;
			 transform: rotate(-45deg) translateY(-14px);
		 }
		 .navbar-brand{
		     margin-right: 50px;
		 }
		 nav{
		     position: fixed;
			 top: -250px;
			 left: 0;
			 width: 100%;
			 z-index: 100;
		 }
		 nav.active{
		     top: 0;
		 }
		 .navbar-nav{
		     height: 250px;
			 flex-direction: column;
			 justify-content: center;
			 align-items: flex-start;
			 padding-right: var(--padding-x);
			 border-bottom: 1px solid var(--blank-color);
		 }
		 .navbar-nav li:not(:last-child){
		     margin-right: 0;
			 margin-bottom: 30px
		 }
		 .navbar-form{
		     position: absolute;
			 top: 100%;
			 left: var(--padding-x);
			 right: var(--padding-x);
			 height: 100%;
			 background-color: var(--blank-color);
			 margin-right: 0;
			 display: flex;
			 justify-content: space-between;
			 align-items: center;
			 z-index: 100;
		 }
		 .navbar-form.active{
		     top: 0;
		 }
		 .navbar-form{
		     margin-left: 40px;
		 }
		 .navbar-form-close{
		     display: block;
			 padding-top: 4px;
			 opacity: 0.8;
		 }
		 .navbar-form-close:hover{
		     opacity: 1;
		 }
		 .navbar-form-close ino-icon{
		     font-size: 30px;
			 color: var(--light-color);
		 }
		 .navbar-search-btn{
		     display: block;
			 margin-left: 100px;
			 padding-top: 5px;
		 }
		 .banner{
		     margin-top: 100px;
		 }
		 .category-grid{
		     grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		 }
		 .banner-card .card-title{
		     font-size: 2.5em;
		 }
		 .footer-content{
		     flex-direction: column;
		 }
		 .footer-brand{
		     margin-left: 0;
			 margin-bottom: 60px;
		 }
		 .footer-links{
		     grid-template-columns: repeat(auto-fit, minmax(125px, 1fr));
		 }
		 navbar-form-btn{
		     left: 120px;
		 }
		 navbar-form-search{
		     margin-left: 80px;
		 }
		 
		 @media screen and (max-width:768px){
		     :root{
			     --padding-x: 40px;
			 }
			 .banner{
			     display: none;
			 }
			 .movies{
			     margin-top: 120px;
			 }
			 .filter-bar{
			     flex-direction: column;
				 align-items: center;
			 }
			 .filter-bar select{
			     margin-bottom: 20px;
			 }
		 }
		 @media screen and (max-width: 576px){
		     :root{
			     --padding-x: 20px;
				 --font-size-large: 20px;
			 }
			 .navbar-search-btn{
			     margin-left: 20px;
			 }
			 .navbar-form-search{
			     margin-left: 20px;
			 }
			 .navbar-form-btn{
			     left: 55px;
			 }
			 .footer-coypright{
			     flex-direction: column;
			 }
			 .wrapper{
			     margin-bottom: 20px;
			 }
	 }
	 </style>
</head>
<body>
     <div class="container">
	 <header>
	     <div class="navbar">
		     <button class="menu-btn navbar-menu-btn">
			     <span class="one"></span>
				 <span class="tow"></span>
				 <span class="three"></span>
			 </button>
			 <a href="#" class="navbar-brand">
			    <img src="" alt="logo">
				<span class="logo-text">falcon movie</span>
			 </a>
			<nav>
			    <ul class="navbar-nav">
				     <li>
					     <a href="#" class="navbar-link">خانه</a>
				     </li>
					 <li><a href="#category" class="navbar-link">دسته بندی ها</a></li>
					 <li><a href="#category" class="navbar-link">ژانر ها</a></li>
					 <li>
					     <a href="#live" class="navbar-link indicator">پخش زنده</a>
					 </li>
				</ul>
			 </nav>
			 <div class="navbar-actions">
				     <form action="" class="navbar-form">
					     <input
						 type="text" 
						 name="search" 
						 placeholder="دنبال چی میگردی؟..."
						 class="navbar-form-search"
						 />
						 <button class="navbar-form-btn">
						     <ion-icon name="search-outline"></ion-icon>
						 </button>
						 
						 <button class="navbar-form-close">
						     <ion-icon name="close-circle-outline"></ion-icon>
						 </button>
						 <button class="navbar-search-close">
						     <ion-icon name="close-outline"></ion-icon>
						 </button>
					 </form>
					  <button class="navbar-search-btn">
						     <ion-icon name="search"></ion-icon>
						 </button>
						 
					 <a href="#" class="navbar-signin">
					<span>ورود</span>
					<ion-icon name="log-in-outline"></ion-icon>
					</a>
				</div>
		 </div>
	 </header>
	 <main>
	     <section class="banner">
		     <div class="banner-card active" id="main-banner">
			     <img src="https://img9.irna.ir/d/r2/2020/10/17/4/157675241.jpg" alt="">
				 <div class="card-content">
				     <div class="card-info">
					     <div class="genre">
						     <ion-icon name="film-outline"></ion-icon>
							 <span>اکشن / هیجان انگیز</span>
						 </div>
						 <div class="year">
						     <ion-icon name="calendar-outline"></ion-icon>
							 <span>2019</span>
						 </div>
						 <div class="duration">
						     <ion-icon name="time-outline"></ion-icon>
							 <span>2h 11min</span>
						 </div>
						 <div class="quality">4k</div>
					 </div>
					 <h2 class="card-title"> جان ویک: بخش 3 - پارابلوم</h2>
				 </div>
				 
				 <!-- thumbnail ها دقیقاً مانند فایل indexsquid game -->
    <!-- thumbnail ها -->
	
	<div class="thumbnails">
  <div class="thumbnails-container">
    <div class="thumb" data-index="0">
      <div class="thumb-image">
        <img src="https://bbu5.sbs/wp-content/uploads/2025/08/Jurassic-World-Rebirth-2025.jpg" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
	
	<div class="thumb" data-index="1">
      <div class="thumb-image">
        <img src="https://api2.zoomg.ir/media/2018-3-8b9e4f3f-d243-4012-8656-ebc12187b0cb-66cc7d012b5676090d00b39a" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
	
	<div class="thumb" data-index="2">
      <div class="thumb-image">
        <img src="https://salamcinama.ir/api/filedb/a3c2c612/%D9%81%D8%B5%D9%84-%D8%AF%D9%88%D9%85-%D9%88%D9%86%D8%B2%D8%AF%DB%8C.jpg?w=any&q=75" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
	
	<div class="thumb" data-index="3">
      <div class="thumb-image">
        <img src="https://gamotionart.com/wp-content/uploads/2024/11/arcane-season-2-changes-too-many-things-1024x576.jpg" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
	
	<div class="thumb" data-index="4">
      <div class="thumb-image">
        <img src="https://gamefa.com/wp-content/uploads/2021/11/Wonder-Woman-Gal-Gadot-with-shield.jpg.webp" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
	
	<div class="thumb" data-index="5">
      <div class="thumb-image">
        <img src="https://static.namava.ir/Content/Upload/Images/f329df9c-a7e0-4bff-be0f-383b702afd5c.jpg?anchor=middlecenter&crop=auto&scale=both&w=1280&h=600" alt="جان ویک">
        <div class="thumb-overlay">
          <ion-icon name="play-circle-outline"></ion-icon>
        </div>
      </div>
    </div>
	
    <!-- تکرار برای سایر تامبنیل‌ها -->
  </div>
</div>
	
		 </section>
		    
		 <section class="movies">
		     <div class="filter-bar">
			     <div class="filter-dropdowns">
				 <select class="genre">
					     <option value="all genre">فیلم/سریال</option>
						 <option value="movie">فیلم</option>
						 <option value="serius">سریال</option>
					 </select>
				     <select class="genre">
					     <option value="all genre">همه ژانر ها</option>
						 <option value="action">اکشن</option>
						 <option value="adventure">ماجراجویی</option>
						 <option value="animal">حیوانات</option>
						 <option value="animation">انیمیشن</option>
						 <option value="biography">زندگینامه</option>
						 <option value="drama">درام</option>
						 <option value="fantasy">فانتزی</option>
						 <option value="horror">ترسناک</option>
						 <option value="science fiction">علمی تخیلی</option>
						 <option value="war">جنگی</option>
					 </select>
					 <select class="year">
					     <option value="">همه سال ها</option>
						 <option value="">2024</option>
						 <option value="">2020-2023</option>
						 <option value="">2010-2019</option>
						 <option value="">2000-2009</option>
						 <option value="">1980-1999</option>
					 </select>
					 <select class="cline">
					     <option value="">مرتب سازی</option>
						 <option value="">بروزترین</option>
						 <option value="">جدیدترین</option>
						 <option value="">محبوب ترین</option>
						 <option value="">امتیاز IMDB</option>
						 <option value="">سال انتشار</option>
					 </select>
				 </div>
				 <div class="filter-radius">
				     <input type="radio" name="input" id="featured" checked>
					 <label for="featured">ویژه</label>
					 <input type="radio" name="input" id="popular" >
					 <label for="popular">محبوب</label>
					 <input type="radio" name="input" id="newest" >
					 <label for="newest">جدید ترین</label>
					 <div class="checked-radio-bg"></div>
				 </div>
			 </div>
			 <div class="movies-grid">
			 
			 <!--کارت فیلم-->
			     <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://i.pinimg.com/736x/f5/69/d3/f569d38f9a955218efe75837bebfcf10.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>6.3</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">بتمن علیه سوپرمن</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2021</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://upload.wikimedia.org/wikipedia/fa/0/0c/Red_Notice_-_film_promotional_image.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>7.5</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">اعلان قرمز</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2021</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9p_KYh03odvqWi05C9MaWMsKbrSfRJzw7lg&s"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.1</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">بتمن شوالیه تاریکی</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / رازالود</span>
								 <span class="year">2008</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://upload.wikimedia.org/wikipedia/fa/e/ed/Wonder_Woman_%282017_film%29.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.5</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">واندر وومن</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنگی</span>
								 <span class="year">2018</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://subtitlestar.com/wp-content/uploads/2019/10/tt6095472-236x350.jpg.webp"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>7.2</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">پرندگان خشمگین 2</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2022</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://4kdownload.org/wp-content/uploads/2023/04/MV5BNzQ5NzgwNDA4MF5BMl5BanBnXkFtZTgwNTQ5NDY4MDI@._V1_SX.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.9</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">رزیدنت اویل</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / اخرلزمانی</span>
								 <span class="year">2006</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://rozup.ir/view/3239936/Birds-of-Prey-2020_625703.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>7.4</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">پرندگان شکاری</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2020</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://img.uptvs.com/uploads/2024/12/Squid-Game-2025-Season-3.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.4</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">اسکویید گیم</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی</span>
								 <span class="year">2025</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://upmedia.movie/wp-content/uploads/2025/08/Wednesday-2-2025-540x797.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.1</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">ونزدی</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی/رازالود</span>
								 <span class="year">2025</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://files.virgool.io/upload/users/3003781/posts/dfj5tltombag/7h2zxmp4wsnm.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>6.6</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">جوکر</h3>
							 
						     <div class="card-info">
							     <span class="genre">کمدی تاریک / جنایی</span>
								 <span class="year">2024</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://www.film2serial.ir/wp-content/uploads/2025/07/kpop-demon-hunters.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>0</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">شکارچیان کیپاپ</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / فانتزی / موزیکال</span>
								 <span class="year">2025</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://static.cdn.asset.filimo.com/flmt/mov_160424_291550-b.jpg?width=300&quality=85&sharpen=80&secret=09l_ZoVNYQiXLk5u_FscSg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>7.4</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">مگان</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی / علمی تخیلی</span>
								 <span class="year">2025</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://m.media-amazon.com/images/I/71niXI3lxlL._AC_SY679_.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.6</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">انتقام جویان </h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / علمی تخیلی / ابرقهرمانی</span>
								 <span class="year">2019</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://images.plex.tv/photo?size=large-1920&scale=1&url=https%3A%2F%2Fmetadata-static.plex.tv%2Fa%2Fplex%2Fa3d9b641-933e-49b7-92e7-9d3ab891e7f0.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.6</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">بالرین</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی</span>
								 <span class="year">2025</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://www.disfilm.ir/wp-content/uploads/2024/04/disfilm_poster_17058_60964.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.7</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">باربی</h3>
							 
						     <div class="card-info">
							     <span class="genre">موزیکال / کمدی</span>
								 <span class="year">2023</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://cloud.filmfed.com/movies/posters/m_878b3ed7-badf-40c6-91f9-3e5cde4843c0.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.4</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">هیتمن</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی / رازالود</span>
								 <span class="year">2012</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://www.doostihaa.com/img/uploads/2023/03/John-Wick-Chapter-4-2023.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.8</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">جان ویک</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی / رزمی کاری</span>
								 <span class="year">2024</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTjQ97ExJjMXhiO4s8V6OKRe9VZ8pJ1lsiFOQ&s"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.1</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">جانی انگلیش</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2015</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://upmedia.movie/wp-content/uploads/2024/10/Breaking-Bad.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.6</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">بریکینگ بد</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی</span>
								 <span class="year">2012</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://zardfilm.in/wp-content/uploads/2024/02/MV5BZjhmZTlkOTAtYTE0Yi00Yjg2LTg5M2UtNWNmNTZkZGM4ODRmXkEyXkFqcGdeQXVyMTI4NjgxNTk5._V1_.webp"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.7</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">مرد عنکبوتی</h3>
							 
						     <div class="card-info">
							     <span class="genre">ابرقهرمانی / جنگی</span>
								 <span class="year">2023</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://upload.wikimedia.org/wikipedia/fa/5/5f/Terminator_Dark_Fate_poster.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.4</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">ترمیناتور</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی / رازالود</span>
								 <span class="year">2021</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://static.cdn.asset.filimo.com/flmt/mov_6796_183918-b.jpg?width=300&quality=85&sharpen=80&secret=SF-biKzPpN9x1q9yjLGnWA"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>9.8</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">مکانیک</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / جنایی / رزمی کاری</span>
								 <span class="year">2013</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://topfilme.ir/wp-content/uploads/2025/06/terrifier-2-21332.jpg"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.1</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">تریفایر</h3>
							 
						     <div class="card-info">
							     <span class="genre">ترسناک / جنایی</span>
								 <span class="year">2022</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <div class="movie-card">
				     <div class="card-head">
					     <img 
						     src="https://cdn.gapfilm.ir/image/362/panel/19856/portrait.jpg?updateTime=1756220364000"
							 alt="move"
							 class="card-img"
							 />
						 <div class="card-overlay">
					     <div class="bookmark">
						     <ion-icon 
							 name="bookmark"
							 role="img"
							 class="md hydrated"
							 ></ion-icon>
						 </div>
						  <div class="rating">
						     <ion-icon 
						     name="star-outline"
						     role="img"
						     class="md hydrated"
						     ></ion-icon>
						     <span>8.1</span>
						 </div>
						 
						 <div class="play">
						     <ion-icon name="play-outline"></ion-icon>
						 </div>
					    </div>
					 </div>
					     <div class="card-body">
					         <h3 class="card-title">اتک ان تایتان</h3>
							 
						     <div class="card-info">
							     <span class="genre">اکشن / کمدی</span>
								 <span class="year">2015</span>
							 </div>
					     </div>
					 </div>
					 
					 
					 <!--کارت فیلم-->
					 
				 </div>
			 </div>
			 <button class="load-more">نمایش بیشتر</button>
		 </section>
		 
		 
		 <section class="category" id="category">
		     <h2 class="section-heading">دسته بندی</h2>
			 
			 <div class="category-grid">
			     <div class="category-card">
				     <img src="https://vigiato.net/wp-content/uploads/2024/02/983569-scaled.jpg" alt="action">
					 
					 <div class="name">اکشن</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://www.digikala.com/mag/wp-content/uploads/2024/10/l-intro-1685593026-1.jpg" alt="action">
					 
					 <div class="name">ترسناک</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://rooziato.com/wp-content/uploads/2018/09/63e6691f2b57118db36d04d7b1ab6a47.jpg" alt="action">
					 
					 <div class="name">کمدی</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://cdn.plaza.ir/images/681f1a8e75fbfaeab706478d" alt="action">
					 
					 <div class="name">جنگی</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://w0.peakpx.com/wallpaper/816/938/HD-wallpaper-justice-league-warworld-2023-justice-league-movie-comics-poster-superman-wonder-woman-art-man-girl-warworld-fantasy-batman.jpg" alt="action">
					 
					 <div class="name">انیمیشن</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://files.virgool.io/upload/users/43899/posts/sxopbwnhpkjw/or8ustfnpqw6.jpeg" alt="action">
					 
					 <div class="name">ماجراجویی</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://www.digikala.com/mag/wp-content/uploads/2025/08/jurassic-world-rebirth-Main-1.jpg" alt="action">
					 
					 <div class="name">علمی تخیلی</div>
					 <div class="total">100</div>
				 </div>
				 
				 <div class="category-card">
				     <img src="https://ts18.tarafdari.com/contents/user847016/content-article/squid-game-season-2-world-premiere-cast-release-date-1.jpeg" alt="action">
					 
					 <div class="name">جنایی</div>
					 <div class="total">100</div>
				 </div>
			 </div>
		 </section>
		 
		 
		 <section class="live" id="live">
		     <h2 class="section-heading">برنامه های زنده</h2>
			     <div class="live-grid">
			        <div class="live-card">
					     <div class="card-head">
						 	<img src="https://files.virgool.io/upload/users/71426/posts/fucdafkbt2ml/8csrbn1xy0kg.png" alt="">
					        <div class="live-badge">زنده</div>
					        <div class="total-viewers">308k بیننده</div>
							<div class="play">
							     <ion-icon name="play-outline"></ion-icon>
							</div>
						 </div>
                        <div class="card-body">
						     <img src="https://upload.wikimedia.org/wikipedia/commons/d/de/HBO_logo.svg" alt="">
							 <h3 class="card-title">
							    برکینگ بد
							 <br> 
							    فصل 1 - قسمت 1
							 </h3>
						</div>
			        </div>
					
					<div class="live-card">
					     <div class="card-head">
						 	<img src="https://vigiato.net/wp-content/uploads/2021/07/JPUDUENHAVBLAOFVOC7W6EYPXI-1024x614.jpg" alt="">
					        <div class="live-badge">زنده</div>
					        <div class="total-viewers">308k بیننده</div>
							<div class="play">
							     <ion-icon name="play-outline"></ion-icon>
							</div>
						 </div>
                        <div class="card-body">
						     <img src="https://upload.wikimedia.org/wikipedia/commons/d/de/HBO_logo.svg" alt="">
							 <h3 class="card-title">
							    گیم اف ترونز
							 <br> 
							    فصل 1 - قسمت 1
							 </h3>
						</div>
			        </div>
					
					
					<div class="live-card">
					     <div class="card-head">
						 	<img src="https://dl.psarena.ir/wp-content/uploads/2021/09/977365-moneyheist-part5-photos1.jpg" alt="">
					        <div class="live-badge">زنده</div>
					        <div class="total-viewers">308k بیننده</div>
							<div class="play">
							     <ion-icon name="play-outline"></ion-icon>
							</div>
						 </div>
                        <div class="card-body">
						     <img src="https://upload.wikimedia.org/wikipedia/commons/d/de/HBO_logo.svg" alt="">
							 <h3 class="card-title">
							    خانه کاغذی
							 <br> 
							    فصل 1 - قسمت 1
							 </h3>
						</div>
			        </div>
			     </div>
		 </section>
		 
	 </main>
	 
	 
	 <footer>
	     <div class="footer-content">
		    <div class="footer-brand">
			     <img src="" alt="logo">
				 <p class="des">
				 سینما انلاین تماشای فیلم وسریال
			     </p>
				 
				 
				 <div class="social-link">
				     <a href="#"><ion-icon name="logo-youtube"></ion-icon></a>
					 <a href="#"><ion-icon name="logo-instagram"></ion-icon></a>
				 </div>
			</div>
			     <div class="footer-links">
				     <ul>
					     <h4 class="link-heading">سینما انلاین </h4>
					     <li class="link-item"><a href="#">درباره ما</a></li>
						 <li class="link-item"><a href="#">پروفایل من</a></li>
						 <li class="link-item"><a href="#">طرح های قیمت گزاری</a></li>
						 <li class="link-item"><a href="#">تماس با ما</a></li>
					 </ul>
					 
					 <ul>
					     <h4 class="link-heading">مرور </h4>
					     <li class="link-item"><a href="#">درباره ما</a></li>
						 <li class="link-item"><a href="#">پروفایل من</a></li>
						 <li class="link-item"><a href="#">طرح های قیمت گزاری</a></li>
						 <li class="link-item"><a href="#">تماس با ما</a></li>
					 </ul>
					 
					 <ul>
					     <h4 class="link-heading">محتوای ما </h4>
					     <li class="link-item"><a href="#">درباره ما</a></li>
						 <li class="link-item"><a href="#">پروفایل من</a></li>
						 <li class="link-item"><a href="#">طرح های قیمت گزاری</a></li>
						 <li class="link-item"><a href="#">تماس با ما</a></li>
					 </ul>
					 
					 <ul>
					     <h4 class="link-heading">راهنما </h4>
					     <li class="link-item"><a href="#">درباره ما</a></li>
						 <li class="link-item"><a href="#">پروفایل من</a></li>
						 <li class="link-item"><a href="#">طرح های قیمت گزاری</a></li>
						 <li class="link-item"><a href="#">تماس با ما</a></li>
					 </ul>
				 </div>
		 </div>
		 <div class="footer-coypright">
		     <div class="coypright">
			     <p> کلیه حقوق محفوظ است 1404 فالکون مووی ☺ </p>
			 </div>
			 <div class="wrapper">
			     <a href="#">حریم خصوصی </a>
				 <a href="#">قوانین و شرایط </a>
			 </div>
	 </footer>
   </div>
	 
	 
	 
	 <script src="https://unpkg.com/scrollreveal"></script>
	 <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
<script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>

<script>
const header = document.querySelector("header");
  const nav = document.querySelector("nav");
  const navbarMenuBtn = document.querySelector(".navbar-menu-btn");

  function navIsActive() {
    header.classList.toggle("active");
    nav.classList.toggle("active");
    navbarMenuBtn.classList.toggle("active");
  }

  navbarMenuBtn.addEventListener("click", navIsActive);

  const navbarForm = document.querySelector(".navbar-form");
  const navbarFormClose = document.querySelector(".navbar-form-close");
  const navbarSearchBtn = document.querySelector(".navbar-search-btn");

  const searchBarIsActive = () => navbarForm.classList.toggle("active");

  navbarSearchBtn.addEventListener("click", searchBarIsActive);
  navbarFormClose.addEventListener("click", searchBarIsActive);

// اطلاعات فیلم‌ها
        const moviesData = [
            {
                image: "https://bbu5.sbs/wp-content/uploads/2025/08/Jurassic-World-Rebirth-2025.jpg",
                title: "جان ویک: بخش 3 - پارابلوم",
                genre: "اکشن / هیجان انگیز",
                year: "2019",
                duration: "2h 11min",
                quality: "4K"
            },
            {
                image: "https://api2.zoomg.ir/media/2018-3-8b9e4f3f-d243-4012-8656-ebc12187b0cb-66cc7d012b5676090d00b39a",
                title: "بتمن علیه سوپرمن",
                genre: "اکشن / ابرقهرمانی",
                year: "2016",
                duration: "2h 31min",
                quality: "4K"
            },
            {
                image: "https://salamcinama.ir/api/filedb/a3c2c612/%D9%81%D8%B5%D9%84-%D8%AF%D9%88%D9%85-%D9%88%D9%86%D8%B2%D8%AF%DB%8C.jpg?w=any&q=75",
                title: "اعلان قرمز",
                genre: "اکشن / کمدی",
                year: "2021",
                duration: "1h 58min",
                quality: "4K"
            },
            {
                image: "https://gamotionart.com/wp-content/uploads/2024/11/arcane-season-2-changes-too-many-things-1024x576.jpg",
                title: "بتمن شوالیه تاریکی",
                genre: "اکشن / رازالود",
                year: "2008",
                duration: "2h 32min",
                quality: "4K"
            },
            {
                image: "https://gamefa.com/wp-content/uploads/2021/11/Wonder-Woman-Gal-Gadot-with-shield.jpg.webp",
                title: "زن شگفت انگیز",
                genre: "اکشن / ماجراجویی",
                year: "2017",
                duration: "2h 21min",
                quality: "4K"
            },
            {
                image: "https://static.namava.ir/Content/Upload/Images/f329df9c-a7e0-4bff-be0f-383b702afd5c.jpg?anchor=middlecenter&crop=auto&scale=both&w=1280&h=600",
                title: "اسکویید گیم",
                genre: "هیجان انگیز / جنایی",
                year: "2021",
                duration: "قسمت ۴۵-۶۰ دقیقه",
                quality: "4K"
            }
        ];

        // عناصر DOM
        const mainBanner = document.getElementById('main-banner');
        const bannerImg = mainBanner.querySelector('img');
        const cardContent = mainBanner.querySelector('.card-content');
        const thumbs = document.querySelectorAll('.thumb');
        let currentIndex = 0;
        let autoPlayInterval;

        // تابع برای تغییر بنر
        function changeBanner(index) {
            const movie = moviesData[index];
            
            // تغییر عکس بنر
            bannerImg.src = movie.image;
            
            // تغییر اطلاعات بنر
            const genreSpan = cardContent.querySelector('.genre span');
            const yearSpan = cardContent.querySelector('.year span');
            const durationSpan = cardContent.querySelector('.duration span');
            const qualityDiv = cardContent.querySelector('.quality');
            const titleHeading = cardContent.querySelector('.card-title');
            
            genreSpan.textContent = movie.genre;
            yearSpan.textContent = movie.year;
            durationSpan.textContent = movie.duration;
            qualityDiv.textContent = movie.quality;
            titleHeading.textContent = movie.title;
            
            // به‌روزرسانی وضعیت فعال thumbnail
            thumbs.forEach(thumb => thumb.classList.remove('active'));
            thumbs[index].classList.add('active');
            
            currentIndex = index;
        }

        // کلیک روی thumbnail ها
        thumbs.forEach(thumb => {
            thumb.addEventListener('click', () => {
                // توقف اسلایدشو هنگام کلیک کاربر
                clearInterval(autoPlayInterval);
                
                const index = parseInt(thumb.dataset.index);
                changeBanner(index);
                
                // راه اندازی مجدد اسلایدشو پس از 10 ثانیه
                startAutoPlay();
            });
        });

        // تابع برای اسلاید بعدی
        function nextSlide() {
            let nextIndex = (currentIndex + 1) % moviesData.length;
            changeBanner(nextIndex);
        }

        // شروع اسلایدشو اتوماتیک
        function startAutoPlay() {
            clearInterval(autoPlayInterval);
            autoPlayInterval = setInterval(nextSlide, 5000); // تغییر هر 5 ثانیه
        }

        // شروع اسلایدشو هنگام لود صفحه
        document.addEventListener('DOMContentLoaded', () => {
            startAutoPlay();
        });
		
		
		function menu_bars(){
		     const navbar = document.querySelector(".dropdown");
			 navbar.style.transform = "translateY(0px)";
		   }
		   function cancel(){
		     const navbar = document.querySelector(".dropdown");
			 navbar.style.transform = "translateY(-500px)";
		   }
		   
		   ScrollReveal().reveal(".navbar-link", {
		     origin: "bottom",
			 distance: "50px",
			 duration: 1000,
			 interval: 600,
			 });
		   ScrollReveal().reveal(".scroll-link a", {
			 origin: "top",
			 distance: "50px",
			 duration: 1000,
			 interval: 300,
			 });
		   ScrollReveal().reveal(".left", {
			 origin: "left",
			 distance: "60px",
			 duration: 1000,
			 interval: 100,
			 });
		   ScrollReveal().reveal(".right", {
			 origin: "right",
			 distance: "60px",
			 duration: 1000,
			 interval: 100,
			 });
		   ScrollReveal().reveal(".logo", {
			 scale: 0.85,
			 duration: 1000,
			 delay: 100,
			 });
			 
			 document.querySelectorAll('[class*="delay-"]').forEach((el) => {
			     const delay = Number(el.className.match(/delay-(\d)/)?.[1] || 0) * 200;
				 el.style.setProperty("--sr-delay", delay + "ms");
			 });
			 
			 
// اضافه کردن کلاس active به تامبنیل انتخاب شده
thumbs.forEach(thumb => {
  thumb.addEventListener('click', function() {
    // حذف کلاس active از همه تامبنیل‌ها
    thumbs.forEach(t => t.classList.remove('active'));
    
    // اضافه کردن کلاس active به تامبنیل انتخاب شده
    this.classList.add('active');
    
    // تغییر بنر اصلی
    const index = parseInt(this.dataset.index);
    changeBanner(index);
  });
});

// راه‌اندازی اسلایدر خودکار برای تامبنیل‌ها
function startThumbnailsAutoScroll() {
  const container = document.querySelector('.thumbnails-container');
  let scrollAmount = 0;
  const scrollSpeed = 1;
  
  setInterval(() => {
    scrollAmount += scrollSpeed;
    if (scrollAmount >= container.scrollWidth - container.clientWidth) {
      scrollAmount = 0;
    }
    container.parentElement.scrollLeft = scrollAmount;
  }, 50);
}
</script>
<script>
document.addEventListener("DOMContentLoaded", () => {
  const banner = document.getElementById("main-banner").querySelector("img");
  const thumbs = document.querySelectorAll(".thumb");
  let currentIndex = 0;
  let interval;

  function showSlide(index) {
    // تغییر عکس اصلی
    const img = thumbs[index].querySelector("img").src;
    banner.src = img;

    // حذف active از همه
    thumbs.forEach(t => t.classList.remove("active"));

    // اضافه کردن active به کارت فعلی
    thumbs[index].classList.add("active");

    currentIndex = index;
  }

  // وقتی روی تامبنیل کلیک شد
  thumbs.forEach((thumb, index) => {
    thumb.addEventListener("click", () => {
      clearInterval(interval); // اگر کاربر کلیک کرد، تایمر reset شه
      showSlide(index);
      autoSlide(); // دوباره تایمر شروع شه
    });
  });

  // اسلاید خودکار هر ۵ ثانیه
  function autoSlide() {
    interval = setInterval(() => {
      let nextIndex = (currentIndex + 1) % thumbs.length;
      showSlide(nextIndex);
    }, 5000);
  }

  // شروع اولیه
  showSlide(0);
  autoSlide();
});
</script>
<script>
  const slider = document.querySelector('.thumbnails');
  let isDown = false;
  let startX;
  let scrollLeft;

  slider.addEventListener('mousedown', (e) => {
    isDown = true;
    slider.classList.add('active');
    startX = e.pageX - slider.offsetLeft;
    scrollLeft = slider.scrollLeft;
  });
  slider.addEventListener('mouseleave', () => {
    isDown = false;
    slider.classList.remove('active');
  });
  slider.addEventListener('mouseup', () => {
    isDown = false;
    slider.classList.remove('active');
  });
  slider.addEventListener('mousemove', (e) => {
    if(!isDown) return;
    e.preventDefault();
    const x = e.pageX - slider.offsetLeft;
    const walk = (x - startX) * 2; // سرعت حرکت
    slider.scrollLeft = scrollLeft - walk;
  });
</script>
<script>
document.addEventListener("DOMContentLoaded", () => {
  const banner = document.getElementById("main-banner").querySelector("img");
  const thumbsContainer = document.querySelector(".thumbnails-container");
  const thumbs = document.querySelectorAll(".thumb");
  let currentIndex = 0;
  let interval;

  function showSlide(index) {
    const selectedThumb = thumbsContainer.querySelector(`.thumb[data-index="${index}"]`);
    if (!selectedThumb) return;

    // تغییر عکس اصلی
    const img = selectedThumb.querySelector("img").src;
    banner.src = img;

    // حذف active از همه
    thumbsContainer.querySelectorAll(".thumb").forEach(t => t.classList.remove("active"));

    // اضافه کردن active
    selectedThumb.classList.add("active");

    // جابه‌جا کردن کارت انتخاب شده به اول لیست
    thumbsContainer.prepend(selectedThumb);

    currentIndex = index;
  }

  // کلیک روی کارت‌ها
  thumbsContainer.querySelectorAll(".thumb").forEach((thumb) => {
    thumb.addEventListener("click", () => {
      clearInterval(interval);
      const index = parseInt(thumb.getAttribute("data-index"));
      showSlide(index);
      autoSlide();
    });
  });

  // اسلاید خودکار
  function autoSlide() {
    interval = setInterval(() => {
      let nextIndex = (currentIndex + 1) % thumbs.length;
      showSlide(nextIndex);
    }, 5000);
  }

  // شروع
  showSlide(0);
  autoSlide();
});
</script>
<script>
document.querySelectorAll('.thumbnails img').forEach(img => {
  img.ondragstart = () => false;
});

// existing slider vars
const slider = document.querySelector('.thumbnails');
let isDown = false;
let startX, scrollLeft;

slider.addEventListener('mousedown', (e) => {
  isDown = true;
  slider.classList.add('active');
  startX = e.pageX - slider.offsetLeft;
  scrollLeft = slider.scrollLeft;
});
slider.addEventListener('mouseup', () => { isDown = false; slider.classList.remove('active'); });
slider.addEventListener('mouseleave', () => { isDown = false; slider.classList.remove('active'); });
slider.addEventListener('mousemove', (e) => {
  if(!isDown) return;
  e.preventDefault();
  const x = e.pageX - slider.offsetLeft;
  const walk = (x - startX) * 2;
  slider.scrollLeft = scrollLeft - walk;
});

// touch events
slider.addEventListener('touchstart', (e) => {
  isDown = true;
  slider.classList.add('active');
  startX = e.touches[0].pageX - slider.offsetLeft;
  scrollLeft = slider.scrollLeft;
}, {passive:false});
slider.addEventListener('touchend', () => { isDown = false; slider.classList.remove('active'); });
slider.addEventListener('touchmove', (e) => {
  if(!isDown) return;
  e.preventDefault();
  const x = e.touches[0].pageX - slider.offsetLeft;
  const walk = (x - startX) * 2;
  slider.scrollLeft = scrollLeft - walk;
}, {passive:false});


thumbs.forEach(t => t.classList.remove("active"));
thumbs[index].classList.add("active");
</script>
<script>
banner.style.opacity = 0; // محو بشه
setTimeout(() => {
  banner.src = newSrc;    // عکس جدید
  banner.style.opacity = 1; // ظاهر بشه
}, 300);
</script>
</body>
</html>
