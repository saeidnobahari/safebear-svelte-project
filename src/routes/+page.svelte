<script>
	import Safebear from '$lib/images/safebear.png';
	import Button, { Label } from '@smui/button';
</script>

<svelte:head>
	<title>Welcome</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<div class="welcome-copy-wrapper">
		<h1>
			Safebear, la solution anti<br /> <span class="underline-text">cyber harcèlement</span> et
			<span class="underline-text">tricheurs</span>
		</h1>
	</div>
	<div class="description-wrapper">
		<div class="description-card-wrapper">
			<img src={Safebear} alt="SafeBear" width="119" height="119" />
			<p class="card-text">
				SafeBear est une solution multiplateforme qui protège ses utilisateurs de la toxicité sur
				internet en utilisant la technologie blockchain dans le web3
			</p>
		</div>
		<div class="description-text-wrapper">
			<div class="line-wrapper" />
			<p class="desc-p first-p">
				SafeBear s’engage à accompagner ses clients, grâce à une aide juridique incluse dans la
				solution
			</p>
			<div class="line-wrapper" />
			<p class="desc-p second-p">
				De plus SafeBear garantit la non-utilisation des données utilisateurs à des fins
				commerciales
			</p>
			<div class="line-wrapper" />
		</div>
	</div>
	<div class="button-wrapper">
		<Button type="button" variant="raised" class="safebear-button button-shaped-round">
			<Label>Accéder à Safebear</Label>
		</Button>
	</div>
</section>

<style>
	@font-face {
		font-family: Poppins;
		src: url('$lib/fonts/Poppins/Poppins-Medium.ttf');
	}

	:global(.safebear-button) {
		padding: 19px 54.5px;
		border-radius: 999px;
		border: none;
		background-color: #007d82;
		color: white;
		font-family: 'Poppins';
		font-style: normal;
		font-size: 20px;
		line-height: 30px;
	}

	section {
		position: relative;
		display: flex;
		flex-direction: column;
		width: 100%;
		height: 1080px;
	}
	h1 {
		position: absolute;
		left: 12.15%;
		right: 15.62%;
		top: 16.76%;
		bottom: 67.69%;
		/* margin-top: 293px;
		margin-left: 175px; */
		width: fit-content;

		font-family: Poppins;
		font-style: normal;
		font-weight: 600;
		font-size: 64px;
		line-height: 131.4%;
		/* or 84px */

		color: #2a4a51;
	}
	img {
		margin-bottom: 8px;
		margin: 58px 0 0 15px;
	}
	.welcome-copy-wrapper {
		width: 100%;
		height: 645px;
		margin-top: -112px;

		background: linear-gradient(0deg, rgba(130, 195, 208, 0.4), rgba(130, 195, 208, 0.4)), #ffffff;
		box-shadow: 0px 4px 18px rgba(0, 0, 0, 0.07);
		border-bottom-left-radius: 55%;
		border-bottom-right-radius: 55%;
	}
	.underline-text {
		border-bottom: 2px solid #007d82;
		color: #007d82;
	}
	.description-wrapper {
		display: flex;
		flex-direction: row;
		align-items: center;
		margin: -90px 0 0 145px;
	}
	.description-card-wrapper {
		width: 590px;
		border-radius: 29px;
		margin-right: 30px;
		background-color: white;
		box-shadow: 0px 56px 37px -32px rgba(42, 74, 81, 0.18);
		backdrop-filter: blur(10px);
	}
	.card-text {
		font-family: Poppins;
		font-style: normal;
		font-weight: 500;
		font-size: 24px;
		line-height: 36px;
		margin: 0 30px;
		margin-bottom: 66px;
		/* Dark green */

		color: #2a4a51;
	}
	.description-text-wrapper {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 530px;
	}
	.line-wrapper {
		width: 100%;
		height: 0;
		border-top: 3px solid #007d82;
	}
	.desc-p {
		width: 526px;
		font-family: Poppins;
		font-style: normal;
		font-weight: 500;
		font-size: 24px;
		line-height: 36px;
		color: rgba(0, 125, 130, 1);
	}
	.first-p {
		margin: 19px 2px;
	}
	.second-p {
		margin: 26px 2px;
	}
	.button-wrapper {
		margin-top: 71px;
		margin-left: auto;
		margin-right: auto;
	}
</style>
