
<script setup>
    import page1 from "/src/views/page1.vue"
    import{ref} from "vue";
</script>

<template>
    <link rel="icon" href="/src/assets/tachi.png">
    <link rel="stylesheet" href="base.css">
    <header>
        <ul class="header">
            <a href="">
                <img src="/src/assets/tachi.png" alt="">
                <li class="title">日文漢字對答案</li>
            </a>
            <a target="_blank" href="https://dictionary.goo.ne.jp/" class="Go">
                <img src="/src/assets/Go.png" alt="">
            </a>
            <a target="_blank" href="https://dictionary.goo.ne.jp/" class="middle">
                Go 辞書
            </a>
            <a href="" class="login">登錄會員</a>
        </ul>
    </header>
    <main>
        <ul class="answer">
            <page1></page1>
            <span class="answer-switch">
                <svg width="24px" height="24px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M6 12H18M6 12L11 7M6 12L11 17" stroke="#000000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
                <a href="">1 2 3 4 5</a>
                <svg width="24px" height="24px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M6 12H18M18 12L13 7M18 12L13 17" stroke="#000000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>

            </span>
        </ul>
    </main>
    <footer>

    </footer>
</template>

<style scoped>
    /* header */
    header {
        position: relative;
        width: 100%;
        background-color: rgb(255,126,126);
    }
    header img{
        width: 80px;
        margin-left: 5vh;
    }
    header .title{
        font-size: 32px;
        position: absolute;
        height: 40px;
        display: flex;
        top: 24px;
        left: 130px;
        letter-spacing: 4px;
    }
    header .middle{
        font-size: 24px;
        color: rgb(138, 0, 0);
        position: absolute;
        right: 180px;
        top: 32px;
    }
    header .Go img {
        position: absolute;
        right: 265px;
        top: 18px;
        width: 60px;
    }
    header .middle:hover {
        cursor: pointer;
        box-shadow: 0 1px;
    }
    header ul .login {
        position: absolute;
        right: 24px;
        font-size: 20px;
        top: 35px;
        letter-spacing: 2px;
    }
    header ul .login:hover {
        box-shadow: 0 1px;
        padding-bottom: 1px;
    }

    /* main */
    main {
        position: relative;
        width: 100%;
        height: 1500px;
        background: linear-gradient(rgb(255,126,126), rgba(255, 182, 200, 0.62), rgba(255, 196, 196, 0.62));
    }
    main .answer {  /* 調整大小 */
        margin-left: 2.5%;
        position: relative;
        width: 95%;
        height: 1150px;
        background-color: rgba(rgb(255, 255, 255), rgb(244, 246, 244), rgb(255, 255, 255), 1);
        border: 1px solid black;
        border-radius: 12px;
        padding: 4px;
        display: flex;
        justify-content: center;
    }
    main .answer-switch {
        display: flex;
        justify-content: center;
        align-items: end;
    }
    main .answer-switch a {
        margin: 0 10px 2px 10px;
    }

    /* 響應 */
    @media only screen and (max-width: 730px){
        header .title {
            left: 90px;
        }
        header img {
            margin-left: 3px;
        }
        header ul .login {
            top: 50px;
            right: 48px;
        }
        header .middle{
        top: 18px;
        right: 50px;
        }
        header .Go img {
        top: 2px;
        right: 140px;
        }
    }
    
</style>