<script>
export default{
  name: "NavComp",
}

</script>

<template>
<nav class="w-75 mx-auto d-flex justify-content-between align-items-center p-3">
    <div id="logo">
        <img class="d-block" src="/images/logo.png" alt="">
    </div>
    <div id="list">
        <ul>
            <li>
                <a href="/">home</a>
            </li>
            <li>
                <a href="/">pages</a>
            </li>
            <li>
                <a href="/">program</a>
            </li>
            <li>
                <a href="/">tickets</a>
            </li>
            <li>
                <a href="/">speakers</a>
            </li>
            <li>
                <a href="/">papers</a>
            </li>
            <li>
                <a href="/">blog</a>
            </li>
            <li>
                <a href="/">shortcodes</a>
            </li>
            
            <i class="fa-solid fa-magnifying-glass"></i>
        </ul>
    </div>
</nav>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;
#list{
    display: flex;
    align-items: center;
    ul{
        display: flex;
        li{
            list-style-type: none;
            margin: 0 15px;
            &:hover{      
                    border-bottom: 2px solid $Scarlet;
                    a{
                        color: $Scarlet;
                    }
                    
                }
               
            a{
                text-decoration: none;
                text-transform: uppercase;
                font-weight: bold;
                font-size: 12px;
                color: $Natural-Gray;
                
            }
            
        }
        i{
                font-family: "Font Awesome 6 Free";
                color: $Natural-Gray;
                border-left: 2px solid $Natural-Gray;
                padding-left: 20px;
            }
    }
}

</style>