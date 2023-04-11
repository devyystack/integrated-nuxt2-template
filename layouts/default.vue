<template>
    <div class="wrapper">
        <AppHeader/>
        <div class="topBlock">
			<div class="highlight">
				<div class="highlight-3"></div>
				<div class="highlight-4"></div>
			</div>
			<div class="circle circle1"></div>
			<div class="circle circle2"></div>
			<div class="logo">
				<a href="/"><img src="@/assets/images/logo.png" alt="Logo"></a>
			</div>
		</div>
        <main class="main flex-s">
			<div class="main-content">
				<div class="upper">
					<div class="upperBlock flex-c-c">
						<a href="" class="upper-block flex-c">
							<div class="upper-block_img">
								<img src="@/assets/images/icons/icon-book.png" alt="">
							</div>
							<div class="upper-block_info">
								<p>Presentation</p>
								<span>See the content of our game</span>
							</div>
						</a>
						<a href="" class="upper-block flex-c">
							<div class="upper-block_img">
								<img src="@/assets/images/icons/icon-discord.png" alt="">
							</div>
							<div class="upper-block_info">
								<p>Discrod</p>
								<span>Join our community</span>
							</div>
						</a>
						<a href="" class="upper-block flex-c">
							<div class="upper-block_img">
								<img src="@/assets/images/icons/icon-vote.png" alt="">
							</div>
							<div class="upper-block_info">
								<p>Donate</p>
								<span>Vote for us and eam rewards</span>
							</div>
						</a>
					</div>
				</div>
				<Nuxt/>
			</div>
			<AppSideBar/>
            
            
        </main>
		
        <Modal v-show="$store.state.isModal"/>
        <footer class="footer">
			<div class="footer-container flex">
				<div class="footer-info">
					<a href="/"><img src="@/assets/images/logo-footer.png" alt=""></a>
					<div class="copyright">
						Copyright @ 2022 grandoespada.com. All rights reserved.<br>
						All other trademarks are the property of their respective owners.
					</div>
				</div>
				<div class="footerMenu">
					<span>Resorces</span>
					<ul>
						<li><a href="">Terms & Conditions</a></li>
						<li><a href="">Privacy</a></li>
						<li><a href="">Legal</a></li>
						<li><a href="">Cookie Preferences</a></li>
					</ul>
				</div>
				<div class="footerMenu">
					<span>Support</span>
					<ul>
						<li><a href="">Ticket System</a></li>
						<li><a href="">Game Wiki</a></li>
						<li><a href="">Contact Support</a></li>
					</ul>
				</div>
				<div class="footerMenu footerMenu-soc">
					<span>Follow Us</span>
					<ul>
						<li><a href=""><i class="icon-soc fb"></i> Facebook</a></li>
						<li><a href=""><i class="icon-soc md"></i> granadoespadaDownloads</a></li>
						<li><a href=""><i class="icon-soc ep"></i> Elitepvpers</a></li>
						<li><a href=""><i class="icon-soc ds"></i> Discord</a></li>
					</ul>
				</div>
			</div>
		</footer>
    </div>
    
</template>
<script>
    import AppHeader from './AppHeader.vue';
	import AppSideBar from './AppSideBar.vue'
    // import LeftPanel from '../components/LeftPanel.vue';
    // import RightPanel from '../components/RightPanel.vue';
    // import BottomMenu from '../components/BottomMenu.vue';
    // import AppOverLay from './AppOverLay.vue';

    

    import Modal from "@/components/modals/index.vue";

    export default {
        name: 'default',
        components: {AppHeader, AppSideBar, Modal},
		data() {
			return {
			};
		},
    }
</script>
<style lang="scss" scoped>

</style>