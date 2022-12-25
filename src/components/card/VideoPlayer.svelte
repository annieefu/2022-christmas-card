<script>
	import Player from "@vimeo/player";
	import { onMount } from "svelte";


    onMount(() =>{

        if (document.getElementById('#vimeo-frame')){
            const frame = document.querySelector('iframe')
            const player = new Vimeo.Player(frame);


            player.on('play', function() {
            console.log('played the video!');
            });

        }
        
        
        

    });

</script>

<div class="player-container">


	<div id = "vimeo-frame" style="padding:75% 0 0 0;position:relative; z-index: 5;">
		<iframe
			src="https://player.vimeo.com/video/784209660?h=e48d6b3e81&amp;autoplay=1&amp;muted=1&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
			frameborder="0"
			allow="autoplay; fullscreen;"
			allowfullscreen
			style="position:absolute;top:0;left:0;width:100%;height:100%;"
            title="S"
		/>
	</div>


</div>

<style>


	.player-container {
		max-width: 95%;
		padding-top: 40%;
		z-index: 5;
        margin-left: 2.5%;
        margin-right: 2.5;
        opacity: 0;

            animation: fadeIn 3s;
            -webkit-animation: fadeIn 3s;
            -moz-animation: fadeIn 3s;
            -o-animation: fadeIn 3s;
            -ms-animation: fadeIn 3s;
            animation-delay: 5.5s;
            animation-fill-mode: forwards;
	}

	@media (min-width: 768px) {
		.player-container {
			z-index: 5;
			width: 80%;
		padding-top: 25%;
			/* padding-bottom: 10%; */
			margin-left: 10%;
			margin-right: 10%;
            animation: fadeIn 3s;
            -webkit-animation: fadeIn 3s;
            -moz-animation: fadeIn 3s;
            -o-animation: fadeIn 3s;
            -ms-animation: fadeIn 3s;
            animation-delay: 5s;
animation-fill-mode: forwards;
		}
	}


	@media (min-width: 960px) {
		.player-container {
			z-index: 5;
			width: 60%;
		    padding-top: 12%;
			margin-left: 20%;
			margin-right: 20%;
            animation: fadeIn 3s;
            -webkit-animation: fadeIn 3s;
            -moz-animation: fadeIn 3s;
            -o-animation: fadeIn 3s;
            -ms-animation: fadeIn 3s;
            animation-delay: 5s;
animation-fill-mode: forwards;
		}
	}




    
    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    
    @-moz-keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    
    @-webkit-keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    
    @-o-keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    
    @-ms-keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
</style>
