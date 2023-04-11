<template>
    <aside class="sidebar">
        <div v-if="$store.state.account.name ==''" class="userPanel">
            <div class="userPanel-title">
                User Panel
            </div>
            <div class="userPanel-info">
                Please <a href="">log In</a> to use the entire website.
            </div>
            <div class="userPanel-enter">
                <div class="userPanel-button">
                    <a class="button open-modal" @click="$store.dispatch('setModalType', 'sign-in')">Sign In</a> 
                </div>
                <span class="or">or</span>
                <div class="userPanel-button">
                    <a href="#" class="button open-modal" @click="$store.dispatch('setModalType', 'sign-up')">Sign Up</a>
                </div>
                <a href="" class="download">
                    <p>Download</p>
                    <span>File Size 2Gb</span>
                </a>
            </div>
        </div>
        <div v-else class="userPanel">
            <div class="userPanel-title">
                User Panel
            </div>
            <div class="userPanel-name">
                Welcome, <span>{{$store.state.account.name}}</span>
            </div>
            <div class="coin flex-s-c">
                <div class="coin-block">
                    <i class="icon-coin coin-f"></i>
                    Coins
                    <span>1500</span>
                </div>
                <div class="coin-block">
                    Server:
                    <span>Andro</span>
                    <i class="icon-coin coin-s"></i>
                </div>
            </div>
            <ul class="cp-menu">
                <li><a @click="$router.push('/item-shop')" class="button">Itemshop</a></li>
                <li><a class="button">Donate</a></li>
                <li><a class="button">Account</a></li>
                <li><a class="button">Characters</a></li>
                <li><a class="button">Delete Account</a></li>
                <li><a class="button">My Tickets</a></li>
                <li><a @click="$store.dispatch('account/resetState')" class="button">logout</a></li>
            </ul>
        </div>

        <div class="statistics flex-c-c">
            <div class="statisticsBlock">
                <div class="statisticsBlock-title">
                    Game Statistics
                </div>
                <div class="statisticsBlock-info">
                    Players Online <span>1.500</span>
                </div>
                <div class="statisticsBlock-info">
                    Players Online 24h <span>2.480</span>
                </div>
                <div class="statisticsBlock-info">
                    Accounts <span>3.000</span>
                </div>
                <div class="statisticsBlock-info">
                    Characters <span>1.500</span>
                </div>
            </div>
        </div><!--statistics-->

        <div class="banner flex-c-c">
            <div class="bannerBlock">
                <a href="#">
                    <img src="@/assets/images/prem-bg.jpg" alt="">
                </a>
            </div>
        </div><!--banner-->
        <div class="king">
            <div class="king-title">
                King Of Kings
            </div>
            <div class="king-block">
                <img class="king-block_img" src="@/assets/images/hero.png" alt="">
                <div class="king-block_info">
                    <div class="king-block_info-name">
                        Vex
                    </div>
                    <div class="king-block_info-guild flex-c-c">
                        <span class="color-yellow">Sura</span>
                        <span class="color-red">Shinsoo</span>
                    </div>
                </div>
                <div class="kills king-block_stat">
                    <p>Kills</p>
                    <span>100.000</span>
                </div>
                <div class="playtime king-block_stat">
                    <p>Playtime</p>
                    <span>3.5 Years</span>
                </div>
                <div class="wars king-block_stat">
                    <p>Wars</p>
                    <span>97.450</span>
                </div>
            </div>
            <div class="king-more">
                <a href="">All Hail To The King!</a>
            </div>
        </div><!--king-->
    </aside>
</template>
<script></script>