<script>
    import {onMount} from "svelte";
    import {fade , slide , scale} from "svelte/transition";
    import { Router, Link, Route } from "svelte-routing";
    import about from "./about.svelte";
    export let url = "";
    import Team from "./Team.svelte";
    /*let team = {};
     onMount(
		async() => {
			const res = await fetch('data.JSON')
			team = await res.json()
		}
	);
    */
</script>
<style>
    @import "public/global.css";
</style>
<section class="container-fluid text-header-custom pt-5 pb-5 header-image w-100 h-auto mt-0" transition:scale>
    <h1 class="mt-4">به اینولینکس خوش آمدید</h1>
    <p style="font-size: 20px;" class="col-md-10 offset-md-1 mt-5">
        اگر شما یک طراح هستین و یا با طراحی های گرافیکی سروکار دارید به متن های برخورده اید که با نام لورم ایپسوم شناخته می‌شوند. لورم ایپسوم یا طرح‌نما به انگلیسی متنی ساختگی و بدون معنی است که برای امتحان فونت و یا پر کردن فضا در یک طراحی گرافیکی و یا صنعت چاپ استفاده میشود..
    </p>
    <Router url="{url}">
        <Link to="about">
            <button class="my-btn text-center btn col-xs-12 col-md-2 btn-lg mt-5 mb-xs-6">بیشتر بدانید</button>
        </Link>
        <Route path="about" component="{about}" />
    </Router>
</section>
<br><hr class="col-10 offset-1"><br><br><br>
<section class="container-fluid " style="direction: rtl;">
    <article class="row">
        <h1 class="col-12 text-center" style="direction: rtl;">
            <i class="fas fa-book-reader"></i>&nbsp;<span>
                رخدادهای روزانه را در اینجا دنبال کنید 
            </span>
        </h1>
        <div class="col-12 col-md-4 selection">
            <div class="card text-center p-4" style="direction: rtl;">
                <div class="card-img ">
                    <i style="font-size: 150px;" class="my-icon fab fa-node fa-lg rounded-circle p-4"></i>
                </div>
                <div class="card-body">
                    <h4 class="card-title" >دوره آموزشی Node.js</h4>
                    <p class="card-text"> دوره آموزشی زبان برنامه نویسی Node.js  بریا افراد مبتدی در حال انتشار است لطفا تا زمان انتشار منتظر بمانید</p>
                    <a href="#" class="btn btn-info">بیشتر بدانید</a>
                  </div>
            </div>
        </div>
        <div class="col-12 col-md-4 selection">
            <div class="card text-center p-4" style="direction: rtl;">
                <div class="card-img ">
                    <i style="font-size: 150px;" class="my-icon fab fa-python fa-lg rounded-circle p-4"></i>
                </div>
                <div class="card-body">
                    <h4 class="card-title" >دوره آموزشی Python3</h4>
                    <p class="card-text"> دوره آموزشی زبان برنامه نویسی Python3  بریا افراد مبتدی در حال انتشار است لطفا تا زمان انتشار منتظر بمانید</p>
                    <a href="#" class="btn btn-info">بیشتر بدانید</a>
                  </div>
            </div>
        </div>
        <div class="col-12 col-md-4 selection">
            <div class="card text-center p-4" style="direction: rtl;">
                <div class="card-img ">
                    <i style="font-size: 150px;" class="my-icon fab fa-linux fa-lg rounded-circle p-4"></i>
                </div>
                <div class="card-body">
                    <h4 class="card-title" >دوره آموزشی DataBase</h4>
                    <p class="card-text"> دوره آموزشی زبان برنامه نویسی DataBase بریا افراد مبتدی در حال انتشار است لطفا تا زمان انتشار منتظر بمانید</p>
                    <a href="#" class="btn btn-info">بیشتر بدانید</a>
                  </div>
            </div>
        </div>
        
    </article>
</section>
<br><hr class="col-10 offset-1"><br><br><br>
<section class="container-fluid">
    <article class="row cust-raw">
        <div class="col-12 col-md-5 ml-md-5 p-0" style="overflow: hidden;border-radius: 15px;">
            <img src="20.jpg" class="picture-custom w-100" alt="">
        </div>
        <div class="col-12 col-md-6 bg-light" style="border-radius: 0 40px 10px 0;">
            <div class="container-fluid text-center ">
                <div class="row">
                    <h3 class="col-12 mt-4" style="font-weight: bold;">
                         مهارت جهت کارآفرینی با پکیج های اینولینکس
                    </h3>
                    <hr class="col-10 offset-1">
                    <p class="col-12" style="text-align: justify;direction: rtl;">
                        لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد، کتابهای زیادی در شصت و سه درصد گذشته حال و آینده، شناخت فراوان جامعه و متخصصان را می طلبد، تا با نرم افزارها شناخت بیشتری را برای طراحان رایانه ای علی الخصوص طراحان خلاقی، و فرهنگ پیشرو در زبان فارسی ایجاد کرد، در این صورت می توان امید داشت که تمام و دشواری موجود در ارائه راهکارها، و شرایط سخت تایپ به پایان رسد و زمان مورد نیاز شامل حروفچینی دستاوردهای اصلی،.
                    </p>
                    <a style="" href="#" class="btn btn-success col-12 col-md-4 text-center ">بیشتر بدانید</a>
                </div>
            </div>
        </div>
    </article><br><br><br>
    <article class="row cust-raw justify-content-md-center" >
        <div class="col-12 col-md-6 bg-light " style="border-radius: 40px 0 0 10px;">
            <div class="container-fluid text-center ">
                <div class="row">
                    <h3 class="col-12 mt-4" style="font-weight: bold;">
                         یکی از راه های موفقیت کار تیمی است
                    </h3>
                    <hr class="col-10 offset-1">
                    <p class="col-12" style="text-align: justify;direction: rtl;">
                        لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد، کتابهای زیادی در شصت و سه درصد گذشته حال و آینده، شناخت فراوان جامعه و متخصصان را می طلبد، تا با نرم افزارها شناخت بیشتری را برای طراحان رایانه ای علی الخصوص طراحان خلاقی، و فرهنگ پیشرو در زبان فارسی ایجاد کرد، در این صورت می توان امید داشت که تمام و دشواری موجود در ارائه راهکارها، و شرایط سخت تایپ به پایان رسد و زمان مورد نیاز شامل حروفچینی دستاوردهای اصلی،.
                    </p>
                    <a style="" href="#" class="btn btn-success col-12 mb-4 col-md-4 text-center ">بیشتر بدانید</a>
                </div>
            </div>
        </div>
        <div class="col-12 col-md-5 order-md-last order-first p-0" style="overflow: hidden;border-radius: 15px;">
            <img src="download.jpeg" class="picture-custom w-100" alt="">
        </div>
    </article><br>
</section>
<hr class="col-10 offset-1"><br>
<Team />

