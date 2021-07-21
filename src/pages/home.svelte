<script>
    import {fade , slide , scale} from "svelte/transition";
    import { Router, Link, Route } from "svelte-routing";
    import about from "./about.svelte";
    export let url = "";
</script>
<style>
    @import "public/global.css";
</style>
<div class="container-fluid text-header-custom pt-5 pb-5 header-image w-100 h-auto mt-0" transition:scale>
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
</div>
<br><hr class="col-10 offset-1"><br><br><br>
<div class="container-fluid">
    <div class="row">
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
        
    </div>
</div>