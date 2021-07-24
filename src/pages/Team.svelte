
<script>
    import {fade , slide , scale , fly} from "svelte/transition";
    export let y;
    </script>
<style>
    /**********************************/
/***** Layout & Section Title *****/
/**********************************/
.container {
    width: 100%;
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
}

@media (min-width: 576px) {
    .container {
        max-width: 540px;
    }
}

@media (min-width: 768px) {
    .container {
        max-width: 720px;
    }
}

@media (min-width: 992px) {
    .container {
        max-width: 960px;
    }
}

@media (min-width: 1200px) {
    .container {
        max-width: 1140px;
    }
}

.row {
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    margin-right: -15px;
    margin-left: -15px;
}

.column {
    position: relative;
    width: 100%;
    padding-right: 15px;
    padding-left: 15px;
    -ms-flex: 0 0 100%;
    flex: 0 0 100%;
    max-width: 100%;
}

@media (min-width: 576px) {
    .column {
        -ms-flex: 0 0 50%;
        flex: 0 0 50%;
        max-width: 50%;
    }
}

@media (min-width: 768px) {
    .column {
        -ms-flex: 0 0 33.333333%;
        flex: 0 0 33.333333%;
        max-width: 33.333333%;
    }
}

@media (min-width: 992px) {
    .column {
        -ms-flex: 0 0 25%;
        flex: 0 0 25%;
        max-width: 25%;
    }
}

.section-title {
    width: 100%;
    text-align: center;
    padding: 45px 0 30px 0;
}

.section-title::after {
    position: absolute;
    content: "";
    width: 50px;
    height: 5px;
    left: calc(50% - 25px);
    background: #353535;
}

.section-title h1 {
    color: #353535;
    font-size: 50px;
    margin-bottom: 5px;
}

@media(max-width: 767.98px) {
    .section-title h1 {
        font-size: 40px;
    }
}

@media(max-width: 567.98px) {
    .section-title h1 {
        font-size: 30px;
    }
}



/**********************************/
/********* Team #3 Style **********/
/**********************************/

.team-3 {
    margin-bottom: 30px;
}

.team-3 .team-img {
    position: relative;
    font-size: 0;
    clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
    -webkit-clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
}

.team-3 .team-img img {
    width: 100%;
    height: auto;
}

.team-3 .team-social {
    position: absolute;
    width: 100%;
    height: 100%;
    padding: 20px;
    top: 0;
    left: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    background: rgba(255, 255, 255, .5);
    transition: all .3s;
    font-size: 0;
    z-index: 1;
    opacity: 0;
}

.team-3:hover .team-social {
    opacity: 1;
}

.team-3 .team-social a {
    display: inline-block;
    width: 40px;
    height: 40px;
    margin-right: 5px;
    padding: 11px 0 10px 0;
    font-size: 16px;
    font-weight: 300;
    line-height: 16px;
    text-align: center;
    color: #ffffff;
    transition: all .3s;
    margin-top: 50px;
    clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
    -webkit-clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
}

.team-3 .team-social a.social-tw {
    background: #00acee;
}

.team-3 .team-social a.social-fb {
    background: #3b5998;
}

.team-3 .team-social a.social-li {
    background: #0e76a8;
}

.team-3 .team-social a.social-in {
    background: #3f729b;
}

.team-3 .team-social a.social-yt {
    background: #c4302b;
}

.team-3 .team-social a:last-child {
    margin-right: 0;
}

.team-3:hover .team-social a {
    margin-top: 0;
}

.team-3 .team-social a:hover {
    color: #222222;
    background: #ffffff;
}

.team-3 .team-content {
    padding: 70px 20px 20px 20px;
    margin-top: -50px;
    text-align: center;
    background: #f3f4fa;
    transition: all .5s;
}

.team-3:hover .team-content {
    background: #222222;
}

.team-3:hover .team-content h2,
.team-3:hover .team-content h3,
.team-3:hover .team-content h4,
.team-3:hover .team-content p {
    color: #ffffff;
}

.team-3 .team-content h2 {
    font-size: 25px;
    font-weight: 400;
    letter-spacing: 2px;
}

.team-3 .team-content h3 {
    font-size: 16px;
    font-weight: 300;
}

.team-3 .team-content h4 {
    font-size: 16px;
    font-weight: 300;
    font-style: italic;
    letter-spacing: 1px;
    margin-bottom: 0;
}

.team-3 .team-content p {
    font-size: 16px;
    font-weight: 400;
    line-height: 22px;
}
.team-image-cust{
    box-shadow: 0 0 10px gray;
    border: 1px solid gray;
}

</style>


<section class="container" >
    {#if y>= 1600}
        
    
    <div transition:slide={{delay:50,duration:200}} class="section-title" >
        <h1>اعضای تیم اینولینکس</h1>
    </div>
    {/if}
    <div class="row">
        {#if y> 1750}
        <div class="column" transition:scale={{opacity:0.1,delay:600,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/1.jpeg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>مسعود آقایی</h2>
                    <h3>Product Owner</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:450,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/12.jpg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>محمدخلیفه</h2>
                    <h3>CTO &nbsp; Management</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:300,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/2.jpeg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>محمد یدالله ‍‍</h2>
                    <h3>Junior UI & UX</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:150,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/4.jpeg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>مجتبی اکبری</h2>
                    <h3>Junior Backend</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        {/if}
        {#if y> 2200}        
        <div class="column" transition:scale={{opacity:0.1,delay:150,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/13.jpg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>محسنی</h2>
                    <h3>Sunior UI & UX</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:300,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/517.jpg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>علی فلاح</h2>
                    <h3>Sunior Frontend & Backend</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:450,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/6.jpeg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>سیدعباس موسوی اصل</h2>
                    <h3>Junior Frontend</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        <div class="column" transition:scale={{opacity:0.1,delay:600,duration:300}}>
            <div class="team-3">
                <div class="team-img">
                    <img class="team-image-cust" src="image/22.jpeg" alt="Team Image">
                    <div class="team-social">
                        <a class="social-tw" href=""><i class="fab fa-twitter"></i></a>
                        <a class="social-fb" href=""><i class="fab fa-facebook-f"></i></a>
                        <a class="social-li" href=""><i class="fab fa-linkedin-in"></i></a>
                        <a class="social-in" href=""><i class="fab fa-instagram"></i></a>
                        <a class="social-yt" href=""><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="team-content">
                    <h2>شهید صدرزاده</h2>
                    <h3>Martyr</h3>
                    <p>لورم یک ساختار متن ساختگی برای سایت و بلاگ است</p>
                    <h4>info@info.com</h4>
                </div>
            </div>
        </div>
        {/if}
    </div> 
</section>