<div class="post">
	<div class="post-head">
		<img
			width="40"
			height="40"
			alt="Username"
			loading="lazy"
			class="post-head__img-profile"
			src="https://avatars.dicebear.com/api/croodles-neutral/apriliandi.svg?size=40"
		/>

		<a href="/user/_apriliandi_" class="post__username post-user">_apriliandi_</a>
		<span class="middle-dot">·</span>
		<span class="post-head__date">6 Apr</span>
	</div>

	<div class="post-words">
		Svelte is a radical new approach to building user interfaces. Whereas traditional frameworks
		like React and Vue do the bulk of their work in the browser, Svelte shifts that work into a
		compile step that happens when you build your app.. Instead of using techniques like virtual DOM
		diffing, Svelte writes code that surgically updates the DOM when the state of your app changes.
	</div>
</div>

<style>
	.post {
		width: 100%;
		border-radius: 3px;
		margin-bottom: 26px;
		padding: 18px 17px 20px 17px;
		background-color: var(--grey-50);
		border: 1px solid var(--primary-900);
	}

	.post-head {
		display: flex;
		align-items: center;
	}

	.post-head__img-profile {
		font-size: 13px;
		overflow: hidden;
		margin-right: 14px;
		border-radius: 100%;
		color: var(--primary-900);
		background-color: var(--grey-200);
		border: 1px solid var(--primary-900);
	}

	.post__username:hover {
		background-color: var(--primary-50);
	}

	.post__username:focus {
		outline-offset: 0px;
		outline: 2px solid var(--primary-900);
	}

	.post-user {
		font-size: 15px;
		font-weight: 600;
		padding: 4px 12px;
		border-radius: 3px;
		letter-spacing: 0.5px;
		color: var(--grey-900);
		border: 1px solid var(--primary-900);
	}

	.post-words {
		font-size: 15px;
		margin-top: 15px;
		line-height: 27px;
		padding: 8px 13px;
		border-radius: 3px;
		letter-spacing: 0.5px;
		color: var(--grey-900);
		border: 1px solid var(--primary-900);
	}

	.post-head__date {
		padding: 2px 10px;
		border-radius: 3px;
		color: var(--grey-600);
		font-size: var(--text-14x);
		border: 1px solid var(--primary-900);
	}

	.middle-dot {
		margin: 0 12px;
		font-weight: 500;
		font-size: var(--text-36x);
	}

	@media screen and (min-width: 483px) and (max-width: 550px) {
		.post {
			padding: var(--space-16x);
		}
	}
</style>
