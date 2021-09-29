<template>
    <div class="padding">
        <div class="col-left">
            <p>DC COMICS</p>
            <ul>
                <li><a href="">wq</a></li>
                <li><a href="">wq</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
            </ul>
            <p>SHOP</p>
            <ul>
                <li><a href=""></a></li>
                <li>a</li>
            </ul>
        </div>
        <div class="col-center">
            <p>DC COMICS</p>
            <ul>
                <li><a href="">wq</a></li>
                <li><a href="">wq</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
            </ul>
            
        </div>
        <div class="col-right">
            <p>DC COMICS</p>
            <ul>
                <li><a href="">wq</a></li>
                <li><a href="">wq</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
                <li><a href="">qw</a></li>
            </ul>
        </div>
    </div>
</template>
<script>
    export default{
            name:"FooterTop"
    }
</script>
<style lang="scss" scoped>
        div{
            display: flex;
            flex-direction: row;
            padding-top: 50px;
            background-image: url(../img/footer-bg.jpg);
            background-size: cover;

            .col-left, .col-right, .col-center{
                display: flex;
                flex-direction: column;
            }
            p{
                color: white;
                font-size: 15px;
            }
            ul{
                padding-right: 30px;
                list-style: none;
            }
            a{
                text-decoration: none;
                color: #69687a;
            }
            div{
                margin-right:30px ;
            }
        }
</style>
