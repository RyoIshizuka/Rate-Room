<template>
            <div class="grid-wrap">
            <ul>
                <li>
                    <a href="#">
                        <picture class="list-ikon">
                            <source srcset="@/assets/images/cat-food.webp" type="image/webp">
                            <img src="@/assets/images/cat-food.png">
                        </picture>
                        <p class="list-name">ご飯</p>
                    </a>

                </li>
                <li>
                    <a href="#">
                        <picture class="list-ikon">
                            <source srcset="@/assets/images/cat-weight.webp" type="image/webp">
                            <img src="@/assets/images/cat-weight.png">
                        </picture>
                        <p class="list-name">体重</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <picture class="list-ikon">
                            <source srcset="@/assets/images/cat-toilet.webp" type="image/webp">
                            <img src="@/assets/images/cat-toilet.png">
                        </picture>
                        <p class="list-name">トイレの回数</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <picture class="list-ikon">
                            <source srcset="@/assets/images/grooming.webp" type="image/webp">
                            <img src="@/assets/images/grooming.png">
                        </picture>
                        <img src="" alt="">
                        <p class="list-name">ブラッシング</p>
                    </a>
                </li>
            </ul>
        </div>
</template>

<style lang="scss" scoped>
.grid-wrap{
    max-width: 800px;
    width: 100%;
    margin: 0 auto;
    padding: 0 1em;
    ul{
        display: grid;
        grid-template-columns: repeat(auto-fill,300px);
        justify-content: space-around;
        grid-template-rows: repeat(2,350px);
        grid-row-gap:3em;
        li{
            list-style: none;
            border: solid 1px;
            background: rgba( 255, 255, 255, 0.25 );
            backdrop-filter: blur( 1px );
            -webkit-backdrop-filter: blur( 1px );
            border-radius: 10px;
            border: 2px solid rgba( 255, 255, 255, 0.18 );
            position: relative;
            .list-name{
                background: rgba( 255, 255, 255, 0 );
                backdrop-filter: blur( 20px );
                -webkit-backdrop-filter: blur( 20px );
                border-radius: 10px;
                border: 1px solid rgba( 255, 255, 255, 0.18 );
            }
            a{
                text-decoration: none;
                display: block;
                text-align: center;
                position: absolute;
                bottom: 30px;
                right: 85px;
                font-size: 15px;
                .list-ikon{
                    display: block;
                    line-height: 155px;
                    img{
                        max-width: 90px;
                        width: 100%;
                    }
                }
                p{
                    display: inline-block;
                    color: #000;
                    padding: 8px 45px 7px 45px;
                }
            }
        }
        li:nth-child(3){
            a{
                right: 55px;
            }
        }
        li:nth-child(4){
            a{
                right: 55px;
            }
        }
    }
}
</style>